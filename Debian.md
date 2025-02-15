sudo apt edit-sources <br>

_add the following to sources.list for non free repo_ <br>
<br>
deb https://deb.debian.org/debian bullseye main contrib non-free <br> 
deb https://deb.debian.org/debian bullseye-updates main contrib non-free <br> 
deb https://deb.debian.org/debian-security bullseye-security main contrib non-free <br>
_be sure to place a # symbol in front of the default directories so there are no double ups. # turns them into comments so they're ignored_ <br>
<br>
sudo apt update <br>
sudo apt upgrade <br>
<br>
_Then in order to install nvidia drivers_ <br>
<br>
_the following will tell you what type of nvidia card you have_ <br>
sudo apt install nvidia-detect <br>
nvidia-detect <br>

_the following will updatae the kernal_ <br>
sudo apt install linux-headers-$(uname -r) <br>
<br>
_this will install the required driver. remember that it may be different to nvidia-driver depending on what nvidia-detect said_ <br>
sudo apt install nvidia-driver <br>

_the following is a basic reboot command_ <br>
sudo reboot <br>
<br>
_once the system has rebooted the following command will confirm the driver installation_ <br>
nvidia-smi <br>
