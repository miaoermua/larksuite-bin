# larksuite-bin
AUR [packages/larksuite-bin](https://aur.archlinux.org/packages/larksuite-bin)

源由：飞书国际版（larksuite）在下载链接中通过时间戳和签名，构建 .deb 的包下载需要手动下载构建，所以我这里 releases 就缓存一份当前版本的 deb 包文件用于 AUR 包的构建。

## 本仓库无法解决

- 无法解决小版本更新但是不更新 pkgver 的
- 无法解决自动化下载并同步至 PKGBUILD
- 无法解决 Larksuite 对不同国家及地区的内容不一致

如果你不信任本仓库提供的 deb 文件包，可以自行到 Larksuite 官网进行下载：
- https://www.larksuite.com/download

然后校对 PKGBUILD 的 sha256sums，和 releases 里面提供的 sha256，如果不一样你可以选择不使用我缓存的文件，自行修改构建 Larksuite 。

本仓库使用 MIT 许可证，您可以自由更改，如果本人无法留意到更新提交 issuse 提醒我进行更新。🤗