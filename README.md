# larksuite-bin
AUR [packages/larksuite-bin](https://aur.archlinux.org/packages/larksuite-bin)

[README-EN](/REMEAD-EN.md)

源由：飞书国际版（larksuite）在下载链接中通过时间戳和签名，构建 .deb 的包下载需要手动下载构建，所以我这里 releases 就缓存一份当前版本的 deb 包文件用于 AUR 包的构建。

Maintainer: https://github.com/strrl

## 本仓库无法解决

- 无法解决小版本更新但是不更新 pkgver 的
- 无法解决自动化下载并同步至 PKGBUILD
- 无法解决 Larksuite 对不同国家及地区的内容不一致

如果你不信任本仓库提供的 deb 文件包，可以自行到 Larksuite 官网进行下载：
- https://www.larksuite.com/download

然后校对 PKGBUILD 的 sha256sums，和 releases 里面提供的 sha256，如果不一样你可以选择不使用我缓存的文件，自行修改构建 Larksuite 。

![截图 2025-07-07 10-22-16](https://github.com/user-attachments/assets/cc72253e-fa4c-42a2-83c6-ed49b40e65b3)

本仓库使用 MIT 许可证，您可以自由更改，如果本人无法留意到更新提交 [issues](https://github.com/miaoermua/larksuite-bin/issues/new) 提醒我进行更新。🤗

## 不通过 AUR 构建安装本项目

```sh
git clone https://github.com/miaoermua/larksuite-bin.git
cd larksuite-bin
makepkg
sudo pacman -U larksuite-bin-*.pkg.tar.zst
```

![截图 2025-07-07 11-13-21](https://github.com/user-attachments/assets/ff4aabfb-ee3a-475b-b5fb-221aa4bf2529)

<!--
## 通过 AUR 安装

还在旧版本，没完全谈完

```sh
paru -S larksuite-bin
```
--->
