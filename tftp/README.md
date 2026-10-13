# TFTP boot files

The boot flow expects these files to be available from the configured
TFTP server:

- `zImage` — Linux kernel image
- `vexpress-v2p-ca15-tc1.dtb` — Device Tree Blob for the QEMU VExpress
  platform

The files used during the original test are not included here yet.
Use files built from a compatible Linux kernel source tree and ensure
that the TFTP server serves them under the filenames expected by U-Boot.

The TFTP server address in the example configuration is `192.168.100.1`.
Adjust it if your host-side network configuration differs.
