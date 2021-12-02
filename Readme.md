# OpenCore 0.7.5 for Ryzen 1600X, B350, RX480
## **Before use, MUST BE generating Platforminfo value, Core Replace value!** Checkout [Information](#1.-Information)!

- [한국어](https://github.com/icaros7/OpenCore_Ryzen_B350/blob/main/Readme_ko.md)
- English (This document)

![](screenshot.png)

# 1. Information
The laest version of OpenCore that based on OpenCore 0.7.5

|✅ / ❌|Feature|Etc|
|:---:|:---|:---|
|✅|Hardware Acceleration||
|✅|Play DRM||
|✅|VGA Identify|Sapphire Radeon RX480 8GB|
|❌|Microphone|Cause from `AppleALC`|

You can use this bootloader for hackintosh install & daily-use

<span style="color:red">**Please change serial number and UUID from `default value`**</span> by way of SMBIOS Generator like [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS). You can follow [this guide of OpenCore Official Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#platforminfo).

FYI, If you not using Six Core Ryzen, you must be patch for your CPU. Check out at [AMD-OSX's AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla).

# 2. Tested Environment
Successfully working following environment.

- macOS 11.6.1
- AMD Ryzen 1600X (Six Core)
- MSI B350M Mortar
- Samsung DDR4 24GB @3200Mhz
- Sapphire Radeon RX480 8GB
- 120GB for macOS
- Multi-boot environment via rEFInd

# 3. Configuration
Include following configuration

- Default Language : Korean (You can choose other language at installation step)
- Default Keyboard Layout : Qwerty
- Boot Timeout: 5 Sec.
- Set Default: Enabled (`Ctrl + Enter` to set default)
- SecurityPolicy: Disabled
- Hide Auxiliary: Enabled (`Space Bar` to see that entry like recovery)
- Boot Verbose: Disable
- Apple Hot Key: Enable (`Cmd + V` to boot with Verse mode)
- iMac (Retina 4K, 21.5-inch, 2019) Model (`iMac19,2`)
- AMD Kernel Patch for 1600x (set for Six Core)

# 4. Special Thanks To
- [@acidanthera](https://github.com/acidanthera) - [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg) and etc...
- [@AMD-OSX](https://github.com/AMD-OSX) - [AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla) patch