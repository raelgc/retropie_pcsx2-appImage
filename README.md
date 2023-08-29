# PCSX2 Qt Setup for Retropie

Retropie plugin to install and update the [PCSX2 emulator](https://pcsx2.net) with the new [Qt interface](https://www.reddit.com/r/emulation/comments/uvf7cd/pcsx2_first_public_qt_release_is_now_available/) using the [AppImage]() version, which requires no compilation.

This will add an entry on [Retropie-Setup](https://github.com/RetroPie/RetroPie-Setup) named `pcsx2-appImage`.

Available only on `X86` (aka PC) platform.


## Requirements

Check if you have PS2 already listed in file `~/RetroPie-Setup/platforms.cfg`.

If not, create (or edit) file `/opt/retropie/configs/all/platforms.cfg` and add:

```
ps2_exts=".iso .img .bin .mdf .z .z2 .bz2 .dump .cso .chd .ima .gz"
ps2_fullname="PlayStation 2"
```


## Install

Install the `pcsx2-qt` pluging running in a terminal:

```bash
wget https://raw.githubusercontent.com/raelgc/retropie_pcsx2-qt/master/pcsx2-appImage.sh -O ~/RetroPie-Setup/scriptmodules/emulators/pcsx2-appImage.sh
```

Now you can run **RetroPie Setup** script and `rpcs2-appImage` will available under `exp` (experimental) packages section.

## Playing

Check [PCXS2 Basic Setup Guide](https://pcsx2.net/guides/basic-setup/).
