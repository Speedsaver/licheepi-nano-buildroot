Before building, install these Ubuntu dependencies:
```
sudo apt install -y chrpath gawk texinfo libsdl1.2-dev whiptail diffstat cpio libssl-dev swig fakeroot devscripts python3-dev python3-distutils
```
Clone this repo

Ensure build scripts are executable:
```
chmod a+x licheepi-nano-buildroot/board/licheepi_nano/*.sh
```

Download the latest Buildroot, cd into the top level directory and run
```
BR2_EXTERNAL=/path/to/licheepi-nano-buildroot make licheepi_nano_defconfig
```
Customise if required
```
make menuconfig
```
```
make
```

