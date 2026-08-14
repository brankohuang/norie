# GitHub 仓库创建建议

## Repository name

```text
norie
```

## Description

```text
A quiet, local-first personal bookkeeping app for Android. Your data stays yours.
```

## Visibility

```text
Public
```

## 建议开启

- Issues
- Releases

## 不需要开启

如果只是安静发布 APK，可以暂时不启用：

- Discussions
- Wiki
- Projects

## APK 放在哪里

**推荐放 GitHub Releases，不要把 APK 直接 commit 到仓库主分支。**

流程：

1. 打开仓库右侧 `Releases`；
2. `Draft a new release`；
3. Tag 例如 `v0.23.3`；
4. Title 例如 `Norie v0.23.3`；
5. 使用 `RELEASE_TEMPLATE.md` 作为说明基础；
6. 上传 `Norie-v0.23.3-release.apk`；
7. 填入构建脚本输出的 APK SHA-256；
8. Publish release。

## 主分支只需要放什么

```text
README.md
PRIVACY.md
DOWNLOAD.md
VERIFY.md
CHANGELOG.md
NOTICE.md
assets/
screenshots/
.github/
```

不需要上传：

```text
src/
android/
node_modules/
构建脚本
内部需求文档
内部项目交接文档
keystore
签名 properties
真实账单 ZIP
真实账户 ZIP
API Key
个人迁移 Excel
```
