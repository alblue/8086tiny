This git repository was created from its source downloads at
  http://www.megalith.co.uk/8086tiny/download.html

Source is copyright Adrian Cable unless otherwise noted

About 8086tiny
==============

8086tiny is a free, open source PC XT-compatible emulator/virtual machine
written in C. It is, we believe, the smallest of its kind (the fully-commented
source is under 25K). Despite its size, 8086tiny provides a highly accurate
8086 CPU emulation, together with support for PC peripherals including XT-style
keyboard, floppy/hard disk, clock, and Hercules graphics. 8086tiny is powerful
enough to run software like AutoCAD, Windows 3.0, and legacy PC games.

8086tiny is highly portable and runs on practically any little endian machine,
from simple 32-bit MCUs upwards. 8086tiny has successfully been deployed on
32-bit/64-bit Intel machines (Windows, Mac OS X and Linux), Nexus 4/ARM
(Android), iPad 3 and iPhone 5S (iOS), and Raspberry Pi (Linux).

The philosophy of 8086tiny is to keep the code base as small as possible, and
through the open source license encourage individual developers to tune and
extend it as per their specific requirements, adding support, for example, for
more complex instruction sets (e.g. Pentium) or peripherals (e.g. mouse). Any
questions, comments or suggestions are very welcome in our forum.

An obfuscated version of 8086tiny (condensed into just 4043 bytes of C code)
was a winner of the 2013 IOCCC contest. Significant interest followed for a
documented, commented, maintainable version. The result is the distribution
presented here.

Feature Highlights
==================

8086tiny's feature highlights include:

* Highly accurate, complete 8086 CPU emulation (including undocumented features and behavior)
* Support for all standard PC peripherals: keyboard, 3.5" floppy drive, hard drive, video (Hercules graphics and CGA color text mode, including direct video memory access), real-time clock, timers
* Disk images are compatible with standard Windows/Mac/UNIX mount tools for simple interoperability
* Complete source code provided (including custom BIOS)

8086tiny is highly portable, with minimal system requirements:

* Minimal C runtime library support required (uses POSIX file I/O and time functions only - no memory management or string functions)
* Uses SDL 1.2 for graphics, but can compile without SDL for text-only applications
* Storage requirement: typically around 20KB for compiled binary, 9KB for BIOS image, and 720KB/1.44MB for floppy disk image
* System RAM requirement: around 1.5MB

Applications
============

Some possible applications:

* Run legacy PC software and games on modern hardware
* Teach computer architecture and Intel assembly language in a safe, sandboxed environment
* Deploy on Raspberry Pi to make the world's cheapest ($25) complete IBM-compatible PC
* Extend the code base to develop a lean, modern-processor VM

If you develop an application that makes use of 8086tiny, and would like a link
to it at http://www.megalith.co.uk/8086tiny/, please get in touch with the
author, Adrian Cable.

License
=======

8086tiny is free to use for any purpose, commercial or non-commercial, and is
made available under the MIT License.

If 8086tiny brings you joy or profit, the author, Adrian Cable, welcomes modest
donations as a token of appreciation. See http://www.megalith.co.uk/8086tiny/
for more information.

Distribution
============

The 8086tiny distribution includes:

* C source and Makefile
* BIOS source (builds with NASM [NASM]) and ready-made BIOS binary
* FreeDOS [FreeDOS] 1.44MB floppy boot disk image from Joris_VR [JorisVR]
* Documentation and license

To build 8086tiny, you will need a C compiler of your choice (such as gcc or
Microsoft Visual Studio 2013) and SDL 1.2 [SDL12].

A highly condensed version of 8086tiny (just 4043 bytes of C source) won the
2013 International Obfucated C Code Contest [IOCCC]. The distribution and
documentation are available courtesy of the IOCCC website [Tiny8086].

External Resources
==================
* NASM 2.11: Freeware x86 assembler for rebuilding the BIOS binary. [NASM]
* OSFMount: Windows tool for mounting emulator disk images on a real PC. [OFS]
* FreeDOS: Free MS-DOS-compatible OS. [FreeDOS]
* The Rugxulo 1.44MB boot disk image works well with the emulator. [Rugxulo]
* Vetusware: Legacy DOS/Windows software source. [Vetusware]
* Sample 40MB hard disk image containing a range of software. [DodgyHD]

[NASM] http://www.nasm.us/
[FreeDOS] http://www.freedos.org/
[JorisVR] http://jorisvr.nl/freedos.html
[SDL12] http://libsdl.org/download-1.2.php
[IOCCC] http://www.ioccc.org/
[Tiny8086] http://ioccc.org/years-spoiler.html#2013_cable3
[OFS] http://www.osforensics.com/tools/mount-disk-images.html
[Rugxulo] https://sites.google.com/site/rugxulo/dskthree.zip
[Vetusware] http://www.vetusware.com/
[DodgyHD] http://bitly.com/1bU8URK
