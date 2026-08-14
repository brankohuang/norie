# 验证 Norie 官方 APK

如果你希望确认一个 Norie APK 是否来自 Branko 的官方长期签名，可以核对 Android 签名证书。

## 官方身份

```text
Application ID
io.github.brankohuang.norie

Official certificate SHA-256
69:FF:B6:3C:1A:09:7F:42:85:5E:53:DE:CA:60:3B:3F:B3:ED:89:95:0E:40:0E:73:D0:62:EC:BA:24:D3:7E:7A
```

这个证书指纹应在正式 Norie Release 版本之间保持不变。

## 使用 apksigner 检查

如果电脑安装了 Android SDK Build Tools，可以运行：

```powershell
apksigner verify --print-certs Norie-v0.23.3-release.apk
```

输出中的 signer certificate SHA-256 应与上面的官方证书指纹一致。

## 校验某个 Release 文件的 SHA-256

每个 APK 文件本身还可以有独立 SHA-256。它用于确认你下载到的文件是否与该 Release 发布时的文件完全一致。

Windows PowerShell：

```powershell
Get-FileHash .\Norie-v0.23.3-release.apk -Algorithm SHA256
```

注意：

- **Certificate SHA-256** 用来识别长期发布者签名；
- **APK SHA-256** 用来识别某一个具体 APK 文件。

两者用途不同。
