# Information page for "Learning ROS robot programming with Raspberry Pi"

## important notices

### May 26, 2018

Though I have written a recovery method from the disablement of the on-board Wi-Fi device after ``apt upgrade`` in Section 2.1.6, this method is now invalid. Unless I give a solution, please use the following image. 

* http://file.ueda.tech/RPIM_BOOK/ubuntu-16.04-preinstalled-server-armhf+raspi3-upgradable-20171223.img.xz

You can install Ubuntu with this image file and use the Wi-Fi device. However, if you execute ``apt upgrade``, it will disappear from the system.

## ERRATA

|locations|errors|amendments|comments|detectors|
|:--|:--|:--|:--|:--|
|Lines 4 through 7 of Figure 6.12, p.112|pip install ... |sudo pip install ...||Y.A|
