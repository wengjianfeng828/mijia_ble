此分支为ST bluenrg-1平台的米家蓝牙标准接入SDK，米家在原厂SDK基础上，提供库以及示例demo。

### 使用

1、 先到ST官网搜索STSW-BLUENRG1-DK 注册并获取低功耗蓝牙sdk2.6.0 

http://www.st.com/content/st_com/en/products/embedded-software/evaluation-tool-software/stsw-bluenrg1-dk.html

2、进入SDK目录
```
cd BlueNRG-1_2 DK 2.6.0\Project\BLE_Examples
git clone -b ST --recursive https://github.com/MiEcosystem/mijia_ble.git
```

3、将从米家开放平台上申请得到的mijia_std_authen_IAR_BLUENRG-1_1_1_2.a

拷贝到mijia_ble\libs\mible_app_authen文件夹下，米家蓝牙标准认证库闭源，请联系 https://iot.mi.com/ 平台申请，详见https://iot.mi.com/guide.html#id=57

4、工程开发环境:IAR8.22.1, 工程路径mijia_ble\demos\BlueNRG-1\mible_std_authen\EWARM\BlueNRG-1\BLE_Chat.eww

5、此demo可以在STEVAAL-IDB007V1开发板上运行，STEVAAL-IDB007V1开发板请在ST官网申请或采购，安装dk后使用相关烧录工具flasher对芯片进行烧录，也可以使用STlink直接烧录并仿真。

6、米家认证库的具体说明参见：https://miecosystem.github.io/mijia_ble/

### 其他
1、开发环境目前支持IAR，后续会支持Keil。

2、芯片型号目前只支持BlueNRG-1，后续会增加BlueNRG-2以及相关系列。

3、目前分配了0x400的heap使用，如需更改，请在icf文件中修改。

4、如需获取技术支持，请于ST原厂或代理商联系。

