# Network Connectivity Validation

## Purpose

Network connectivity testing confirms that hosts, storage, and virtual machines can communicate across the private infrastructure network.

## Example Tests

| Source | Destination | Test | Expected Result |
|---|---|---|---|
| XenServer host | Gateway | ping gateway | Successful response |
| XenServer host | FreeNAS01 | ping storage IP | Successful response |
| Web-SG | Web-JP | ping web server IP | Successful response |
| Remote Desktop VM | Web servers | browser or ping test | Successful access |

## Commands

```bash
ping 172.16.110.1
ping 172.16.110.77
ping 172.16.110.86
ping 172.16.110.64
ping 172.16.110.37
ping 172.16.110.62
```

## Notes

Successful ping tests confirm network reachability, but service-level testing is still required to confirm that applications are functioning.
