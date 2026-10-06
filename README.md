# 豆豆图纸 Android 更新

当前版本为 V1.2.6。App 从固定地址读取 [latest.json](latest.json)，发现更高版本后在浏览器打开对应 APK。

## V1.2.6 离线激活

新版采用一机一码。所有用户（包括从旧版升级的用户）首次打开新版时，需将 App 显示的设备码发给商家，获取对应的 16 位卡密。卡密验证无需联网；请在升级前准备卡密。

## 发布新版

1. 保持包名 `com.doudou.pattern` 与 APK 签名密钥不变，增加 Android `versionCode`。
2. 沿用原离线发卡密钥，否则已发出的卡密会失效。发卡密钥不得上传到本公开仓库。
3. 先上传签名 APK 并确认下载地址可用，再修改 `latest.json` 的 `versionCode`、`versionName`、`apkUrl` 和 `notes`。
4. 用旧版 App 验证更新提示和浏览器下载，再用真实手机验证覆盖安装及离线激活。

版本信息：<https://raw.githubusercontent.com/zebin41s-source/doudoupindou/main/latest.json>
