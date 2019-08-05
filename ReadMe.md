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



