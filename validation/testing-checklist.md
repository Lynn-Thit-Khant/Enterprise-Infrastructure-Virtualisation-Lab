# Testing Checklist

## Infrastructure

- [ ] XenServer hosts are reachable
- [ ] XenCenter can manage all hosts
- [ ] FreeNAS is reachable from hypervisor hosts
- [ ] Shared storage repositories are visible
- [ ] VMs can start successfully

## Network

- [ ] Hosts can reach the gateway
- [ ] Hypervisor hosts can reach FreeNAS
- [ ] VMs can reach other required VMs
- [ ] Web server IPs are reachable
- [ ] Remote Desktop VMs are reachable

## Services

- [ ] Apache is running on Linux web servers
- [ ] Web pages load successfully
- [ ] Remote Desktop access works
- [ ] Storage access works as expected

## Backup and Recovery

- [ ] VM export completes successfully
- [ ] Backup files are stored on SMB share
- [ ] VM import or restore test succeeds
- [ ] Restored VM boots successfully
- [ ] Services work after restoration

## Migration

- [ ] Migration prerequisites are met
- [ ] VM migration completes successfully
- [ ] VM is visible on the destination host
- [ ] Network and service access continue after migration
