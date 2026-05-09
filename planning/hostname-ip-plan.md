# Hostname and IP Plan

## Purpose

A clear hostname and IP plan makes the environment easier to manage, test, and troubleshoot.

## Infrastructure Hosts

| Hostname | Role | IP Address |
|---|---|---|
| XS-SG-TH | XenServer host | 172.16.110.96 |
| XS-JP-TW | XenServer host | 172.16.110.94 |
| FreeNAS01 | Shared storage server | 172.16.110.77 |
| XS-Backup | Backup/recovery host | Lab-assigned IP |

## Virtual Machines

| VM Name | Role | IP Address |
|---|---|---|
| Web-SG | Singapore web server | 172.16.110.86 |
| Web-TH | Thailand web server | 172.16.110.64 |
| Web-JP | Japan web server | 172.16.110.37 |
| Web-TW | Taiwan web server | 172.16.110.62 |
| RD-Singapore | Remote Desktop VM | Lab-assigned IP |
| RD-JP | Remote Desktop VM | Lab-assigned IP |

## Notes

The IPs above reflect the lab environment and should be adjusted if the project is recreated on a different subnet.
