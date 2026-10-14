# MGLive Android 下载

MGLive 是用于两台设备在局域网内配合拍摄的工具。一台设备分享相机画面，另一台设备实时监看，并可使用配对确认、远程快门、语音和互动功能。当前发布为公开测试版。

## 下载

- [Android 安装包（ARM 32/64 位，兼容范围更广）](https://github.com/lukamorefree/mglive-downloads/releases/latest/download/MGLive-Android.apk)
- [Android ARM64 精简安装包（推荐现代 Android 手机）](https://github.com/lukamorefree/mglive-downloads/releases/latest/download/MGLive-Android-arm64.apk)
- [版本说明和 SHA-256 校验文件](https://github.com/lukamorefree/mglive-downloads/releases/latest)

当前版本：**0.3.66（73）**；Android 8.0 及以上；包名：`com.mglive.sender`。OPPO Find X8、Redmi Note 11T Pro 等 ARM64 手机可使用精简版。两个安装包的功能、版本号和签名相同，不需要同时安装。Intel/x86 Android 设备不适用这两个手机安装包。

请从此仓库的 Releases 下载 APK，再按 Android 的安装提示允许浏览器安装。旧版 MGLive 用户可以覆盖安装，无需卸载。不要通过卸载或清除数据解决账号问题，当前测试版仍在完善账号恢复。

## 使用与权限

两台设备应在可互访的同一局域网内。首次分享时，Android 会请求屏幕共享许可；需要远程快门及相关辅助操作时，会引导用户开启无障碍服务；语音功能需要麦克风许可。用户可以在系统设置中撤销权限。局域网发现所需的附近设备/旧系统位置许可依 Android 版本而异。

相机画面和实时语音通过设备之间的 WebRTC 连接传输。云 API 用于账号及权限服务。当前 Android 测试版尚未启用 Jianpay 购买入口，付款和永久 Pro 销售流程仍在开发与审核中。

仅在信任的局域网中使用；旧版兼容信令仍基于局域网 TCP。不要把拍摄端的信令端口映射到互联网。

## 版本来源与签名

此仓库仅发布安装包和说明，源代码单独管理。公开 APK 为关闭调试、经 R8 优化的发布构建。

签名证书 SHA-256：

```text
246D647D484F09D763A19B9494A739AC51550EB4282654AE283D46E93548FFCE
```

请以 Releases 中的 `SHA256SUMS.txt` 核对实际下载文件。证书指纹是公开验证信息，签名私钥不会随安装包发布。
