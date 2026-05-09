# Storage Design

FreeNAS was used as the shared storage platform for the virtualised infrastructure.

The storage design separates workloads by protocol based on the type of virtual machine and operational need.

## Storage Protocol Mapping

| Protocol | Used For | Purpose |
|---|---|---|
| NFS | Linux web server virtual machines | File-level storage suitable for Linux workloads |
| iSCSI | Windows Remote Desktop virtual machines | Block-level storage suitable for Windows system disks |
| SMB | Backup storage | Shared location for VM exports, ISO files, and recovery files |

## Why Different Storage Protocols Were Used

### NFS for Linux Web Servers

NFS is suitable for Linux workloads because it integrates well with Linux file systems and supports shared access to web server storage.

### iSCSI for Windows Remote Desktop VMs

iSCSI provides block-level storage, which appears like a local disk to Windows systems. This makes it suitable for Windows Remote Desktop virtual machines.

### SMB for Backup Storage

SMB provides simple file sharing for backup exports and recovery files. It is easy to access from management workstations and infrastructure hosts.

## Storage Design Outcome

The storage design supports different workload types while keeping backup files separate from active virtual machine storage.
