# VM Export and Import

## Purpose

VM export and import procedures were used to validate backup and restore capability.

## Export Methods

### XVA Export

XVA export creates a full VM backup suitable for restoring within XenServer environments.

### OVF/OVA Export

OVF/OVA export provides a more portable VM backup format that can be useful for compatibility and recovery scenarios.

## Restore Validation

A restore test should confirm:

- The VM imports successfully.
- The VM boots without errors.
- Network connectivity works.
- Required services are running.
- Data and configuration are intact.

## Validation Checklist

- [ ] Backup file exists in SMB backup storage
- [ ] VM import completes successfully
- [ ] VM starts successfully
- [ ] VM network connectivity is confirmed
- [ ] Application/service access is confirmed

## Notes

Restore validation is a key part of disaster recovery. A backup that has not been tested should not be assumed reliable.
