# Infrastructure Design

## Design Goal

The main goal was to redesign a physical server environment into a virtualised infrastructure that is easier to manage, recover, and scale.

## Original Environment

The original setup consisted of multiple physical servers for:

- Linux web servers
- Windows Remote Desktop systems
- Storage services

These systems were distributed across regional workloads and required separate hardware resources.

## Redesigned Environment

The redesigned environment uses:

- XenServer for virtual machine hosting
- XenCenter for centralised management
- FreeNAS for shared storage
- Virtual machines for Linux and Windows workloads
- Backup and restore workflows for recovery readiness

## Consolidation Approach

The environment consolidates **9 physical servers into 6 virtual machines**.

| Workload Type | Original Approach | Virtualised Approach |
|---|---|---|
| Web Servers | Separate physical Linux servers | Linux web server VMs |
| Remote Desktop | Separate physical Windows servers | Windows Remote Desktop VMs |
| Storage | Dedicated storage server | FreeNAS shared storage |
| Recovery | Manual rebuild/restore | VM backup, export, import, and migration |

## Design Benefits

- Reduced hardware dependency
- Faster provisioning of new virtual machines
- Centralised management through XenCenter
- Easier backup and recovery validation
- More flexible maintenance through live migration
