# SBKS  
### (Slack-Build-Kernel-Script) 
It use yad dialogs, so yad required (install it from SBo)

SBKS is a bash script for auto download, build, and install a second (backup) Linux kernel for Slackware and Slack based systems.
Slackware Based Distros should execute this script as root ONLY, NOT sudo ./SBKS else  mkinitrd probably will fail and SBKS will stop.

Past versions was using zenity, but I found yad more stable and better working in a Slackware system...

### Install 
First install zenity from SlackBuild.org 
Use sbopkg or slpkg or whatever you like.

Then:

```
su -l or sudo -i
wget -P /usr/local/bin/ https://raw.githubusercontent.com/rizitis/SBKS/main/SBKS
chmod +x /usr/local/bin/SBKS
```


### Run SBKS 
```
su -l or sudo -i 
SBKS 
```

Everything else you will find it in the script at yad dialogs.
A 5 minutes video is here how to install and run SBKS

[![SBKS](https://github.com/rizitis/SBKS/raw/main/Screenshot%20from%202023-02-03%2017-16-55.png)](https://www.youtube.com/watch?v=PfLugpULA-8)



### Info
SBKS wont remove or upgrade older Linux kernel versions that allready existed in your system.
 In case your old .config is a custom kernel, for example if you are running now a kernel builded by you, named 6.0.14-rtz (uname -r will show you)
 Then on the VERSION2 dialog ONLY you should write:
```
6.1.8-rtz
```
If for example the Kernel you want to build is 6.1.8...
AND you dont have custom kernel version, or you are using officially Slackware Kernel, then just write again on dialog box the kernel version you wish to build. 
```
6.1.8
```

With this script you can always have a second generic kernel that officially Slackware upgrade kernels will not touch it.
We dont need SBKS but only if we want a second or a third... kernel in our system. In other words, Slackware kernels are always fine, but just in case... 
It is tested to Slackware64 15+ and Slackel

### NOTE: 
This script its NOT working for testing kernels (for example 6.2-RC) 
For testing kernels use SBKS-RC (yad not needed for this)
(https://github.com/rizitis/SBKS/tree/SBKS-RC)
