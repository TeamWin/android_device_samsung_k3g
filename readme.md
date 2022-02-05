# Samsung Galaxy S5 SM-G900H TWRP Device Tree

TWRP Device tree for the Samsung Galaxy S5 Exynos

This tree compatible with TWRP 3.6.0_9 as of 05/02/2022

---
![Samsung Galaxy S5](https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-s5-g900f-1.jpg)


# About Device

Samsung Galaxy S5 Exynos (k3gxx)

### Specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 4x1.9GHz Cortex-A15 + 4x1.3Ghz Cortex-A7, ARM big.LITTLE
Chipset | Samsung Exynos 5422 Octa
GPU     | ARM Mali T628-MP6
Memory  | 2 GB
Shipped Android Version | 4.4.2
Updated Android Version | 6.0.1
Storage | 16 GB
MicroSD | Up to 64 GB
Battery | 2800 mAh (non-removable)
Dimensions | 159 x 75.1 x 8.5 mm
Display | 1080 x 1920 pixels, 5.1" Super AMOLED
Rear Camera  | 16.0 MP, LED Flash
Front Camera | 2.1 MP

---

#  Steps to Compile

 Place the device tree in proper location $SOURCE_HOME/device/samsung/k3gxx/ 
 
 Add Omni Source or Minimal TWRP Source
 
 `repo sync git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-6.0`
 
Then Run `repo sync` 

```sh
. source ./build/envsetup.sh && lunch omni_k3g-eng && make clean && make -j# recoveryimage
```
`# = No. of CPU threads of your PC'

#  Kernel Source here

 Kernel Source from which the prebuilt kernel is built is here, twrp-6.0 branch.
 
 https://github.com/akhil1999/android_kernel_samsung_k3gxx

### Thanks to:
 * Me, akhil1999
 * TeamWin
