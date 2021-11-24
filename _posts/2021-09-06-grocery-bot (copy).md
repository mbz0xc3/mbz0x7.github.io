---
title: Using MASM on GNU/Linux (Easiest way)
author: MBZ0x7
date: 2021-11-08 15:10:00 +0800
categories: [assembly]
tags: [assembly]
pin: false
---
### What is the problem ?
MASM (Microsoft Macro Assembler) is a famous x86 assembler belonging to Microsoft that works on Windows only. It's used to convert assembly code into machine language.

If you guessed it from title :D, I am not a fan of Windows so I searched how to get it works on GNU/Linux.
After some times trying some methods I came across a fast and easy solution with less overhead.
So, I wanted to share it with you. It's just code and run.

### Get MASM on GNU/Linux
The first requirement is to install Microsoft Visual Code IDE which you can find it on your distribution repository most likely.

Then you'll need [MASM/TASM](https://marketplace.visualstudio.com/items?itemName=xsro.masm-tasm) which offers:

Language Support: Offer grammar,basic outline view,hover,code formate support for DOS assembly language.
Run and debug: Right click on the VSCode editor panel, run and debug your code.
Diagnose: process the output of ASM tools and display them in VSCode.

also [DOSBox](https://marketplace.visualstudio.com/items?itemName=xsro.vscode-dosbox) the FOSS, multi-platform, DOS x86 emulator which will integrate with MASM/TASM extension.

You can download them from Extensions section of VSCode ones you download it.

Then, after you write your assembly code. Righ click and press `Run ASM Code` and it will assemble, link and load it for you automatically on DOSBox emulator in another VSCode tab.

![](../../assets/img/posts/2/masm.png)

Don't forget to switch to change the default assembler from TASM to MASM.
![](../../assets/img/posts/2/masm.png)