# Storage Protocol Selection

## Purpose

Storage protocols were selected based on workload requirements rather than using a single storage method for all systems.

## Selection Table

| Workload | Protocol | Reason |
|---|---|---|
| Linux web servers | NFS | Suitable for Linux file-level shared storage |
| Windows Remote Desktop VMs | iSCSI | Provides block-level storage suitable for Windows system disks |
| Backup exports and ISO files | SMB | Simple shared file access for backup and recovery files |

## Design Reasoning

Using separate protocols makes the storage design more aligned to each workload:

- Linux systems benefit from NFS because it is commonly used for Unix/Linux file sharing.
- Windows systems benefit from iSCSI because it behaves like a local disk.
- Backup workflows benefit from SMB because it provides accessible shared storage for exported VM files.

## Outcome

The result is a more organised shared storage architecture that supports workload separation and recovery planning.
