# Information page for "Learning ROS robot programming with Raspberry Pi"

* [update information](update_info.md)
* OS images for Raspberry Pi Mouse: https://b.ueda.tech/?post=20180617_raspi_ubuntu

## important notices

### Aug. 9, 2018

Travis CI requires `sudo` when we use `pip`. Please modify `travis_ros_install.bash` as follows.

```
$ head travis_ros_install.bash 
#!/bin/bash -xve

#required packages
sudo pip install catkin_pkg       ###add sudo!!!###
sudo pip install empy             ###add sudo!!!###
sudo pip install pyyaml           ###add sudo!!!###
sudo pip install rospkg           ###add sudo!!!###

#ros install
cd ..
```

### June 15, 2018

I have confirmed that the WiFi problem can be solved with the procedure in https://wiki.ubuntu.com/ARM/RaspberryPi#Wifi .

Please change the URLs in p.22 as shown in [this page](https://gist.github.com/ryuichiueda/f03bbcdd28d4e8742ca7d87032d5626d). 


### June 11, 2016

When we create a ROS package with `catkin_create_pkg`, the format of `package.xml` becomes "Version 2." In this case, we use `exec_depend` instead of `run\depend`.

