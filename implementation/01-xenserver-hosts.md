# XenServer Host Setup

## Purpose

XenServer hosts provide the compute layer for the virtualised infrastructure.

## Hosts

| Host | Purpose |
|---|---|
| XS-SG-TH | Hosts Singapore and Thailand workloads |
| XS-JP-TW | Hosts Japan and Taiwan workloads |
| XS-Backup | Used for backup, recovery, and migration testing |

## Implementation Steps

1. Install XenServer on each host.
2. Assign static management IP addresses.
3. Connect each host to XenCenter for centralised management.
4. Attach shared storage repositories from FreeNAS.
5. Validate host connectivity and storage access.

## Validation

- Confirm hosts appear in XenCenter.
- Confirm each host can reach FreeNAS.
- Confirm storage repositories are available.
- Confirm VMs can be created and started successfully.

## Notes

Centralised management through XenCenter makes it easier to monitor hosts, manage virtual machines, and perform migration or backup tasks.
