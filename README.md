# GuoFlix TV

适配 Android TV 和遥控器的短剧播放器。

## 项目说明

支持 Android 8.0 及以上系统。当前版本仅公开源码和 Git 备份，不提供公开 APK 下载。


## 线路配置

本仓库的 [playback-routes.json](./playback-routes.json) 用于应用支持的备用线路配置。电视端会定期检查，也可以进入“设置 → 刷新线路配置”手动更新。

修改配置后，需要增大 `revision` 再提交。仅支持应用内置允许的域名、模式和参数，无效配置会被忽略。

普通线路参数调整可以远程更新；签名算法或播放协议变化需要升级 APK。0.14.5 起已内置当前官方播放协议，旧 JSON 配置保留作为备用。

## 源码与备份

[下载页面](https://github.com/LorenYan98/guoflix-routes/releases/latest) 中：

- `source.zip`：完整源码。
- `.bundle`：包含提交历史的 Git 备份。

应用派生源码遵循 GPL-3.0-only，第三方声明与构建文件随源码包提供。

本项目是第三方客户端，与红果官方无隶属关系。播放能力取决于上游服务和设备支持。

