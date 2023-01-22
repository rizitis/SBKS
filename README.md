SBKS (Slack-Build-Kernel-Script) 

Is a bash script for auto download, build, and install a new Linux kernel for Slackware and Slack based systems.
Slackware Based Distro should execute this script as root NOT sudo, or during the time mkinird probably it will stop.
On the top of script you just have to edit Kernel versions any time you use it.

example:
```
KERNEL_URL=https://cdn.kernel.org/pub/linux/kernel/v6.x
KERNEL_VERSION=6.0.14
VERSION2=6.0.14
```
SBKS wont remove or upgrade older Linux kernel versions that allready exist in your system.
 NOTE:
 If your old .config is custom kernel for example you are running now a kernel named 6.0.14-rtz 
 Then the VERSION2 only should be:
 ```
KERNEL_URL=https://cdn.kernel.org/pub/linux/kernel/v6.x
KERNEL_VERSION=6.0.14
VERSION2=6.0.14-rtz
```
This script in NOT working for testing kernels (for example 6.2-RC) 
With this script you can always have a second generic kernel that officially Slackware upgrade kernels will not touch it.
We dont need it beacause Pat`s building are always fine, but just in case... 
It is tested to Slackware64 15+ and Slackel
