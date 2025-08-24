
# SYSTEM SETUP

> ## black header
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
