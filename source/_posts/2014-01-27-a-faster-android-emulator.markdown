---
layout: post
title: "A Faster Android Emulator"
date: 2014-01-27 19:30:46 +0100
comments: true
categories: [Android, Geny Motion, Mac, IntelliJ]
---
Anyone who has done Android development will know that the standard emulator is very slow to startup.
I have recently discovered a much speedier alternative!

##Speeding Things Up
[Geny Motion](http://www.genymotion.com/) is an alternative emulator which is much faster.
However it is a paid product.
They offer a free personal version which I am using.

##Mac Setup
1. [Create an account at Geny Motion](https://cloud.genymotion.com/page/customer/login/)
2. [Install Virtual Box](https://www.virtualbox.org/wiki/Downloads)
3. [Install Geny Motion](https://cloud.genymotion.com/page/launchpad/download/)
4. Optional [Install an IDE Plugin](https://cloud.genymotion.com/page/launchpad/download/) (I use the IntelliJ plugin)
5. Startup Geny Motion and add the device you want
6. Press play on that device
7. Run your Android code (In my IntelliJ run configuration I have set the target device to `Show chooser dialog`)

If you want to use Geny Motion on Windows you can skip step 2 as that is included in the installer.