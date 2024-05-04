

my_strore.p12
    Password：adc123456
    Alias： my_alias

///////////////////////////////////////////////////////////////////////////

为应用/服务进行签名
https://developer.huawei.com/consumer/cn/doc/harmonyos-guides-V2/signing-0000001587684945-V2

自动签名方式调试HarmonyOS应用/元服务
https://developer.huawei.com/consumer/cn/doc/app/agc-help-harmonyos-debugapp-0000001172419675

手动签名方式调试HarmonyOS应用/元服务
https://developer.huawei.com/consumer/cn/doc/app/agc-help-harmonyos-debugapp-manual-0000001177608893

AppGallery Connect
https://developer.huawei.com/consumer/cn/service/josp/agc/index.html#/

发布HarmonyOS应用
https://developer.huawei.com/consumer/cn/doc/app/agc-help-harmonyos-releaseapp-0000001126380068

命令行构建应用/服务（API 8-9）
https://developer.huawei.com/consumer/cn/doc/harmonyos-guides-V2/command-line-building-app-hap-hvigor-0000001553061909-V2


///////////////////////////////////////////////////////////////////////////

应用包签名工具
https://gitee.com/openharmony/developtools_hapsigner

打包工具组件
https://gitee.com/openharmony/developtools_packing_tool/tree/OpenHarmony-3.1-Release

或者 [你的SDK_HOME]\openharmony\[版本号]\toolchains\lib 下有 app_packing_tool.jar、app_unpacking_tool.jar、hap-sign-tool.jar



///////////////////////////////////////////////////////////////////////////
注意 ：
material 目录不能删，它是配置完签名后sync now后生成的。
如果删了，请在 Project Structure 中 重新输入签名密码后再重新sync now。

///////////////////////////////////////////////////////////////////////////


命令打release hap包
./hvigorw clean assembleHap --no-daemon --mode module -p product=default -p debuggable=false




