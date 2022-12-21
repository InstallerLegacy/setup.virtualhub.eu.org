 ---
title: "How to install AltairZ80 emulator?"
date: 2022-10-06T19:18:00+05:30
draft: false
featuredImage: "/images/2022/10/07/banner.webp"
featuredImagePreview: "/images/2022/10/07/banner.webp"
tags: ["Emulator", "Executable",]
categories: ["Emulator"]
---

In this tutorial we will install [AltairZ80](https://schorn.ch/altair.html) emulator. The Altair 8800 simulator is part of the SIMH family of simulators. Unlike a real Altair 8800 it features several enhancements:

- Choice of processor (8080 CPU, Z80 CPU or 8086 CPU)
- Optional banked memory (16 banks with 64 Kbyte)
- MMU supporting ROM and memory mapped I/O
- Optional hard drive support for additional storage capacity
- Networking support via TCP/IP for client/server systems
- Support for multiple consoles
- Timer and keyboard generated interrupts
- Various devices for Northstar, Vector Graphic and CompuPro
- Ability to set the clock speed for "real-time" simulation (useful for games)

## Installing

### Linux

{{< admonition>}}
If you have not already installed a Linux distribution, see [our tutorials on how to install Kubuntu](https://setup.virtualhub.eu.org/categories/os/), a beginner-friendly distro.
{{< /admonition>}}

AltairZ80 emulator is available in Kubuntu repositories in `simh` package. It is also available in repositories of many Linux distro I have used. You can install it on Kubuntu and any Ubuntu/Debian based system using the following command:

```bash
sudo apt install simh
```

This will prompt you for your password. Enter it. The `simh` package will install. Now you can run AltairZ80:

```bash
altairz80
```

To exit the emulator, type `exit` and press enter.

#### Manual Installation

If your distribution does not package AlrairZ80, you need to install it manually. You can download an executable from here:

- [AltairZ80 for 64-bit Linux](https://schorn.ch/cpm/zip/beta/altairz80l64.tar.gz) ([Local copy](https://link.storjshare.io/ju77emwkvag7tp7lmndyyk43jlpa/virtualhub-setup%2FAltairZ80%2Faltairz80l64.tar.gz?download=true))

For other systems, you can download an executable from here: <https://schorn.ch/altair.html>

We need to use the command line to install the emulator. Start Konsole. Now use the following command to move to the `Downloads` folder:

```bash
cd Downloads
```

You can run the `ls` command to verify that the file you downloaded is there. Now run the following command to extract the executable:

```bash
tar -xzf altairz80l64.tar.gz
```

Now run the `ls` command again. There will be many file. We need the `altairz80` file.

{{< image src="/images/2022/10/07/AltairZ80-1.webp" alt="Extract AltairZ80 archive" caption="tar -xzf altairz80l64.tar.gz" >}}

Now we will install the executable in `/usr/local/bin` so that we can call it without specifying its path:

```bash
sudo install altairz80 /usr/local/bin/
```

Enter you password when asked to do so.

{{< image src="/images/2022/10/07/AltairZ80-2.webp" alt="Install AltairZ80 executable" caption="sudo install altairz80 /usr/local/bin/" >}}

We have installed AltairZ80. Now you can start it. Just run this command:

```bash
altairz80
```

{{< image src="/images/2022/10/07/AltairZ80-3.webp" alt="AltairZ80" caption="altairz80" >}}

That's it. We installed Altairz80 emulator. Now you can follow the tutorials on [VirtualHub](https://virtualhub.eu.org) which uses this emulator.

To exit the emulator, type `exit` and press enter.

{{< image src="/images/2022/10/07/AltairZ80-4.webp" alt="Exit AltairZ80" caption="exit" >}}

There are also some documentation included in the archive. If you want, you can read them, else you can delete them. Delete the rest of the files. They are not needed.

### Windows

{{< admonition tip>}}
You should use Linux. If you don't know how to install a Linux distro, see [our tutorials on how to install Kubuntu](https://setup.virtualhub.eu.org/categories/os/), a beginner-friendly distro.
{{< /admonition>}}

You can download an archive for windows from [here](https://schorn.ch/cpm/zip/beta/altairz80.zip) ([local copy](https://link.storjshare.io/jvepufvf4yfei4cay4b7wub7hpha/virtualhub-setup%2FAltairZ80%2Faltairz80.zip?download=true)). Now extract the archive. Inside, you will find two `.exe` files. One is for 64 bit and one for 32 bit. Copy the respective file for your system to somewhere and delete the other one. Rename the file to `altairz80.exe`. You do not need to install anything. See the "Windows" section of the respective tutorial on [VirtualHub](https://virtualhub.eu.org) to know how to use it.

There are also some documentation included in the archive. If you want, you can read them, else you can delete them.

## Documentation

The archives also contain the AltairZ80 guide in PDF format. You can also download the same PDF file from here:

- [AltairZ80 Documentation](https://link.storjshare.io/jv2jesw2rhgalxby3owlr3dudptq/virtualhub-setup%2FAltairZ80%2Faltairz80_doc.pdf?download=true)

AltairZ80 is a part of SIMH family of emulators. You can download SIMH documentation from here:

- [SIMH Users’ Guide](http://simh.trailing-edge.com/pdf/simh_doc.pdf) ([Local copy](https://link.storjshare.io/jw2i4gwq4igsmv3mch6ilssgit7a/virtualhub-setup%2FAltairZ80%2Fsimh_doc.pdf?download=true))
- [SIMH FAQ](http://simh.trailing-edge.com/pdf/simh_faq.pdf) ([Local copy](https://link.storjshare.io/jxviezwk4qnsnycu3azyrhgkn7jq/virtualhub-setup%2FAltairZ80%2Fsimh_faq.pdf?download=true))

## Credits

- [AltairZ80 Emulator (© 2022 by Peter Schorn)](https://schorn.ch/altair.html) - [Peter Schorn](mailto:peter.schorn@acm.org)
- [SIMH](http://simh.trailing-edge.com/)

## Video tutorial

Do you want to follow the tutorial by watching a video? We will post a video on our [youtube channel](https://www.youtube.com/@virtualhubsetup) soon.

Archives of this tutorial are available on [Wayback Machine](http://web.archive.org/web/*/https://setup.virtualhub.eu.org/altair-z80/).

