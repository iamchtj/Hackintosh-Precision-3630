# Hackintosh-Precision-3630-Tower-Workstation


**Opencore Bootloader 0.7.5. Tested on Big Sur 11.6.1**


## Introdution
This is the Hackintosh EFI Folder for Dell Precision 3630 Tower Workstation. The configuration settings support MacOS Big Sur. 


## Hardware Specifications
* **Desktop Computer**: [Dell Precision 3630 Tower Workstation](https://www.dell.com/en-us/work/shop/desktops-all-in-one-pcs/precision-3630-tower-workstation/spd/precision-3630-workstation)
* **CPU**: [Intel® Core™ i7-8700](https://ark.intel.com/content/www/us/en/ark/products/126686/intel-core-i78700-processor-12m-cache-up-to-4-60-ghz.html)
* **iGPU**: Intel® UHD Graphics 630
* **RAM**: 32GB DDR4 2666 Daul Channel
* **HDD**: Western Digital 1TB WD Blue PC Hard Drive
* **LAN**: Intel I219LM7
* **Audio**: Realtek ALC255
* **Wi-Fi & Bluetooth**: Intel Wi-Fi 6 AX200


## Working
* CPU Turbo Boost
* iGPU acceleration
* Internal Speaker & Front panel 3.5mm HeadSet/HeadPhone jack & Line out
* All front USB Ports
* LAN & Wireless network
* Sleep & Wakeup


## Known Issue
* Need to enable Power Nap for sleep
* Bluetooth can't connect Xbox controller 
* Apple Music subscription can't play Lossless and higher quality
* Apple TV might not work


## BIOS Settings
* System Configuration → SATA Operation: ***AHCI***
* Secure Boot → Secure Boot Enable: ***Disabled***
* Intel® Software Guard Extensions™ → Intel® SGX™ Enable: ***Software controlled or Disabled***
* Virtualization Support → VT for Direct I/O: ***uncheck***
* Power management → Deep Sleep Control: ***Disabled***
* USB Wake Support: ***uncheck***


## BIOS Settings via GRUB
* Set Pre-Allocated DVMT to 64M: 
***setup_var 0x8DE 0x02***
* Disable CFG lock: 
***setup_var 0x5C0 0x00***


## Fon Fix

### Front panel combo 3.5 jack detection
More details to see: [MicFix](https://github.com/WingLim/MicFix)

### Rear USB port
More details to see: [USBToolBox](https://github.com/USBToolBox/tool)
