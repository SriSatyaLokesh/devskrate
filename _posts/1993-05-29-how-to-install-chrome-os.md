---
layout: post
title: "Install Chrome OS in a PC"
author: nikhil
category: [tutorial]
image: assets/img/chromeos/install-chrome-os.jpg
optimized_image: assets/img/chromeos/install-chrome-os.jpg
tags: [chrome os]
---

There has been many people searching for the installation of Chrome OS on a old PC or a laptop. So, today we're gonna guide you how to install full chrome OS with access to Android from within Chrome OS on an old laptop or an old PC and this isn't using Chromium OS, Cloud OS or Fade OS this is Chrome OS that you can install on pretty much any Intel based PC.

This is full chrome OS for your laptop or your desktop we also have access to Android and the Google Play Store and you can install Linux apps just like you can with most of the newer Chromebooks out there this is actually really easy to install and use.

I'll give you a quick rundown first thing you're gonna need is a USB Drive 16 gigabytes or larger what we're gonna do is install Linux Mint on this USB Drive so you can run it live we're also gonna transfer our Chrome OS installation files to that USB.

Basically what we're gonna do is start up Linux Mint running live from the USB and then install Chrome OS we'll wipe the internal drive of the PC we're going to be installing this on so if you have Windows installed on your PC and you use it every day don't go doing this but if you have an extra laptop or an old desktop laying around you could definitely try installing and use Chrome OS.

I'm going to be using a separate Windows 10 PC to get my USB drive set up but you could always do this on Linux or Mac some of the applications we're going to use will be different on those operating systems but if you're ready to get Chrome OS installed on your laptop or PC let's go ahead and get started all right so let's go ahead and download everything we need we're gonna get this image set up on a USB Drive.

For all this process, we're going to download five files. They're:

- **Linux Mint**
- **Rufus**
- **Brunch Files**
- **Install.sh File**
- **Chrome OS File**

The first thing you'll need is that USB Drive we do recommend at least the 16 gigabyte Drive

#### Downloading Required Files:

