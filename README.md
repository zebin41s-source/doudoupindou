# 豆豆图纸 Android 更新

本仓库保存安卓安装包及版本信息。App 从固定地址读取 [`latest.json`](latest.json)，发现更高版本后使用浏览器打开对应 APK 下载地址。

## 发布新版

1. 保持包名 `com.doudou.pattern` 与原签名密钥不变，增加 Android `versionCode`，生成新 APK。
2. 将 APK 以包含版本号的文件名提交到仓库根目录，例如 `doudou-pattern-v1.2.5.apk`。
3. 修改 `latest.json` 的 `versionCode`、`versionName`、`apkUrl` 和 `notes`，在 APK 已可下载后提交。
4. 用已安装的旧版 App 点击“检查更新”，验证版本号、浏览器下载与覆盖安装。

更新地址：`https://raw.githubusercontent.com/zebin41s-source/doudoupindou/main/latest.json`

APK 下载地址由 `latest.json` 中的 `apkUrl` 指定。首次启用更新功能前安装的旧版需要顾客手动覆盖安装一次。

