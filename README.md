# Gab's build of dwm(forked from Luke)

## FAQ
! 
Check out [config.h](config.h) for bindings and config


## Patches and features

- [Clickable statusbar](https://dwm.suckless.org/patches/statuscmd/) with Luke's build of [dwmblocks](https://github.com/lukesmithxyz/dwmblocks).
- Reads [xresources](https://dwm.suckless.org/patches/xresources/) colors/variables (i.e. works with `pywal`, etc.).
- scratchpad: Accessible with <kbd>mod+shift+enter</kbd>.
- New layouts: bstack, fibonacci, deck, centered master and more. All bound to keys <kbd>super+(shift+)t/y/u/i</kbd>.
- True fullscreen (<kbd>super+f</kbd>) and prevents focus shifting.
- Windows can be made sticky (<kbd>super+s</kbd>).
- [hide vacant tags](https://dwm.suckless.org/patches/hide_vacant_tags/) hides tags with no windows.
- [stacker](https://dwm.suckless.org/patches/stacker/): Move windows up the stack manually (<kbd>super-K/J</kbd>).
- [shiftview](https://dwm.suckless.org/patches/nextprev/): Cycle through tags (<kbd>super+g/;</kbd>).
- [vanitygaps](https://dwm.suckless.org/patches/vanitygaps/): Gaps allowed across all layouts.
- [swallow patch](https://dwm.suckless.org/patches/swallow/): if a program run from a terminal would make it inoperable, it temporarily takes its place to save space.


Installation

dependencies for Debian/Ubuntu

```bash
  sudo apt install build-essential -y
  sudo apt install libx11-dev -y
  sudo apt install libxft-dev -y
  sudo apt install libxinerama-dev -y
  sudo apt install libx11-xcb-dev -y
  sudo apt install libxcb-res0-dev -y
```

```bash
git clone https://github.com/LukeSmithxyz/dwm.git
cd dwm
sudo make install
```

There is also a `PKGBUILD` usable on distributions with pacman. Run `makepkg -si` instead of `sudo make install`.
