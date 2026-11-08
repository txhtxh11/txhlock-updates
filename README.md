# 答题锁屏 · 应用内更新通道

> 当前版本：**v2.0.6**（versionCode 216）
> 本仓库只放更新文件和安装包，**不含源码**；源码在私有仓库。

## 文件

| 文件 | 说明 |
|---|---|
| `update.json` | 版本号、MD5、下载地址 |
| `apk/txhlock_vX.Y.Z.apk` | 安装包（只保留最新一版） |

App 的 `UpdateManager` 从本仓库的 raw / CDN 读取 `update.json`，校验 MD5 后拉起安装。

## 直链

- `https://raw.githubusercontent.com/txhtxh11/txhlock-updates/master/update.json`
- `https://cdn.jsdelivr.net/gh/txhtxh11/txhlock-updates@master/update.json`

## 发版

1. 上传新 APK 到 `apk/`；
2. 更新 `update.json`（versionCode / versionName / md5 / urls）；
3. 删除旧 APK；
4. commit + push。