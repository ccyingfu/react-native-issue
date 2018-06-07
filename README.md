# 记录学习 react-native 遇到的坑

### Genymotion 启动问题

当启动报以下错误:

> FAILURE: Build failed with an exception.
>
> * What went wrong:
> Execution failed for task ':app:installDebug'.
> com.android.builder.testing.api.DeviceException: Could not create ADB Bridge. ADB location: F:\Android\Sdk\platform-tools\adb.exe

原因在于 Genymotion 用的是自己的 adb，通过设置 Genymotion 的 custom Sdk 路径来解决问题。