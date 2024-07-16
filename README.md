# Ryzen 5 5600G Hackintosh EFI
OpenCore EFI for B450 chipset with AMD Ryzen 5 5600G with iGPU.
# 🖥️ Specification
- **CPU:** AMD Ryzen 5 5600G at 3.9Mhz
- **GPU:** Radeon™ Integrated Graphics (Vega 7)
- **MB:** Asus Prime B450M-A II (*Latest BIOS*)
- **RAM:** 2x8GB DDR4 at 3200Mhz
- **Storage:** 512GB SSD
- **Audio:** ALC892 (alcid=11)
- **Ethernet:** RTL8111 by Realtek
- **Boot mode:** UEFI; **Bootloader:** OpenCore 1.0.0; **OS:** Sonoma 14.5 v Windows 11

> Warning: I built this EFI for myself and it is not guaranteed that it will work on any other devices. You can always follow Dortania's guide for setting up your own EFI.

# 📖 Tutorial
- **DIY:** https://dortania.github.io/OpenCore-Install-Guide/
- **USB Installer:** https://dortania.github.io/OpenCore-Install-Guide/installer-guide/
- **SMBIOS:** https://github.com/corpnewt/GenSMBIOS

> SMBIOS infos are empty, please generate your own SMBIOS and edit config.plist 
- All kinds of errors, kernel panics and etc. are beyond my responsibility. However I'm open to questions and suggestions, feel free to contact me on Discord: @skijam

# ❗ Known issues
- Memory map problems can keep your PC from booting. It is an known issue that has nothing to do with this EFI. It's connected to the motherboard. Feel free to edit ```boot-args``` and delete ```slide=xxx```. However, if memory problem occure (you'll know when it occured if you see some random numbers and Apple Stop sign while booting), you'll have to experiment with this number a bit.
> Motherboard is randomizing Memory Map, so sometimes it will throw an error, and sometimes it will work just fine. Current fix is to keep it at one number (ex. 146) and restart it until it boots. Yikes.

# 🖼️ Result

![image](https://github.com/Vuxoni/Sonozen---Ryzen-5600G-APU-Hackintosh/assets/86528980/5999151c-3eb8-401e-81f5-dd3195ed2a7c)

# ❗ Works on Sequoia too :) Well...
- Currently it's not possible to enable AppleALC on AMD machines running Sequoia. You should use USB headphones instead / or VoodooHDA (didn't try that).
- CPU Name is wrong, patchable but I'm kinda lazzy right now.
![image](https://github.com/Vuxoni/Sonozen---Ryzen-5600G-APU-Hackintosh/assets/86528980/cf133b95-da65-482a-9cd7-c5ce2c2e006d)
