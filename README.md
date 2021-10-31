# Hackintosh-EFI-For-ASUS-B250M-i5-7500-RX580

[中文说明](README_ZH.md)

# # Introduction

Recently, Xianyu received a piece of RX580 for personal use. I have made integration and modification after referring to a lot of articles and other predecessors' EFI. Thank you.

No independent graphics card EFI, only added models, three code need to be generated to add.
Core graphics card platform ID: 59120000, just a simple patch to add some attributes of the device, can be regenerated if necessary.

# # Update
- 2021-10-31
	- OC 0.7.5
	- Update KEXT regularly
	- Support Big Sur & Monterey

- 2021-06-12
	- OC 0.7
	- Update KEXT regularly
	- Support Big Sur & Monterey

- 2021-05-05
	- OC 0.6.9
	- Update KEXT regularly
	- Support Big Sur 11.3.1

- 2020-12-31
	- Added EFI without stand-alone display, model MacMini8,1

- 2020-12-15
	- Updated to Big Sur 11.1
	- Replace boot program to OC 0.6.4

- 2020-05-25
	- Keyboard, mouse and Bluetooth interface are built in
	- USB interface customization
	- Delete some useless files
	- Update Clover 5118

- 2020-05-22
	- Initial upload

# # Configuration

- CPU: i5-7500
- Memory: Kingston DDR4 2400MHz 8GB x 2
- hard drive:
	- Toshiba RD500 500G M.2 NVME
	- Samsung SSD 860 EVO 250GB SATA
	- Samsung SSD 850 EVO M.2 250GB
	- Western Digital Mechanical Blue Plate 1TB
- Fan: Cool Blizzard Supreme T400i
- Graphics card: Sapphire RX580 8G 2304SP
- Network card: BCM94360CS2 + PCIE adapter card
- Display: Viewsonic VX2478-4K-HD

# # The Bios Settings
(Refer to the following general options for Settings)

### Disable
- Fast Boot
- Secure Boot
- Serial/COM Port
- Parallel Port
- VT-d
- CSM
- Thunderbolt
- Intel SGX
- Intel Platform Trust
- CFG Lock

### Enable
- VT-x
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS Type: Windows 8.1/10 UEFI Mode
- DVMT Pre-Allocated(iGPU Memory): 64MB
- SATA Mode: AHCI

## Working status

### Work normally:

- The sound card
- The network card
- Bluetooth
- Airdrop
- Hand off
- App store
- Sleep
- H.264, HEVC hardware decoding, encoding, video processing
- SATA SSD Trim (terminal input: sudo Trimforce Enable)

## Instructions for use

- The model has been set and can be installed normally. Please generate the three sizes by yourself

# # Thanks To

- [acidanthera](https://github.com/acidanthera)
- [daliansky](https://github.com/daliansky/)
- [Mrliu12123](http://bbs.pcbeta.com/viewthread-1851046-1-1.html)
