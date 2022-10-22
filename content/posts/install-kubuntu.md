---
title: "How to install Kubuntu?"
date: 2022-10-01T10:46:00+05:30
draft: false
featuredImage: "/images/2022/10/01/banner.webp"
featuredImagePreview: "/images/2022/10/01/banner.webp"
tags: ["Kubuntu", "Operating System"]
categories: ["OS"]
---

In the [last tutorial](/create-kubuntu-installation-media), we prepared a Kubuntu installation media. We will use it in this tutorial to install Kubuntu. If you have not prepared the installation media yet, please see the [last tutorial](/create-kubuntu-installation-media).

First, insert the installation media pen drive which you created in the [last tutorial](/create-kubuntu-installation-media) in your system. Then reboot your computer.

As the computer boots, press the function key which opens the system-specific boot menu. F12 is the most common key for bringing up your system’s boot menu, but Escape, F2 and F10 are common alternatives. If you’re unsure, look for a brief message when your system starts – this will often inform you of which key to press to bring up the boot menu. If no such message is shown, check your device documentation. When the boot menu appears, choose to boot from the pen drive.

After the system boots from the pen drive, select "Try or Install Kubuntu" from the list that is shown. Wait for some time as the system boots. You will see the following screen after the system boots properly.

{{< image src="/images/2022/10/01/Kubuntu-Installer-1.webp" alt="Kubuntu Installer (1)" caption="Kubuntu Installer (1)">}}

Click on `Install Kubuntu` to start the installation.

## Keyboard layout

{{< image src="/images/2022/10/01/Kubuntu-Installer-2.webp" alt="Kubuntu Installer (2)" caption="Kubuntu Installer (2)">}}

Choose your desired keyboard layout and click on `Continue`.

## Wireless

{{< image src="/images/2022/10/01/Kubuntu-Installer-3.webp" alt="Kubuntu Installer (3)" caption="Kubuntu Installer (3)">}}

Click on "Connect to this Network" and then connect to your wifi. If you have a wired connection then you can leave this step. Click on `Continue`.

## Updates and other software

{{< image src="/images/2022/10/01/Kubuntu-Installer-4.webp" alt="Kubuntu Installer (4)" caption="Kubuntu Installer (4)">}}

Select "Install third-party software" and "Configure Secure Boot". Enter a password for configuring Secure Boot and write it down somewhere. Click on `Continue`.

## Installation type

{{< image src="/images/2022/10/01/Kubuntu-Installer-5.webp" alt="Kubuntu Installer (5)" caption="Kubuntu Installer (5)">}}

The default should be to dual-boot with Windows. It will resize your Windows partition (C:) to make room for Kubuntu. It should be the best option, but if you want to do something else, you are free to do so. Click on `Install Now`.

It will ask you for confirmation twice. Make sure everything is correct and then click on `Continue`.

## Where are you?

{{< image src="/images/2022/10/01/Kubuntu-Installer-6.webp" alt="Kubuntu Installer (6)" caption="Kubuntu Installer (6)">}}

Select your time zone by clicking on the map. Then click on `Continue`.

## Who are you?

{{< image src="/images/2022/10/01/Kubuntu-Installer-7.webp" alt="Kubuntu Installer (7)" caption="Kubuntu Installer (7)">}}

Enter your Name, Username and password. You can also change your computer's name to anything you like. Your computer will be visible on your local network using that name. Click on `Continue`. The installation will start.

## Installation

{{< image src="/images/2022/10/01/Kubuntu-Installer-8.webp" alt="Kubuntu Installer (8)" caption="Kubuntu Installer (8)">}}

The installation will take a long time depending on the read and write speed of your pen drive and hard disk. So, sit back and relax.

After your installation is over, click on `Reboot`. Remove the pen drive when asked to do so. Your system should reboot into a blue-colored screen called "Perform MOK management" or something similar. If Windows starts instead of all this, reboot again and press the boot menu key you pressed last time. Choose Ubuntu from the list. The "Perform MOK management" screen should open.

## Perform MOK management

{{< image src="/images/2022/10/01/mok-1.webp" alt="MOK Management (1)" caption="MOK Management (1)">}}

Choose "Enroll MOK key".

{{< image src="/images/2022/10/01/mok-2.webp" alt="MOK Management (2)" caption="MOK Management (2)">}}

Then choose `Continue`.

{{< image src="/images/2022/10/01/mok-3.webp" alt="MOK Management (3)" caption="MOK Management (3)">}}

Then choose `Yes`.

{{< image src="/images/2022/10/01/mok-4.webp" alt="MOK Management (4)" caption="MOK Management (4)">}}

Enter the secure boot configuration password you set earlier, then press enter.

{{< admonition tip>}}
When you enter the secure boot configuration password, nothing will appear on your screen as you enter it, but the password is being entered. This is a common phenomenon in Linux and Unix world.
{{< /admonition >}}

{{< image src="/images/2022/10/01/mok-5.webp" alt="MOK Management (5)" caption="MOK Management (5)">}}

Choose "Reboot" at last. After reboot, Kubuntu should start. If Windows starts instead, reboot again and press the boot menu key and choose Kubuntu. To make Kubuntu start and ask which OS you want to boot, you need to change your boot order. Refer to your device documentation to find how to do so.

After Kubuntu starts, log in using your password. See the [next tutorial](/kubuntu-post-installation) to learn what to do after installing Kubuntu.

## Video tutorial

Do you want to follow the tutorial by watching a video? Here it is:

{{< youtube hM27bdsNYeQ >}}

Don't like youtube? You can download the above video from [here](https://link.storjshare.io/jxuwkw6v7a3fdckqm2x4g4gajfwa/virtualhub-setup-videos%2FOS%2FHow%20to%20install%20Kubuntu%2022.04.mp4?download=true). The video is also available on IPFS. You can download it from [here](https://bafybeih7fgtaft7ks77ytyey2fhnqz4o2sdt3aloow2w5j6dh275ku5lre.ipfs.w3s.link/How%20to%20install%20Kubuntu%2022.04.mp4).

This tutorial itself is also available on IPFS. You can read this tutorial on IPFS [here](https://setup-virtualhub-eu-org.ipns.dweb.link/install-kubuntu/). An archive of this tutorial is available [here](https://web.archive.org/web/20221001100400/https://setup.virtualhub.eu.org/install-kubuntu/) via Wayback Machine.
