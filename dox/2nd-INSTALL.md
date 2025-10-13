
# INTRO
>
> System is based on one public repo (this repo) and number 
> of **shared private GitHub repos** and one or two client 
> specific repos used to enable specific client's needs.
>

### nomenclature
- ***simbox*** - computer with on which simulation runs
- ***#*** - comment


## Preinstall

### clone ue-siminit repo
- switch to **su** & run these commands
```
apt update && apt upgrade && apt autoremove
apt install tree
apt install git
mkdir /opt/iotech/ramdisk -p
mkdir /opt/iotech/client -p
cd /opt/iotech/client
git clone https://github.com/iotech-systems/ue-siminit.git
```
- **ue-siminit** is now on your filesystem 

### create RAMDISK
- switch to **su** & take these steps
- add these lines to your **crontab file** as **root**
```
crontab -e
# if this is the 1st time crontab run; it will ask you to choose editor - select NANO
# append these lines to the file
@reboot sleep 2 && mkdir /opt/iotech/ramdisk -p || true && mount -o size=1G -t tmpfs SIMRAMDISK /opt/iotech/ramdisk
# USER_ID is your user login & same goes for USER_GROUP
@reboot sleep 4 && chown USER_ID:USER_GROUP /opt/iotech/ramdisk
```



## Install 
- edit: /opt/iotech/client/ue-siminit/install/conf/install-path
- switch to **su** & run these commands
```
cd /opt/iotech/client/ue-siminit/install
./run-1st-as-root
```
