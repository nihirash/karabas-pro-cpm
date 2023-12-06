# CP/M 2.2 port for Karabas Pro

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D6JVS74)

![screenshot](readme/screen.png)

Important note!

It's still unstable! Use on your risk but feel free use any ideas from this code for building your own products!

## About project

This repository contains vanilla CP/M 2.2 ported to Karabas Pro. 

It uses +3DOS volumes on Z-Controller SD card as CP/M's partitions.

**This software still in development and can be unstable!**

## SD Card layout

MMC card should have +3DOS volumes. Most important things are - SD card should have these volumes:
 * `CPM.A`(case sensitive - important create them in uppercase, 8 megs size - cause CP/M 2.2 limitations)
 * `CPM.B`(similar)
 * `CPM.C`

 Only `CPM.A` volume is mandatory but it easier to use with 3 drives

## Development

I'm using sjasmplus assembler for development tasks and ZXMak2 emulator.

More information will be added later.

## Terminal

Currently, implemented ADM-3 compatible terminal(like KayPro) with some extensions.

## License

CP/M port licensed with [Nihirash's Coffeware License](LICENSE).

It isn't hard to respect it.

Happy hacking!