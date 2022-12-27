---
title: "How to install VirtualBox?"
date: 2022-12-27T10:18:00+05:30
draft: false
featuredImage: "/images/2022/12/27/VirtualBox-6.webp"
featuredImagePreview: "/images/2022/12/27/banner.webp"
tags: ["Hypervisor", "Developer Repo"]
categories: ["Hypervisor"]
---

VirtualBox is a powerful x86 and AMD64/Intel64 virtualization product for enterprise as well as home use. Not only is VirtualBox an extremely feature rich, high performance product for enterprise customers, it is also the only professional solution that is freely available as Open Source Software under the terms of the GNU General Public License (GPL) version 3.

Presently, VirtualBox runs on Windows, Linux, macOS, and Solaris hosts and supports a large number of guest operating systems including but not limited to Windows (NT 4.0, 2000, XP, Server 2003, Vista, Windows 7, Windows 8, Windows 10), DOS/Windows 3.x, Linux (2.4, 2.6, 3.x and 4.x), Solaris and OpenSolaris, OS/2, and OpenBSD.

VirtualBox is being actively developed with frequent releases and has an ever growing list of features, supported guest operating systems and platforms it runs on. VirtualBox is a community effort backed by a dedicated company: everyone is encouraged to contribute while Oracle ensures the product always meets professional quality criteria.

## Installing

### Linux

{{< admonition>}}
If you have not already installed a Linux distribution, see [our tutorials on how to install Kubuntu](https://setup.virtualhub.eu.org/categories/os/), a beginner-friendly distro.
{{< /admonition>}}

In this tutorial we will see how to install VirtualBox on Kubuntu 22.04. It is also valid for any Ubuntu 22.04 based distro. If you use any other distro, refer to the [VirtualBox manual](https://www.virtualbox.org/manual/ch02.html#install-linux-host) and [VirtualBox download page](https://www.virtualbox.org/wiki/Linux_Downloads) for instructions on how to install it on your specific distro.

VirtualBox is available in Kubuntu repositories. It is also available in repositories of many Linux distro I have used. But most of the times, the repos contain old version of VirtualBox. So, we will install VirtualBox from Oracle’s repository. First, add the key for the repository. You can download and add the key using this single command:

```bash
wget -O- https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --dearmor --yes --output /usr/share/keyrings/oracle-virtualbox-2016.gpg
```

{{< image src="/images/2022/12/27/VirtualBox-1.webp" alt="Add Oracle's key" caption="Add Oracle's key" >}}

Now we will add Oracle's repository. Run the following command:

```bash
sudo nano /etc/apt/sources.list.d/virtualbox.list
```

Copy the following:

```
deb [arch=amd64 signed-by=/usr/share/keyrings/oracle-virtualbox-2016.gpg] https://download.virtualbox.org/virtualbox/debian jammy contrib
```

Press `Shift`+`Ctrl`+`V` to paste it. Then press `Ctrl`+`O` to save and `Ctrl`+`X` to close the file.

{{< image src="/images/2022/12/27/VirtualBox-2.webp" alt="Add Oracle's repository" caption="Add Oracle's repository" >}}

{{< admonition tip >}}
If you are using any other LTS version of Ubuntu except 22.04 or if your distro is based on any other LTS version of ubuntu, replace `jammy` with the codename of your version. If you are using a non-LTS version, replace the `jammy` with the codename of the last LTS version. Oracle used to provide repositories for non-LTS version, but since 21.10, it stopped doing so.
{{< /admonition >}}

Update the package index:

```bash
sudo apt update
```

{{< image src="/images/2022/12/27/VirtualBox-3.webp" alt="Update the package index" caption="sudo apt update" >}}

Now install VirtualBox:

```bash
sudo apt install virtualbox-7.0
```

{{< admonition tip >}}
You can replace `virtualbox-7.0` with other version when it is released. To see a list of versions supported type `sudo apt install virtualbox` and press the TAB key a few times. Do not install `virtualbox` package as it is the old version from Ubuntu repos.
{{< /admonition >}}

{{< image src="/images/2022/12/27/VirtualBox-4.webp" alt="Install VirtualBox" caption="sudo apt install virtualbox-7.0" >}}

Add yourself to the `vboxusers` group:

```bash
sudo usermod -a -G vboxusers username
```

Replace `username` with your account username. Now, logout and login back.

{{< image src="/images/2022/12/27/VirtualBox-5.webp" alt="Add user to vboxusers group" caption="sudo usermod -a -G vboxusers legacyinstaller" >}}

VirtualBox is installed. You can start using it.

{{< image src="/images/2022/12/27/VirtualBox-6.webp" alt="VirtualBox" caption="VirtualBox" >}}

### Windows

{{< admonition tip>}}
You should use Linux. If you don't know how to install a Linux distro, see [our tutorials on how to install Kubuntu](https://setup.virtualhub.eu.org/categories/os/), a beginner-friendly distro.
{{< /admonition>}}

If you are on Windows, refer to the [VirtualBox manual](https://www.virtualbox.org/manual/ch02.html#installation_windows) and [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads) for instructions on how to install it.

## Oracle VM VirtualBox Extension Pack

While VirtualBox is free and open source and hence anyone can use it for free, some features for VirtualBox are released as "Oracle VM VirtualBox Extension Pack". It is not FOSS but is free for non-commercial use. If you want to use it commercially, you need to get a license from Oracle. To install it, download it from [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads) ([Local copy](https://link.storjshare.io/juq524kfigvomkjmjez46dptiqoq/virtualhub-setup%2FVirtualBox%2FOracle_VM_VirtualBox_Extension_Pack-7.0.4.vbox-extpack?download=true)).

Open VirtualBox, then click on `File` > `Tools` > `Extension Pack Manager`.

{{< image src="/images/2022/12/27/VirtualBox-7.webp" alt="Extension Manager" caption="Extension Manager" >}}

Now click on `Install` and choose the extension pack you just downloaded.

{{< image src="/images/2022/12/27/VirtualBox-8.webp" alt="Extension Pack" width=513 >}}

Click on `Install`.

{{< image src="/images/2022/12/27/VirtualBox-9.webp" alt="License" width=620 >}}

Scroll down the License and click on `I Agree`.

Give your password when asked to do so. The installation will start and then complete. That's it.

To go back to the Welcome screen, click on the menu beside the `Tools` in the sidebar and click on `Welcome`.

## Documentation

If you want to read the VirtualBox manual, you can access it by clicking on `Help` > `Contents...` in VirtualBox. You can also read it in you browser [here](https://www.virtualbox.org/manual/). You can download a PDF copy of the manual from [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads) ([Local copy](https://link.storjshare.io/jwmltyhm3n3jfyvk4eq7oivryheq/virtualhub-setup%2FVirtualBox%2FVirtualBox%20UserManual.pdf?download=true)).

## Credits

- [VirtualBox](https://www.virtualbox.org/)

## Video tutorial

Do you want to follow the tutorial by watching a video? We will post a video on our [youtube channel](https://www.youtube.com/@virtualhubsetup) soon.

Archives of this tutorial are available on [Wayback Machine](https://web.archive.org/web/*/https://setup.virtualhub.eu.org/virtualbox/).

