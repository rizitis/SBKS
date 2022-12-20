SBKS (Slack-Build-Kernel-Script) 

Is a bash script for auto download, build, and install a new Linux kernel for Slackware and Slack based systems.
On the top of script you just have to edit Kernel version any time you use it.
```
KERNEL_URL=https://cdn.kernel.org/pub/linux/kernel/v6.x
KERNEL_VERSION=6.0.14
VERSION2=6.0.14
```
SBKS wont remove or upgrade older Linux kernel versions that allready exist in your system.
It is tested to Slackware64 15+ and Slackel
