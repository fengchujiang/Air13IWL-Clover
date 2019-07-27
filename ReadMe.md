#### 2019-07-27

+ 更新`Air13IWL.aml`
+ 从`Air13IWL.kext`中分离`BrcmBluetoothInjector.kext `

#### 2019-07-26

+ 上传完整EFI目录方便单系统用户直接替换

#### 2019-07-17

+ Clover版本5018
+ 使用前先补全`Config.plist` - `SMBIOS`
+ 整合`SSDT-XOSI.aml` , `SSDT-XCPM.aml` , `SSDT-PNLF.aml` , `SSDT-SBUS.aml` , `SSDT-EC.aml` , `SSDT-Q11Q12.aml` , `SSDT-GPRW.aml` 合并为`Air13IWL.aml`
+ 整合`CPUFriendProvider.kext` , `FakePCIID_Intel_HDMI_Audio.kext` , `XHCI-unsupported.kext` , `USBPorts.kext` , `BrcmBluetoothInjector.kext` 合并为`Air13IWL.kext`



