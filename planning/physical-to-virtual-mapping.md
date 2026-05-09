# Physical-to-Virtual Mapping

## Purpose

This file documents how the original physical server environment was mapped into a virtualised environment.

## Consolidation Summary

| Original Infrastructure | Virtualised Infrastructure |
|---|---|
| 9 physical servers | 6 virtual machines |
| Separate physical web servers | Linux web server VMs |
| Separate physical Remote Desktop servers | Windows Remote Desktop VMs |
| Physical storage server | FreeNAS shared storage |
| Manual maintenance and recovery | VM migration, export, import, and restore workflows |

## Virtual Machine Mapping

| Virtual Machine | Workload | Region |
|---|---|---|
| Web-SG | Linux web server | Singapore |
| Web-TH | Linux web server | Thailand |
| Web-JP | Linux web server | Japan |
| Web-TW | Linux web server | Taiwan |
| RD-Singapore | Windows Remote Desktop | Singapore/Thailand |
| RD-JP | Windows Remote Desktop | Japan/Taiwan |

## Outcome

The mapping reduced hardware dependency while keeping workloads logically separated by region and service type.
