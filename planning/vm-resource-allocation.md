# VM Resource Allocation

## Virtual Machine Resources

| VM Name | Location | OS | vCPU | RAM | Storage | Purpose |
|---|---|---|---|---|---|---|
| Web-SG | Singapore | Ubuntu Linux | 1 | 2 GB | 10 GB | Web Server |
| Web-TH | Thailand | Ubuntu Linux | 1 | 2 GB | 10 GB | Web Server |
| Web-JP | Japan | Ubuntu Linux | 1 | 2 GB | 10 GB | Web Server |
| Web-TW | Taiwan | Ubuntu Linux | 1 | 2 GB | 10 GB | Web Server |
| RD-Singapore | Singapore/Thailand | Windows | 1 | 4 GB | 24 GB | Remote Desktop |
| RD-JP | Japan/Taiwan | Windows | 1 | 4 GB | 24 GB | Remote Desktop |

## Design Notes

- Linux web servers were allocated lighter resources because they served simple web workloads.
- Windows Remote Desktop VMs were allocated more RAM and storage to support interactive desktop usage.
- VM resource sizing was kept simple and consistent to make the lab easier to validate and manage.
