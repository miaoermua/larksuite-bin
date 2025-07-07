# larksuite-bin
AUR [packages/larksuite-bin](https://aur.archlinux.org/packages/larksuite-bin)

**Reason**: Lark Suite international version uses timestamps and signatures in the download links. The .deb package needs to be manually downloaded and built, so here in this repository's releases I have cached a deb package file for building the AUR package.

Maintainer: https://github.com/strrl

## Limitations of This Repository

- Unable to resolve issues where minor versions are updated but `pkgver` is not.
- Unable to automate downloading and synchronizing to `PKGBUILD`.
- Unable to address inconsistencies in Larksuite content across different countries and regions.

If you do not trust the `.deb` package files provided by this repository, you can manually download from the official Larksuite website:
- https://www.larksuite.com/download  

Then compare the `sha256sums` value in the `PKGBUILD` with the one provided in this repository's releases. If they don't match, you may choose not to use the cached file here and build Larksuite manually instead.

![Screenshot 2025-07-07 10-22-16](https://github.com/user-attachments/assets/cc72253e-fa4c-42a2-83c6-ed49b40e65b3)

This repository is licensed under the MIT License. You are free to make modifications. If I fail to notice an update, feel free to submit an issue to remind me to update.🤗

## Install Without Using AUR

```sh
git clone https://github.com/miaoermua/larksuite-bin.git  
cd larksuite-bin
makepkg
sudo pacman -U larksuite-bin-*.pkg.tar.zst
```

<!--
## Install via AUR

```sh
paru -S larksuite-bin
```
--->
