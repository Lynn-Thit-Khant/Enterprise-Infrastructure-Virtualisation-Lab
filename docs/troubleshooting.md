# Troubleshooting

## VM cannot reach network

Check:

- VM network adapter is connected
- Correct virtual network is selected
- IP address and gateway are configured
- Host network connectivity is working

## FreeNAS storage is not visible

Check:

- FreeNAS service is running
- NFS/iSCSI/SMB service is enabled
- Correct storage path or target is configured
- XenServer host can ping FreeNAS
- Storage repository credentials and access permissions are correct

## Apache web server does not respond

Check:

```bash
sudo systemctl status apache2
```

Also verify:

- VM IP address
- firewall rules
- Apache service status
- browser access from Remote Desktop VM

## VM migration fails

Check:

- Shared storage is accessible by both hosts
- Destination host has enough CPU and memory resources
- Hosts are reachable over the network
- VM disk is located on shared storage
- Host compatibility requirements are met

## Restore fails

Check:

- Backup file is not corrupted
- Storage destination has enough space
- Correct import format is selected
- Network and VM settings are reviewed after restore
