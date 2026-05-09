# Network Design

The lab uses a private network for communication between hypervisors, shared storage, and virtual machines.

## Network Summary

| Item | Value |
|---|---|
| Network | 172.16.110.0/24 |
| Gateway | 172.16.110.1 |
| Purpose | Private infrastructure communication |

## Main Host IP Plan

| Host / VM | Role | IP Address |
|---|---|---|
| XS-SG-TH | XenServer host for Singapore/Thailand workloads | 172.16.110.96 |
| XS-JP-TW | XenServer host for Japan/Taiwan workloads | 172.16.110.94 |
| FreeNAS01 | Shared storage server | 172.16.110.77 |
| Web-SG | Singapore Linux web server | 172.16.110.86 |
| Web-TH | Thailand Linux web server | 172.16.110.64 |
| Web-JP | Japan Linux web server | 172.16.110.37 |
| Web-TW | Taiwan Linux web server | 172.16.110.62 |

## Design Notes

- Static IP addressing was used to make infrastructure access predictable.
- The private network allows hosts, storage, and VMs to communicate within the lab environment.
- Connectivity testing should be performed using ping and service-level checks after deployment.
