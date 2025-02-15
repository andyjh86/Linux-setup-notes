sudo apt edit-sources

_add the following to sources.list for non free repo_

deb https://deb.debian.org/debian bullseye main contrib non-free 
deb https://deb.debian.org/debian bullseye-updates main contrib non-free 
deb https://deb.debian.org/debian-security bullseye-security main contrib non-free
_be sure to place a # symbol in front of the default directories so there are no double ups. # turns them into comments so they're ignored_

sudo apt update

sudo apt upgrade

_Then in order to install nvidia drivers_

_the following will tell you what type of nvidia card you have_
sudo apt install nvidia-detect
nvidia-detect

_the following will updatae the kernal_
sudo apt install linux-headers-$(uname -r)

_this will install the required driver. remember that it may be different to nvidia-driver depending on what nvidia-detect said_
sudo apt install nvidia-driver 

_the following is a basic reboot command_
sudo reboot

_once the system has rebooted the following command will confirm the driver installation_
nvidia-smi