**1.** We need to do is download Linux Mint from [here](https://www.linuxmint.com/download.php). and we're just gonna use this as a live USB so we can install Chrome OS using this operating system we're gonna run this all from the USB. Download the appropriate version ie., either 32 bit or 64 bit.

<img src="{{ site.baseurl }}/assets/img/chromeos/linux-mint.jpg" alt="Linux Mint" title="Linux Mint">

**2.** Then download [Rufus](https://rufus.ie/) that allows us to flash that image to a USB Drive.

<img src="{{ site.baseurl }}/assets/img/chromeos/rufus.jpg" alt="Rufus" title="Rufus">

**3.** Now, download the latest version of [Brunch](https://github.com/sebanc/brunch/releases) from GitHub. As of now the latest version is 4.19.

<img src="{{ site.baseurl }}/assets/img/chromeos/brunch.jpg" alt="Brunch" title="Brunch">

**4.** Now we actually need to get the Chrome OS image and from this [link](https://cros-updates-serving.appspot.com/) you're gonna find **Rammus** in the page using Find in page(**Ctrl+F**) and **download the latest recovery build and extract it**. As of this post, it is 80, but it could be higher. This this the largest file you're going to download and it's going to be around 1.2 GB.

<img src="{{ site.baseurl }}/assets/img/chromeos/chrome-os-image.jpg" alt="Chrome OS Image" title="Chrome OS Image">

**5.** The final thing we'll need is the install.sh file. For this you need to go to this [page](https://raw.githubusercontent.com/shrikant2002/ChromeOS/master/install.sh) and right click and save it as install.sh.

<img src="{{ site.baseurl }}/assets/img/chromeos/install-sh.jpg" alt="Install Sh" title="Install Sh">

#### Getting ready with the bootable drive:

Now place all of the downloaded files on to a single directory or on to your desktop.

All the files you'll be having are Linux Mint, Rufus, Brunch, Chrome OS Image and install.sh.

First thing we need to do is flash our drive with Linux man we're gonna start up Rufus from within this application we need to make sure that we have our USB drive chosen just make sure it is the correct USB.

We're gonna navigate to where we have the Linux Mint image and finally we'll click start this is gonna flash Linux Mint to that USB drive so we can boot it up live on our PC you get a couple warnings Yes and we want to write this in an ISO image mode click OK all the data on the USB Drive will be destroyed. We're now done with flashing the Linux Mint to our USB Drive.

<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/rufus-1.jpg" width="500">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/rufus-2.jpg" width="500">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/rufus-3.jpg" width="500">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/rufus-4.jpg" width="500">

Now it's time to get the other files we downloaded. Create a folder called Chrome OS and move the install.sh file that we've downloaded inside of this folder. Now extract both the files Brunch and Chrome OS image and move all the files from both of them into the Chrome OS folder you've created. Then move the Chrome OS folder into the USB Drive.

<img src="{{ site.baseurl }}/assets/img/chromeos/chrome-os-folder.jpg" alt="Chrome OS Folder" title="Chrome OS Folder">

Now, finally your bootable drive is ready.

#### Installation:

1. Firstly, go to your machine BIOS menu(ie., by clicking either **Esc**, **F2**, **F9**, **F10**, or **F12** while turning on the machine) and **Disable Secure Boot** and **Boot Option** to **UEFI**.

2. Then plug in your bootable USB and enter in to the boot menu and click on the USB Drive.
3. After that select the Linux Mint option to run it live from the USB Drive.

<img src="{{ site.baseurl }}/assets/img/chromeos/select-linux-mint.jpg" alt="Select Linux Mint" title="Select Linux Mint">

4. Once you have selected Linux Mint, you'll be directed to the Desktop of Linux Mint.
5. Make sure you're online while you're using Linux Mint.
6. Then go to the Chrome OS folder we've created in the File Explorer.

7. Then right click and open terminal in Chrome OS directory.

<img src="{{ site.baseurl }}/assets/img/chromeos/open-terminal.jpg" alt="Open Terminal" title="Open Terminal">

8. Now, in terminal run the command `sudo sh install.sh`. In this step it will download some dependences, that's why you need to be online.

<img src="{{ site.baseurl }}/assets/img/chromeos/sudo-install.jpg" alt="Sudo Install" title="Sudo Install">

9. Now we're going to install the Chrome OS and make this a strictly Chromebook. To do so, type **Yes**.

<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/type-yes.jpg" alt="Type Yes" title="Type Yes">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/yes-typed.jpg" alt="Yes Typed" title="Yes Typed">

10. It will take around 5-10 minutes depending on your internet connection.
    <img src="{{ site.baseurl }}/assets/img/chromeos/os-installed.jpg">
11. Once the process is done, you can either type `sudo reboot` or go to the menu and select **Restart** and remove the USB Drive.

<img src="{{ site.baseurl }}/assets/img/chromeos/restart.jpg" alt="Restart" title="Restart">

Then your pc will be booted with Chrome OS and follow the instructions on the screen to setup the device.

<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/chrome-boot-1.jpg" width="300">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/chrome-boot-2.jpg" width="300">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/chrome-boot-3.jpg" width="300">
<img style="display: inline; margin: 0 5px;" src="{{ site.baseurl }}/assets/img/chromeos/chrome-boot-4.jpg" width="300">

For more detailed procedure of installation, go through the video by [Kedar Nimbalkar](https://www.youtube.com/channel/UCjQ-YHwNTbUQLVzZQFjsDsQ)

<iframe width="480" height="235" src="https://www.youtube.com/embed/4gZYV0RWJQ8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

By the by subscribe to Kedar Nimbalkar for cool videos on operting systems like triple booting a system.  
Content and Image credits: [Kedar Nimbalkar](https://www.youtube.com/channel/UCjQ-YHwNTbUQLVzZQFjsDsQ)
