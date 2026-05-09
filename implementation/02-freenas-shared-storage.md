# FreeNAS Shared Storage Setup

## Purpose

FreeNAS provides shared storage for virtual machine disks, backup exports, and installation media.

## Storage Pools

| Storage Area | Purpose |
|---|---|
| NFS pool | Linux web server VM storage |
| iSCSI pool | Windows Remote Desktop VM storage |
| SMB share | VM backup exports and ISO files |

## Implementation Steps

1. Install and configure FreeNAS.
2. Assign a static management IP address.
3. Create storage pools based on workload requirements.
4. Configure NFS share for Linux VM storage.
5. Configure iSCSI target for Windows VM storage.
6. Configure SMB share for backups and ISO files.
7. Connect XenServer hosts to the storage repositories.

## Validation

- Confirm FreeNAS services are running.
- Confirm XenServer can access NFS storage.
- Confirm Windows VMs can use iSCSI-backed storage.
- Confirm backup files can be written to the SMB share.

## Notes

Storage separation improves manageability by keeping active VM storage and backup storage logically separated.
