# Service Validation

## Purpose

Service validation confirms that deployed workloads are accessible and functional.

## Linux Web Server Validation

Test Apache using a browser or curl:

```bash
curl http://<web-server-ip>
```

Expected result:

- Apache responds successfully
- Web page loads from the target VM

## Remote Desktop Validation

For Windows Remote Desktop VMs:

- Confirm RDP is enabled
- Confirm firewall allows RDP
- Confirm login is successful
- Confirm the VM remains responsive

## Service Validation Table

| Service | Validation Method | Expected Result |
|---|---|---|
| Apache | Browser or curl | Web page loads |
| Remote Desktop | RDP client | Login succeeds |
| Shared Storage | Storage repository check | Storage visible and usable |
| Backup Share | File write/read test | Backup files accessible |
