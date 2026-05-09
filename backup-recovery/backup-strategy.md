# Backup Strategy

## Purpose

Backup planning ensures virtual machines and critical services can be recovered after failure or maintenance issues.

## Backup Methods

| Method | Purpose |
|---|---|
| XVA Export | Full virtual machine backup |
| OVF/OVA Export | Portable VM backup for cross-platform compatibility |
| Snapshots | Point-in-time rollback before changes |
| File-level backup | Recovery of specific files when full VM restore is not required |

## Backup Destination

Backup exports were stored on SMB shared storage provided by FreeNAS.

## Recommended Backup Flow

1. Identify the VM to back up.
2. Export the VM using XVA or OVF/OVA.
3. Store the export on the SMB backup share.
4. Verify the backup file exists.
5. Perform test restore or import validation.
6. Document the result.

## Notes

Backup creation alone is not enough. Backups should be validated through restore testing to confirm they are usable.
