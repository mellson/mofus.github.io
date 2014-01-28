---
layout: post
title: "A Faster Android Emulator"
date: 2014-01-27 19:30:46 +0100
comments: true
categories: [Android, Genymotion, Mac, IntelliJ]
---
Anyone who has done Android development will know that the standard emulator (Android Virtual Device Manager) is very slow to startup.
Luckily there is a much speedier alternative!

##Speeding Things Up
[Genymotion](http://www.genymotion.com/) is an alternative emulator which is much faster.
However it is a paid product.
They offer a free personal version which I am using.

###Initial Setup (Mac)
1. [Install Virtual Box](https://www.virtualbox.org/wiki/Downloads)
2. [Create an account at Genymotion](https://cloud.genymotion.com/page/customer/login/)
3. [Install Genymotion](https://cloud.genymotion.com/page/launchpad/download/)
4. Optional [Install an IDE Plugin](https://cloud.genymotion.com/page/launchpad/download/) (I use the IntelliJ plugin)
5. Startup Genymotion and add the device you want
6. Press play on that device
7. Run your Android code (In my IntelliJ run configuration I have set the target device to `Show chooser dialog`)

If you want to use Genymotion on Windows you can skip step 1 as that is included in the installer.

###Everyday usage
The above is for the initial setup of Genymotion.
After the first setup it gets much easier to use the emulator.
Just follow these three steps.

1. Startup Genymotion
2. Press play on your virtual device
3. Run your Android code

##Benchmark
Let us see how much faster Genymotion is compared to the standard emulator.
We will approach this in a very, *ahem*, scientific benchmark of the two emulators using a timer on my smartphone.
Before you can run your Android emulator you need to prepare it.
Let us test how long it takes to do just that.

###Installing the virtual devices
Both emulators is installing a virtual Nexus 4 device from scratch.
I open the emulator press start on my timer and ask them to startup the device.
When the virtual device hits the desktop I stop the clock.

* Cold boot of the normal emulator with a Nexus 4 virtual device - **211 seconds**
* Cold boot of Genymotion with a Nexus 4 virtual device - **14 seconds**

Over 3 minutes saved here alone.

###Running the virtual devices
After the initial setup you still need to boot up your virtual device every time you need it.
So lets us test how a normal start of the emulators fare against each other.

* Boot of the normal emulator with a Nexus 4 virtual device - **62 seconds**
* Boot of Genymotion with a Nexus 4 virtual device - **9 seconds**

Keep in mind that when you are developing you don't need to shutdown the emulator between runs.

*The test computer is a MacBook Pro, 2,6 GHz i7, 16GB RAM and SSD running os 10.9.1.*