# Disaster Recovery Plan

## Purpose

This file outlines recovery approaches for common infrastructure failure scenarios.

## Scenario 1: Virtual Machine Failure

Recovery steps:

1. Identify the failed VM.
2. Locate the latest valid backup export.
3. Import or restore the VM.
4. Start the VM.
5. Validate network and service access.

## Scenario 2: Hypervisor Host Failure

Recovery steps:

1. Confirm whether shared storage remains available.
2. Register or restore affected VMs on another host.
3. Start required VMs.
4. Validate service availability.
5. Document the incident and recovery result.

## Scenario 3: Storage Failure

Recovery steps:

1. Identify affected storage pool or share.
2. Restore backup files to available storage.
3. Reattach VM disks or import VM backups.
4. Validate VM boot and data integrity.
5. Review storage redundancy and backup frequency.

## Notes

Disaster recovery planning should include both technical restore steps and validation steps. Recovery is only successful when services are confirmed operational.
