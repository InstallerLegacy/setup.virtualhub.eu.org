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

AltairZ80 emulator is available in Kubuntu repositories in `simh` package. It is also available in repositories of many Linux distro I have used. But the version included in all distributions are very old and can not run some OS we are going to install on [VirtualHub](https://virtualhub.eu.org). So, we need to install it manually. You can download an executable from here:

- [AltairZ80 for 64-bit Linux](https://schorn.ch/cpm/zip/beta/altairz80l64.gz) ( [Local copy](https://link.storjshare.io/jwfri42zngvnnz6yxuwpjvofyika/virtualhub-setup%2FAltairZ80%2Faltairz80l64.gz?download=true) / [IPFS](https://bafybeigg6myj7trzhvvben33fk3b7exrtjy4foofws44dfgfm72xm4d6fa.ipfs.w3s.link/altairz80l64.gz) )

For other systems, you can download an executable from here: <https://schorn.ch/altair_beta.php>

We need to use the command line to install the emulator. Start Konsole. Now use the following command to move to the `Downloads` folder:

```bash
cd Downloads
```
You can run the `ls` command to verify that the file you downloaded is there. Now run the following command to extract the executable:

```bash
gunzip altairz80l64.gz
```

Now run the `ls` command again. The `.gz` extension should have been removed. This means the file is extracted.

{{< image src="/images/2022/10/07/AltairZ80-1.webp" alt="Extract AltairZ80 archive" caption="gunzip altairz80l64.gz" >}}

Now we will make the file executable. Run the following command to make it executable:

```bash
chmod +x altairz80l64
```

{{< image src="/images/2022/10/07/AltairZ80-2.webp" alt="Make the AltairZ80 file executable" caption="chmod +x altairz80l64" >}}

Now we will place the executable in `/usr/local/bin` so that we can call it without specifying its path:

```bash
sudo mv altairz80l64 /usr/local/bin/altairz80
```

Enter you password when asked to do so.

{{< image src="/images/2022/10/07/AltairZ80-3.webp" alt="Install AltairZ80 executable" caption="sudo mv altairz80l64 /usr/local/bin/altairz80" >}}

We have installed AltairZ80. Now you can start it. Just run this command:

```bash
altairz80
```

{{< image src="/images/2022/10/07/AltairZ80-4.webp" alt="AltairZ80" caption="altairz80" >}}

That's it. We installed Altairz80 emulator. Now you can follow the tutorials on [VirtualHub](https://virtualhub.eu.org) which uses this emulator.

To exit the emulator, type `exit` and press enter.

{{< image src="/images/2022/10/07/AltairZ80-5.webp" alt="Exit AltairZ80" caption="exit" >}}

### Windows

{{< admonition tip>}}
You should use Linux. If you don't know how to install a Linux distro, see [our tutorials on how to install Kubuntu](https://setup.virtualhub.eu.org/categories/os/), a beginner-friendly distro.
{{< /admonition>}}

You can download an archive for windows from [here](https://schorn.ch/cpm/zip/beta/altairz80.zip) ( [local copy](https://link.storjshare.io/ju7vgjnsfdotdbdrinmxfbcfpx5q/virtualhub-setup%2FAltairZ80%2Faltairz80.zip?download=true) / [IPFS](https://bafybeiam5qjbpupbwayegr2rkks5hjcmgpnlc4vnpgs6pooefoslqr27re.ipfs.w3s.link/ipfs/bafybeiam5qjbpupbwayegr2rkks5hjcmgpnlc4vnpgs6pooefoslqr27re/altairz80.zip) ). Now extract the archive. Inside, you will find two `.exe` files. One is for 64 bit and one for 32 bit. Copy the respective file for your system to somewhere and delete the other one. You do not need to install anything. See the "Windows" section of the respective tutorial on [VirtualHub](https://virtualhub.eu.org) to know how to use it.

There are also some documentation included in the archive. If you want, you can read them, else you can delete them.

## Documentation

The linux archive only contains a single executable. It does not include any documentation files. If you want to read the AltairZ80 guide, you can download the Windows archive from [above](#windows). It contains the guide in PDF format. You can also download the same PDF file from here:

- [AltairZ80 Documentation](https://link.storjshare.io/jv2jesw2rhgalxby3owlr3dudptq/virtualhub-setup%2FAltairZ80%2Faltairz80_doc.pdf?download=true) ( [IPFS](https://bafybeidiwqm2uffr2au77rqzgpmcgzcqcssi2xgdkg5m3ibhqk5i2basbe.ipfs.w3s.link/altairz80_doc.pdf) )

AltairZ80 is a part of SIMH family of emulators. You can download SIMH documentation from here:

- [SIMH Users’ Guide](http://simh.trailing-edge.com/pdf/simh_doc.pdf) ( [Local copy](https://link.storjshare.io/jvtg4ghgzfe35l5lfyzhdeuwyzdq/virtualhub-setup%2FAltairZ80%2Fsimh_doc.pdf?download=true) / [IPFS](https://bafybeih3dtpvg5xstjx6rghk3ftyixim4pnvplesjjg23mkfoc4kwyqupi.ipfs.w3s.link/simh_doc.pdf) )
- [SIMH FAQ](http://simh.trailing-edge.com/pdf/simh_faq.pdf) ( [Local copy](https://link.storjshare.io/jxviezwk4qnsnycu3azyrhgkn7jq/virtualhub-setup%2FAltairZ80%2Fsimh_faq.pdf?download=true) / [IPFS](https://bafybeihc6elabrromcaxuj2sjtcacbslnsr4upmloicqc3ipjffr3n6dam.ipfs.w3s.link/simh_faq.pdf) )


## Credits

- [AltairZ80 Emulator (© 2022 by Peter Schorn)](https://schorn.ch/altair.html) - [Peter Schorn](mailto:peter.schorn@acm.org)
- [SIMH](http://simh.trailing-edge.com/)

## Video tutorial

Do you want to follow the tutorial by watching a video? Here it is:

{{< youtube zgzS9w_qaRw >}}

Don't like youtube? You can download the above video from [here](https://link.storjshare.io/jv63w2lpjiuu5ltbm3m4eswkgdaa/virtualhub-setup-videos%2FEmulators%2FHow%20to%20install%20AltairZ80%20emulator.mp4). The video is also available on IPFS. You can download it from [here](https://bafybeiddci3h4uwslnwjejfqngnsutzdg245qns2e474gqi4abo6skulnm.ipfs.w3s.link/How%20to%20install%20AltairZ80%20emulator.mp4).

This tutorial itself is also available on IPFS. You can read this tutorial on IPFS [here](https://setup-virtualhub-eu-org.ipns.dweb.link/altair-z80/). An archive of this tutorial is available [here](http://web.archive.org/web/20221022161813/https://setup.virtualhub.eu.org/altair-z80/) via Wayback Machine.
