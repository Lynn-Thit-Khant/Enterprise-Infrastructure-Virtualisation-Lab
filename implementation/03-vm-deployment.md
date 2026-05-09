# Virtual Machine Deployment

## Purpose

Deploy Linux and Windows virtual machines to replace the original physical server workloads.

## Virtual Machines

| VM | OS | Purpose |
|---|---|---|
| Web-SG | Ubuntu Linux | Singapore web server |
| Web-TH | Ubuntu Linux | Thailand web server |
| Web-JP | Ubuntu Linux | Japan web server |
| Web-TW | Ubuntu Linux | Taiwan web server |
| RD-Singapore | Windows | Remote Desktop access for Singapore/Thailand |
| RD-JP | Windows | Remote Desktop access for Japan/Taiwan |

## Implementation Steps

1. Create virtual machines from installation media.
2. Assign CPU, memory, and storage based on workload type.
3. Connect VMs to the private infrastructure network.
4. Install required operating systems.
5. Configure network settings and service access.
6. Validate VM boot and network connectivity.

## Validation

- Confirm each VM boots successfully.
- Confirm each VM receives or uses the correct IP configuration.
- Confirm ping connectivity between relevant systems.
- Confirm web and Remote Desktop services respond correctly.
