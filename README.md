# Enterprise Infrastructure Virtualisation Lab

## Overview

This lab simulates an enterprise infrastructure consolidation scenario using XenServer and FreeNAS. The environment was designed to reduce physical server dependency, centralise virtual machine management, and validate backup, restore, and live migration procedures.

The lab models a company environment with regional workloads across Singapore, Japan, Taiwan, and Thailand. The original physical server setup was redesigned into a virtualised infrastructure using shared storage and multiple hypervisor hosts.

## Problem Scenario

The simulated organisation faced several infrastructure challenges:

- Multiple physical servers across different regional workloads
- Slow deployment of new infrastructure
- Overprovisioned hardware resources
- Limited recovery flexibility during failures
- Maintenance windows that could affect service availability

## Solution

The solution uses a virtualised architecture with XenServer hosts, FreeNAS shared storage, and workload-specific storage protocols.

The infrastructure design consolidates **9 physical servers into 6 virtual machines** across a **2-host virtualisation environment**, with a dedicated backup/recovery host used for recovery testing.

## Key Outcomes

- Consolidated 9 physical servers into 6 virtual machines
- Designed a 2-host virtualisation environment using XenServer
- Configured FreeNAS shared storage for Linux, Windows, and backup workloads
- Used NFS for Linux web servers, iSCSI for Windows Remote Desktop systems, and SMB for backup storage
- Tested live virtual machine migration to validate maintenance flexibility
- Validated backup exports, restore procedures, and recovery readiness

## Technologies Used

- XenServer
- XenCenter
- FreeNAS
- Virtual Machines
- NFS
- iSCSI
- SMB
- Ubuntu Linux
- Windows Remote Desktop
- Apache

## Repository Structure

| Folder | Purpose |
|---|---|
| `architecture/` | High-level infrastructure design, network layout, and storage design |
| `planning/` | Physical-to-virtual mapping, VM resources, hostname/IP plan, and protocol selection |
| `implementation/` | Build documentation for XenServer, FreeNAS, VMs, web servers, and RDP systems |
| `backup-recovery/` | Backup strategy, VM export/import, live migration, and disaster recovery planning |
| `validation/` | Testing checklists and validation notes for connectivity, services, and recovery |
| `docs/` | Design decisions, troubleshooting notes, and lessons learned |

## Skills Demonstrated

- Infrastructure design
- Virtualisation planning
- Shared storage design
- Virtual machine deployment
- Backup and recovery planning
- Live migration validation
- Network and service testing
- Technical documentation

## Outcome

This lab demonstrates the ability to plan, build, validate, and document a virtualised infrastructure environment. It presents a practical simulation of enterprise infrastructure consolidation, with attention to storage design, service continuity, and recovery readiness.
