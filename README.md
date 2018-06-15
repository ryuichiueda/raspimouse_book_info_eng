# Information page for "Learning ROS robot programming with Raspberry Pi"

## important notices

### June 15, 2018

I have confirmed that the WiFi problem can be solved with the procedure in https://wiki.ubuntu.com/ARM/RaspberryPi#Wifi_firmware .

Please change the URLs in p.22 as follows:

* bin file: 
    * old: https://github.com/RPi-Distro/firmware-nonfree/raw/master/brcm80211/brcm/brcmfmac43430-sdio.bin
    * new: https://github.com/RPi-Distro/firmware-nonfree/raw/master/brcm/brcmfmac43430-sdio.bin
* txt file: 
    * old: https://github.com/RPi-Distro/firmware-nonfree/raw/master/brcm80211/brcm/brcmfmac43430-sdio.txt
    * new: https://github.com/RPi-Distro/firmware-nonfree/raw/master/brcm/brcmfmac43430-sdio.txt

### June 11, 2016

When we create a ROS package with `catkin_create_pkg`, the format of `package.xml` becomes "Version 2." In this case, we use `exec_depend` instead of `run\depend`.

### May 26, 2018

Though I have written a recovery method from the disablement of the on-board Wi-Fi device after ``apt upgrade`` in Section 2.1.6, this method is now invalid. Unless I give a solution, please use the following image. 

* http://file.ueda.tech/RPIM_BOOK/ubuntu-16.04-preinstalled-server-armhf+raspi3-upgradable-20171223.img.xz

You can install Ubuntu with this image file and use the Wi-Fi device. However, if you execute ``apt upgrade``, it will disappear from the system.

## ERRATA

|locations|errors|amendments|comments|detectors|
|:--|:--|:--|:--|:--|
|Lines 4 through 7 of Figure 6.12, p.112|pip install ... |sudo pip install ...||Y.A|
