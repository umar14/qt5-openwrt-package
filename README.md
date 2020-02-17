# Qt5 Library Package for OpenWRT

Cross compile the Qt5 Core library for OpenWRT MIPS platform.

## Configure Qt Modules and Features

TBA

## How to Compile

OpenWRT compiler is required.

1. Download SDK, for example https://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620n/OpenWrt-SDK-ramips-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2  
2. Extract the SDK  
3. Clone this repo  
4. Put this repo into SDK/package  
5. Install dependencies by  

```bash
sudo apt install libncurses-dev zlib1g-dev gawk subversion
```

6. Compile by  

```bash
make package/qt5-openwrt-package/compile V=s  
```

7. It will take a long time to build  
8. You can find compiled ipk files in SDK/bin/  

## Install the Compiled Library to Target Device

1. Copy compiled ipk files to the target device by scp  
2. Install ipk files by  

```bash
opkg install qt5-core_5.11-3_ramips_24kec.ipk
opkg install qt5-network_5.11-3_ramips_24kec.ipk

```

## Tested Platform

TBA

## Acknowledgments

* Forked from https://github.com/pawelkn/qt5-openwrt-package  
* Updated by https://github.com/vonger  
* Inspired by http://vonger.cn/?p=14588  
