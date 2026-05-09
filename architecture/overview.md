# Architecture Overview

This lab simulates an enterprise infrastructure consolidation project.

The original environment used separate physical servers for web and remote desktop workloads across multiple regional offices. The redesigned environment uses virtual machines hosted on XenServer, with FreeNAS providing shared storage for different workload types.

## Main Components

### XenServer Hosts

Two XenServer hosts were used to run regional workloads:

| Host | Purpose |
|---|---|
| XS-SG-TH | Hosts Singapore and Thailand workloads |
| XS-JP-TW | Hosts Japan and Taiwan workloads |

### Shared Storage

FreeNAS was used as the shared storage platform for:

- Linux web server virtual machines
- Windows Remote Desktop virtual machines
- Backup exports and recovery files

### Backup/Recovery Host

A separate backup/recovery host was included to validate migration and recovery procedures.

## High-Level Design

```text
Regional Workloads
      |
      v
+-------------------+       +-------------------+
|   XS-SG-TH Host   |       |   XS-JP-TW Host   |
|  Web-SG / Web-TH  |       |  Web-JP / Web-TW  |
|  RD-Singapore     |       |  RD-JP            |
+---------+---------+       +---------+---------+
          \                         /
           \                       /
            v                     v
              +-----------------+
              |    FreeNAS01    |
              | Shared Storage  |
              | NFS/iSCSI/SMB   |
              +--------+--------+
                       |
                       v
              +-----------------+
              |    XS-Backup    |
              | Recovery Host   |
              +-----------------+
```

## Purpose

The architecture demonstrates how physical workloads can be consolidated into virtual machines while maintaining shared storage access, backup capability, and migration flexibility.
