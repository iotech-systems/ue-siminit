
# SYSTEM SETUP

> ## Overview
> _**iotech.systems'**_ simulation software is build to run on **ubuntu 25.04** -
> kernel 6.14 with NTSync driver.
> Simulation's backbone is the use of RAMDISK to pass data from **UE5 Actors** to external **actor drivers**
> 
> [kernel 6.14](https://www.linuxjournal.com/content/linux-kernel-614-leap-forward-intel-and-amd-cpu-support)
> 



> ## block text header
> some more text goes here
> adfasdfasdfasfas
> asdfa;lkj askdfasdfk
> asd;kajdf;aksldfj
> 

## [ Create RAMDISK ]
There are two ways to do this:
1. under root cronjob
2. @reboot sleep 4 && mount -o size=128M -t tmpfs SIMRAMDISK /opt/iotech/ramdisk && chown erik:erik /opt/iotech/ramdisk
3. 

> **[ cronjob text ]**
> 
> linux user: erik
> 
> 