# 答题锁屏 · 应用内更新通道

这个仓库**只放更新文件和 APK**，不含源码。源码在私有仓库里。

- `update.json`：版本号、MD5、下载地址
- `apk/txhlock_vX.Y.Z.apk`：安装包

App 的 `UpdateManager` 会从此仓库的 raw / CDN 地址读取 `update.json`。