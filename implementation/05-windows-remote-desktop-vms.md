# Windows Remote Desktop VM Setup

## Purpose

Windows Remote Desktop virtual machines provide administrative access to regional workloads.

## Implementation Steps

1. Deploy Windows Remote Desktop virtual machines.
2. Install XenServer Tools for better VM performance.
3. Enable Remote Desktop access.
4. Configure firewall rules for RDP.
5. Connect Windows VMs to appropriate storage.
6. Validate RDP access and disk availability.

## Validation

- Confirm Remote Desktop is enabled.
- Confirm the VM is reachable on the network.
- Confirm login access works.
- Confirm storage is visible and usable inside Windows.
- Confirm the VM remains functional after backup or migration testing.

## Notes

Remote Desktop systems were allocated more memory and storage than web servers because they support interactive sessions and Windows system requirements.
