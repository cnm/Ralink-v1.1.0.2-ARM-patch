Intro
=====

This repo contains a patch for the ralink rt2501 kernel module. The patch corrects warnings when compiling the module for ARM processors.

``Please note that this has not been fully tested.``

It also contains another patch which will add Lalith's code to the driver.

Applying the patch
==================

Pull the driver from git://github.com/joninvski/USB_Wifi_RT2501_TS-7500.git::

    git clone git://github.com/joninvski/USB_Wifi_RT2501_TS-7500.git

cd onto the USB_Wifi_RT2501_TS-7500 folder and use git apply to patch the driver::

    git apply -p1 ralink_module_v1.1.0.2_arm_kernel_2.6.24.patch

Alternatively, you can download it from ftp://ftp.embeddedarm.com/ts-arm-sbc/ts-7500-linux/sources/wifi-g-usb-2_rt2501usb-sources.tar.gz (provided it is the same version) and apply the patch using patch::

    patch -p1 < ralink_module_v1.1.0.2_arm_kernel_2.6.24.patch
