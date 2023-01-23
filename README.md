# SBKS-RC (Slack-Build-Kernel-Script) 

Is a bash script for auto download, build, and install TESTING Linux-kernel-RC for Slackware and Slack based systems.
### RUN this script  ONLY if you are buildning TESTING kernels from https://git.kernel.org/torvalds/t/ 
### Otherwise use aparently the MAIN script (https://gitlab.com/rizitis/SBKS)

How to edit this script for testing kernels in Slackware
Add the direct link of Linux kernel source at the first place were is LINK=
ADD KERNEL_VERSION exactly the same 
ADD VERSION2 as is in the example (add a zero 0) else kernel modules will not be install
also if you use custom old config with your tag in kernel name add it on VERSION2 too. example: (VERSION2=6.2.0-rc5-rtz) 

example:
```
LINK=https://git.kernel.org/torvalds/t/linux-6.2-rc5.tar.gz
KERNEL_VERSION=6.2-rc5
VERSION2=6.2.0-rc5
```
SBKS wont remove or upgrade older Linux kernel versions that allready exist in your system.
 
## NOTE
This script in ONLY for testing kernels (for example 6.2-RC)
It no suggested for Slackware stable and ofcource suggested for currend if you want to help devs...else no reason for it.  


