---
title: "What to do after installing Kubuntu?"
date: 2022-10-03T12:57:00+05:30
draft: false
featuredImage: "/images/2022/10/03/banner.webp"
featuredImagePreview: "/images/2022/10/03/banner.webp"
tags: ["Kubuntu", "Operating System", "Tweaks"]
categories: ["OS"]
---

In the [last tutorial](/install-kubuntu), we installed Kubuntu 22.04. We need to do some post-installation work before we can start installing different Hypervisors and emulators. So let's start.

{{< admonition >}}
If you have not installed Kubuntu yet, please see [our tutorial](/install-kubuntu) on how to install it. You need an installation media to install Kubuntu. If you do not have installation media, please see [this tutorial](/create-kubuntu-installation-media).
{{< /admonition >}}

There are GUI ways of doing the following things in Kubuntu, but the command line is much more stable. We will use the command line in this tutorial. You need to start Konsole first. Click on the "Start Menu" in the bottom left of the screen then click on Konsole to open it. Kubuntu is much similar to Windows in its desktop layout, so you should be comfortable using it.

## Installing Updates

First of all, we should install the available updates. To fetch the list of updates, run the following command:

```bash
sudo apt update
```

Enter your password when asked.

{{< admonition tip>}}
When you enter your password, nothing will appear on your screen as you enter it, but the password is being entered. This is a common phenomenon in Linux and Unix world.
{{< /admonition >}}

{{< image src="/images/2022/10/03/aptupdate.webp" alt="sudo apt update" caption="sudo apt update">}}

To perform the upgrade, run:

```bash
sudo apt upgrade
```

{{< image src="/images/2022/10/03/aptupgrade.webp" alt="sudo apt upgrade" caption="sudo apt upgrade">}}

Press `Y` and then press enter to start the upgrade.

{{< image src="/images/2022/10/03/upgrading.webp" alt="Upgrading" caption="Upgrading">}}

It will take time to upgrade, depending on your internet speed and the time elapsed since the release of the ISO file you used to install Kubuntu. Don't worry. Every upgrade does not take so long. If you update daily, it should take less than a minute.

After the update is done, you should reboot if there was a kernel upgrade. If you are not sure, reboot anyway.

### Updating Snap packages

Snap packages should update automatically in the background, but if you want them to update now, run this command:

```bash
snap refresh
```

A window will pop up asking for your password. Enter it and click on `OK`.

{{< image src="/images/2022/10/03/password.webp" alt="Password" caption="Enter your password">}}

The snap packages will start to update.

{{< image src="/images/2022/10/03/snaprefresh.webp" alt="snap refresh" caption="snap refresh">}}

It will take some time, depending on your internet speed.

## Installing restricted packages

We installed most of the restricted codecs when we ticked the ["Install third-party software"](/install-kubuntu/#updates-and-other-software). But there are some more packages. Also, we will install Microsoft fonts so that some of the documents look better. To install these, run the following command:

```bash
sudo apt install kubuntu-restricted-extras
```

Enter your password when asked to do so. When asked for confirmation, press `Y` and then press enter. The installation will start. After some time the following screen will open:

{{< image src="/images/2022/10/03/microsoft-font-1.webp" alt="Microsoft Font (1)" caption="Microsoft Font (1)">}}

Press `TAB` key and then press enter. The following screen will open:

{{< image src="/images/2022/10/03/microsoft-font-2.webp" alt="Microsoft Font (2)" caption="Microsoft Font (2)">}}

Press the left arrow key to move to `Yes` then press enter. The installation will continue. It takes a long time to download Microsoft fonts from SourceForge, so sit back and relax.

## Installing Flatpak

Many emulators that we will install come as Flatpak packages. So, we will install Flatpak support on Kubuntu. To do so, run:

```bash
sudo apt install flatpak plasma-discover-backend-flatpak
```

This will install Flatpak and configure Discover for Flatpak.

{{< admonition tip>}}
Discover is the app store for KDE. If you have used the Play Store on Android or App Store on apple products, you should be familiar with the concept. Open it > Search for the app > Install the app with a single click.
{{< /admonition >}}

Now we need to add Flathub repository to Flatpak. To do so, run:

```bash
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Enter your password when asked to do so. After it is done, restart your system. That's it. We enabled Flatpak support.

## Explore the system

Now we have completed the post-installation setup. Explore the plasma desktop and learn new things. You can refer to the User Manuals if you want. To access the User Manuals, start the application called "Help" and choose the required manual from the left sidebar.

{{< image src="/images/2022/10/03/help.webp" alt="Help" caption="Help">}}

## Video tutorial

Do you want to follow the tutorial by watching a video? Here it is:

{{< youtube GxXiRfft-6w >}}

Don't like youtube? You can download the above video from [here](https://link.storjshare.io/jufpdsrfdlu6zxdaf3gslyag2n7a/virtualhub-setup-videos%2FOS%2FWhat%20to%20do%20after%20installing%20Kubuntu.mp4?download=true).

Archives of this tutorial are available on [Wayback Machine](https://web.archive.org/web/*/https://setup.virtualhub.eu.org/kubuntu-post-installation/).
