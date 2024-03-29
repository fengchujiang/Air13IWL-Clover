## Lenovo 小新 Air13IWL Clover `(xlivans)`
### 感谢 宪武 小兵 各位群友 大佬们 为此机型的辛苦付出

##### 如何安装系统请跳跃至小兵大佬教程 : https://github.com/daliansky/Lenovo-Air13-IWL

##### 配置说明 : https://github.com/xlivans/Air13IWL

##### 自用 OpenCore : https://github.com/xlivans/Air13IWL-OC

##### 自用 Clover : https://github.com/xlivans/Air13IWL-Clover

##### 微云 : https://share.weiyun.com/5yMO9jB

----

#### 2019-08-26

+ 更新机型和变频数据使用`MacBookPro15,4`
+ 更新显卡ID使用`3EA60005`,解决高Hidpi异常问题

#### 2019-08-12

+ 更新Clover版本至5045
+ 更新`Acidanthera`所有驱动

#### 2019-08-10

+ 定制`AppleALC.kext`,默认使用子骏ID：98（62000000）无需使用`ALCPlugFix`和`CodecCommander.kext` ,3.5mm麦克风需要手动切换；可选原版小兵ID：99（63000000）需安装 `ALCPlugFix` 并使用 `CodecCommander.kext` 

+ 添加 `BrcmFirmwareData.kext` , `BrcmPatchRAM2.kext`（`DW1820A`蓝牙驱动）,此驱动经过修改只适合ID：`0a5c_6412`使用

#### 2019-08-03

+ 更新Clover版本5033

- 移除声卡注入`device-id`，修改`Air13IWL.kext`，声卡驱动`AppleALC.kext`可单独使用不在受`FakePCIID.kext`和`FakePCIID_Intel_HDMI_Audio.kext`影响，使用HDMI音频仍需`FakePCIID.kext`
- 移除部分驱动内的非必要文件

#### 2019-07-27

+ 更新`SSDT-Air13IWL.aml`
+ 从`Air13IWL.kext`中分离`BrcmBluetoothInjector.kext `
+ 添加`Config.plist` -`RtVariables` - `CsrActiveConfig` 参数  `0x67`，默认关闭SIP

#### 2019-07-26

+ 上传完整EFI目录方便单系统用户直接替换

#### 2019-07-17

+ Clover版本5018
+ 使用前先补全`Config.plist` - `SMBIOS`
+ 整合`SSDT-XOSI.aml` , `SSDT-XCPM.aml` , `SSDT-PNLF.aml` , `SSDT-SBUS.aml` , `SSDT-EC.aml` , `SSDT-Q11Q12.aml` , `SSDT-GPRW.aml` 合并为`Air13IWL.aml`
+ 整合`CPUFriendProvider.kext` , `FakePCIID_Intel_HDMI_Audio.kext` , `XHCI-unsupported.kext` , `USBPorts.kext` , `BrcmBluetoothInjector.kext` 合并为`SSDT-Air13IWL.kext`



