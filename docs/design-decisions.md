# Design Decisions

## Virtualisation Instead of Physical Expansion

Virtualisation was used to reduce hardware dependency and improve manageability. Instead of adding more physical servers, workloads were consolidated into virtual machines.

## Two-Host Design

A two-host design was used to separate regional workloads and support migration testing. This also simulates a more realistic infrastructure layout than a single-host lab.

## FreeNAS Shared Storage

FreeNAS was used to provide centralised shared storage for virtual machines and backup exports.

## Workload-Specific Storage Protocols

Different storage protocols were selected based on workload needs:

- NFS for Linux web servers
- iSCSI for Windows Remote Desktop virtual machines
- SMB for backup exports and ISO files

## Backup and Restore Validation

Backup validation was included because a backup process is incomplete unless restoration is tested.

## Live Migration

Live migration was included to demonstrate how planned maintenance can be performed while reducing downtime risk.
