# List of useful software

1. [Visual Studio Code](https://code.visualstudio.com/)



## Windows

1. [Chocolatey](https://chocolatey.org/) Package manager for Windows. 
2. Cmder - Terminal emulator
3. Hyper.js - Configurable Terminal Emulator

### Tips

* [Fix Windows update issues ( Win 8/8.1/10)](https://support.microsoft.com/en-us/help/10164/fix-windows-update-errors)

### Auto mount NTFS (internal/external) partitions
Edit `/etc/fstab` to add NTFS partitons
``` console
# <file system> <mount point>   <type>  <options>       <dump>  <pass>
#
UUID=6C45-C882 /boot/efi vfat defaults,rw,relatime 0 0
UUID=222eadcb-81a5-4e34-9b5d-4cb28c1800bb swap swap defaults 0 0
UUID=a5015c69-934b-468e-b405-e4ad0e7eda32 / ext4 defaults,rw,lazytime,data=ordered 0 1
UUID=fb3a61e4-a139-48bf-8a3c-7b507dd4c8e6 /home ext4 defaults,rw,lazytime,data=ordered 0 0
UUID=1EE27CA3E27C80B7 /media/kranti/New\040Volume ntfs    defaults,relatime,nofail,x-systemd.device-timeout=1    0   0
UUID=20F67F21F67EF67E /media/kranti/external/ ntfs    defaults,nofail,relatime,x-systemd.device-timeout=1    0   0
#tmpfs	/home/kranti/.cache	tmpfs	noatime,nodev,nosuid	0	0
```
