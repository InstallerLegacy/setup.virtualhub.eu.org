 ---
title: "How to install AltairZ80 emulator?"
date: 2022-10-06T19:18:00+05:30
draft: false
featuredImage: "/images/2022/10/07/banner.webp"
featuredImagePreview: "/images/2022/10/07/banner.webp"
tags: ["Emulator", "Source",]
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

AltairZ80 emulator is not available in Kubuntu repositories. It is also not available in repositories of any Linux distro I have used. So, we need to install it manually. You can download an executable from here:

- [AltairZ80 for 64-bit Linux](https://schorn.ch/cpm/zip/beta/altairz80l64.gz) ( [Local copy](https://link.storjshare.io/jwfri42zngvnnz6yxuwpjvofyika/virtualhub-setup%2FAltairZ80%2Faltairz80l64.gz?download=true) / [IPFS](https://dweb.link/ipfs/bafkreifslgft4pe3u5vt25rj5las5dofswtbx367pslkjed5o6vveyvnlq) )

For other systems, you can download an executable from here: <https://schorn.ch/altair_beta.php>

Now run the following command to extract the executable:

```bash
gunzip altairz80l64.gz
```

{{< image src="/images/2022/10/07/AltairZ80-1.webp" alt="Extract AltairZ80 archive" caption="gunzip altairz80l64.gz" >}}

Now we will place the executable in `/usr/local/bin` so that we can call it without specifying its path:

```bash
sudo cp altairz80l64 /usr/local/bin/altairz80
```

{{< image src="/images/2022/10/07/AltairZ80-2.webp" alt="Install AltairZ80 executable" caption="sudo cp altairz80l64 /usr/local/bin/altairz80" >}}


Enter you password when asked to do so. Now you can run AltairZ80. Just run this command:

```bash
altairz80
```

{{< image src="/images/2022/10/07/AltairZ80-3.webp" alt="AltairZ80" caption="altairz80" >}}

That's it. We installed Altairz80 emulator. Now you can follow the tutorials on [VirtualHub](https://virtualhub.eu.org) which uses this emulator.

### Windows

{{< admonition tip>}}
You should use Linux. If you don't know how to install a Linux distro, see [our tutorials on how to install Kubuntu](https://setup.virtualhub.eu.org/categories/os/), a beginner-friendly distro.
{{< /admonition>}}

You do not need to install anything for following the tutorials which use the AltairZ80 emulator. All the archives you download have an executable for Windows and a batch file. Run the batch file and AltairZ80 will start with the OS you wanted to install on it.

## Documentation

You can download the AltairZ80 guide from here:

- [AltairZ80 Documentation](https://link.storjshare.io/jv2jesw2rhgalxby3owlr3dudptq/virtualhub-setup%2FAltairZ80%2Faltairz80_doc.pdf?download=true) ( [IPFS](https://dweb.link/ipfs/bafkreiggumjovndpcubxzeseaesaeyqjmci6urxzlmjpyvuzaaujj5cpzy) )

AltairZ80 is a part of SIMH family of emulators. You can download SIMH documentation from here:

- [SIMH Users’ Guide](http://simh.trailing-edge.com/pdf/simh_doc.pdf) ( [Local copy](https://link.storjshare.io/jvtg4ghgzfe35l5lfyzhdeuwyzdq/virtualhub-setup%2FAltairZ80%2Fsimh_doc.pdf?download=true) / [IPFS](https://dweb.link/ipfs/bafkreihuwr5b6f4a3evhzojpnez7ye7ckee45qcvtpxcb2exvcnkyqgsk4) )
- [SIMH FAQ](http://simh.trailing-edge.com/pdf/simh_faq.pdf) ( [Local copy](https://link.storjshare.io/jxviezwk4qnsnycu3azyrhgkn7jq/virtualhub-setup%2FAltairZ80%2Fsimh_faq.pdf?download=true) / [IPFS](https://dweb.link/ipfs/bafkreickurjax44p6wvb3zaejajo232j564vrf2ua75koyqh75tetmw54q) )


## Credits

- [AltairZ80 Emulator (© 2022 by Peter Schorn)](https://schorn.ch/altair.html) - [Peter Schorn](mailto:peter.schorn@acm.org)
- [SIMH](http://simh.trailing-edge.com/)
