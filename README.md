# vmware-mokutil-keygen
VMWare Error: Cannot open /dev/vmmon: No such file or directory. Please make sure that the kernel module 'vmmon' is loaded.

On a Linux host with secure mode enabled, it is not allowed to load any unsigned drivers. Due to this, VMware drivers, such as vmmon and vmnet, are not able to be loaded which prevents virtual machine to power on.

The Script automates the steps to sign VMware drivers on Linux host with secure boot enabled, so that VMware Workstation can run VMs successfully.

# Installation
1. Make file executable (sudo chmod +x vmpatch).
2. Run the script (./vmpatch).
3. Enter a password for the MOK enrollment request.
4. Reboot your device. A blue screen will pop up upon boot. Follow the instructions to complete the enrollment from the UEFI console.
5. When your machine reboots, try running the virtual machine again. If it fails, repeat the process or enter in the commands one line at a time.
