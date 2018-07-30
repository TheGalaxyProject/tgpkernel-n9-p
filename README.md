# TGPKernel Note 9 (for Android Pie 9)

![TGPKernel Logo](https://github.com/TheGalaxyProject/tgpkernel-n9-p/blob/master/build/logo.png?raw=true)

A Custom Kernel for Samsung Galaxy Note 9

* XDA Note 9 Forum: http://forum.xda-developers.com/showthread.php?t=3910842


Compiled using Google GCC 4.9 Toolchain

* URL: https://github.com/djb77/aarch64-linux-android-4.9

## How to use
Adjust the toolchain path in build.sh and Makefile to match the path on your system. 

Run build.sh with the following options, doesn't matter what order keep and silent are in.

- **./build.sh** will build TGPKernel
- **./build.sh -k** will build TGPKernel and also copy the .img files to the .output folder
- **./build.sh -s** will build TGPKernel but only display warning and errors in the log
- **./build.sh -ks** will do both **-k** and **-s** at the same time

When finished, the new files and logs will be created in the .output directory.

If Java is installed, the .zip file will be signed.


These commands can only be executed by themselves

- **./build.sh 0** will clear the workspace
- **./build.sh 00** will clear CCACHE
- **./build.sh config** will regenerate the stock crownlte config and overwrite the old ones


## Credit and Thanks to the following:
- [Samsung Open Source Release Center](http://opensource.samsung.com) for the Source code (my personal repo [here](https://github.com/djb77/samsung-kernel))
- [Google](https://android.googlesource.com/kernel/common) for AOSP Common Kernel Source
- @osm0sis for [Android Image Kitchen](https://github.com/osm0sis/Android-Image-Kitchen/tree/AIK-Linux) and [anykernel2](https://github.com/osm0sis/AnyKernel2)
- @farovitus, @Eamo5, and @Noxxxious for help and commits
- All the other kernel devs I have picked commits from to form this kernel

