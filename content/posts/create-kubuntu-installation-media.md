---
title: "How to create a Kubuntu installation media?"
date: 2022-09-30T13:22:00+05:30
draft: false
featuredImage: "/images/2022/09/30/banner.webp"
featuredImagePreview: "/images/2022/09/30/banner.webp"
tags: ["Rufus", "Installation Media", "Preparation"]
categories: ["OS"]
---

As promised, first we will install a beginner-friendly Linux Distribution, Kubuntu. Kubuntu is a very good Linux distribution. It unites Ubuntu with KDE and the fabulous Plasma desktop, bringing a full set of applications. The installation includes productivity, office, email, graphics, photography, and music applications ready to use at startup. If you have used Windows before, you should be comfortable using it.

To install Kubuntu, first, we need to create an installation media pen drive. You need a pen drive with 4 GB or more storage. Everything stored on the pen drive will be deleted, so make sure you have a backup. Plug this pen drive into your system.

## Downloads

### Rufus

We will use Rufus to create the installation media, so let us download it. Go to <https://rufus.ie>. Scroll down a little and download the latest version (At the time of writing, it is 3.20).

{{< image src="/images/2022/09/30/rufus-download.webp" alt="Rufus Download" caption="Rufus Website">}}

### Kubuntu

Now we will download Kubuntu itself. Go to <https://kubuntu.org/getkubuntu> and download the latest LTS release. In this tutorial, we will use Kubuntu 22.04 LTS.

{{< image src="/images/2022/09/30/kubuntu-download.webp" alt="Kubuntu Download" caption="Kubuntu Download">}}

## Installation Media Creation

Now we will write the ISO file to the pen drive. Double-click on Rufus to start it. It will ask whether you want to check for updates.

{{< image src="/images/2022/09/30/rufus-updates.webp" alt="Rufus Updates Prompt" width=468 >}}

Click on `Yes` to allow updates. Now Rufus will start.

{{< image src="/images/2022/09/30/rufus.webp" alt="Rufus Main Window" width=403 >}}

Click on the `Select` button in the Boot selection portion of the window and choose the ISO file you just downloaded. Make sure your pen drive is selected in the device selection. Click on `Start` to start writing the image to the pen drive. The following window will open:

{{< image src="/images/2022/09/30/dd.webp" alt="ISOHybrid image detected" width=542 >}}

Make sure you choose `Write in DD Image mode` and click on `OK`. Rufus will start writing the ISO to the pen drive.

{{< image src="/images/2022/09/30/writing-image.webp" alt="Writing the ISO image" width=490 >}}

It will take a long time to write the image, depending on the write speed of your pen drive. Have patience. After the image is written, eject your pen drive. That's it we created a Kubuntu installation media pen drive. In the [next tutorial](/install-kubuntu), we will use it to install Kubuntu.

## Video tutorial

Do you want to follow the tutorial by watching a video? Here it is:

{{< youtube YgtnF2ZQBk0 >}}

Don't like youtube? You can download the above video from [here](https://link.storjshare.io/s/jwgvrk72blugzyx3rcbvgs7jnx6q/virtualhub-setup-videos/OS/How%20to%20create%20a%20Kubuntu%20installation%20media.mp4?download=true). The video is also available on IPFS. You can download it from [here](https://bafybeidnpq3znhqkjmqkx7ctg2y5msl6meswa2hia3dukeqee3yzwecqy4.ipfs.w3s.link/How%20to%20create%20a%20Kubuntu%20installation%20media.mp4).

This tutorial itself is also available on IPFS. You can read this tutorial on IPFS [here](https://setup-virtualhub-eu-org.ipns.dweb.link/create-kubuntu-installation-media/). An archive of this tutorial is available [here](https://web.archive.org/web/20220930110753/https://setup.virtualhub.eu.org/create-kubuntu-installation-media/) via Wayback Machine.
