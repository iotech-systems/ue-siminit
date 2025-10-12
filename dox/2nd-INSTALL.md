
# INTRO
>
> System is based on one public repo (this repo) and number 
> of **shared private GitHub repos** and one or two client 
> specific repos used to enable specific client's needs.
>

### nomenclature
- ***simbox*** - computer with on which simulation runs


## Preinstall
- switch to **su** & run these commands
```
apt update && apt upgrade && apt autoremove
apt install git
mkdir /opt/iotech/client -p
cd /opt/iotech/client
git clone https://github.com/iotech-systems/ue-siminit.git
```
- **ue-siminit** is not on your filesystem 


## Install 
- switch to **su** & run these commands
```
cd /opt/iotech/client/ue-siminit/install
./run-1st-as-root
```
