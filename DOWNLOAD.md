# 下载与安装 Norie

## 官方下载位置

Norie 的正式 APK 只通过本仓库 GitHub Releases 免费发布：

**https://github.com/brankohuang/norie/releases**

建议不要从网盘、论坛转载、网店或来源不明的网站下载 Norie。

## 下载哪个文件

在对应版本的 Release 页面下载类似：

```text
Norie-v0.23.3-release.apk
```

如果 Release 同时提供 SHA-256，请一起核对。

## Android 安装

第一次安装 GitHub 下载的 APK 时，Android 可能提示是否允许当前浏览器或文件管理器“安装未知应用”。这是直接安装 APK 的正常系统安全流程。

请只为你信任的下载来源授权。

## 以后升级

官方 Norie Release 使用同一长期 Android 签名发布。

正常升级时直接安装新版本 APK 即可。Android 会在签名一致且 Application ID 相同的情况下覆盖升级，不应主动删除 Norie 的本地 SQLite 数据。

尽管如此，重要升级前仍建议先在 Norie 中导出数据备份。

## 官方 Android 身份

```text
Application ID
io.github.brankohuang.norie

Certificate SHA-256
69:FF:B6:3C:1A:09:7F:42:85:5E:53:DE:CA:60:3B:3F:B3:ED:89:95:0E:40:0E:73:D0:62:EC:BA:24:D3:7E:7A
```

更详细的 APK 验证方法见 [VERIFY.md](./VERIFY.md)。

## Norie 是免费的

Norie 当前通过官方 GitHub 仓库免费发布。

如果有人以“官方授权”“正版激活”“付费购买 APK”等名义销售 Norie，请先核对本仓库以及应用内的“设置 → 关于 Norie → 官方项目主页”。
