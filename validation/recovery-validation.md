# Recovery Validation

## Purpose

Recovery validation confirms that backups and migration workflows produce usable results.

## VM Restore Validation

After importing or restoring a VM, confirm:

- VM boots successfully
- Correct IP address is configured
- Network connectivity works
- Required services respond
- Data and configuration are intact

## Live Migration Validation

After live migration, confirm:

- VM appears on the destination host
- VM remains reachable
- Application service continues to respond
- No major downtime is observed

## Backup File Validation

For exported VM backups:

- Confirm backup file exists
- Confirm file size is reasonable
- Confirm import or restore procedure completes
- Confirm restored VM operates correctly

## Notes

Recovery validation is one of the most important parts of infrastructure operations. Backups should be tested regularly, not only created.
