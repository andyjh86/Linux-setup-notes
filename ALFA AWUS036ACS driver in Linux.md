_make sure the kernal is up to datae_ <br>
sudo apt-get install linux-headers-$(uname -r) <br>
<br>
_make sure root directory is mounted_ <br>
cd / <br>
<br>
_check the usb adapter is available_ <br>
lsusb <br>
<br>
_clone the github repo_ <br>
git clone https://github.com/aircrack-ng/rtl8812au.git <br>
<br>
_build the source via make_ <br>
sudo make<br>
<br>
_install the make file_ <br>
sudo make install <br>
<br>
_check the adapter has been installed_ <br>
iwconfig <br>
