# VueScan packaged for Flatpak

[![VueScan-logo](/icons/icon128x128.png)](https://flathub.org/apps/details/com.hamrick.VueScan)

This is a Flatpak for the popular (but sadly, proprietary) scanning software [VueScan](https://www.hamrick.com/).

Originally released in 1998 for Windows, VueScan is now a cross-platform application with builds for Windows XP and up, MacOS X 10.3 "Panther" and up, and Linux distributions running on kernel version 2.6 or newer. It is compatible with over 6,000 devices and remains in very active development.

## Installing from Flathub

This package is available on [Flathub](https://www.flathub.org/); more information can be found there on its [listing page](https://flathub.org/apps/details/com.hamrick.VueScan).

To install, enter the following command in your terminal:

```bash
flatpak install flathub com.hamrick.VueScan
```

Once installed, you can open it through your system's application manager or from the terminal with this command:

```bash
flatpak run com.hamrick.VueScan
```

## How to build

This Flatpak uses the standard
[flatpak-builder](docs.flatpak.org/en/latest/flatpak-builder-command-reference.html)
tool to build.

You can run a command like the following to build the package from this repo
and install it in your 'user' Flatpak installation:

    flatpak-builder --install ./build com.hamrick.VueScan.yaml --force-clean --user

During development you can also run a build without installing it, like this:

    flatpak-builder --run build net.purrdata.PurrData.yml pd-l2ork

See the [Flatpak manual](http://docs.flatpak.org/en/latest/) for more information.
