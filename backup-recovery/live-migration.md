# Live Migration

## Purpose

Live migration was used to validate maintenance flexibility by moving a virtual machine between hosts while maintaining service continuity.

## Migration Scenario

The Web-TW virtual machine was migrated from the Japan/Taiwan host to the backup/recovery host.

| VM | Source Host | Destination Host |
|---|---|---|
| Web-TW | XS-JP-TW | XS-Backup |

## Prerequisites

- Shared storage accessible by both source and destination hosts
- Compatible host configuration
- Network connectivity between hosts
- Sufficient resources on destination host
- VM storage available through shared storage

## Validation Steps

After migration, validate:

- VM appears under the destination host
- VM starts or continues running
- VM IP address remains reachable
- Web service responds correctly
- No unexpected service interruption occurs

## Outcome

The live migration test demonstrates how planned maintenance can be performed with reduced downtime risk.
