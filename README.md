# Qt5 Library Package for OpenWRT

Cross compile the Qt5 Core for OpenWRT.

## Configure Qt Modules and Features

TBA

## How to Compile

OpenWRT compiler is required.

1. Download SDK, for example https://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620n/OpenWrt-SDK-ramips-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2  
2. Extract the SDK  
3. Clone this repo  
4. Put this repo into SDK/packages  
5. Compile by make package/qt5-openwrt-package/compile V=s  
6. Go to sleep and check it in the morning  

## Tested Platform

TBA

## Acknowledgments

* Forked from https://github.com/pawelkn/qt5-openwrt-package  
* Updated by https://github.com/vonger  
* Inspired by http://vonger.cn/?p=14588  
