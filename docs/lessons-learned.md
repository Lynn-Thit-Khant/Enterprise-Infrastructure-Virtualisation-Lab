# Lessons Learned

## Infrastructure Planning

This lab showed that virtualisation is not only about creating virtual machines. Proper planning is needed for networking, storage, host placement, backup, and recovery.

## Storage Design Matters

Different workloads benefit from different storage protocols. NFS, iSCSI, and SMB each serve different operational needs.

## Recovery Must Be Tested

Creating a backup is not enough. Restore testing is required to prove that the backup can actually support recovery.

## Live Migration Requirements

Live migration depends on shared storage, network connectivity, compatible host configuration, and sufficient destination resources.

## Documentation Improves Operations

Clear documentation makes an infrastructure environment easier to understand, troubleshoot, rebuild, and explain during technical interviews.
