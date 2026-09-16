# SimpleDisableSecureFlag

在设置了 `FLAG_SECURE` 的应用中启用截图，并禁用截图与录屏检测。

> 仅 100 行代码，轻装上阵，最小影响

## 支持范围

- Android 12+
- libxposed API 102 框架
- 已在 Android API 37 上使用 Vector 2.2 测试

## 使用方法

1. 安装 APK。
2. 在框架管理器中启用该模块。
3. 将 `system_server` 以及目标应用加入模块作用域。
4. 重启。

需要 `system_server` 作用域以接收 Android 系统级捕获回调；启用期间会影响系统范围内的回调注册。
