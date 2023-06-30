## Welcome! Paranoid Android for xiaomi lahaina devices

-----

### Notice:

- It's just a **personal project** and not an official one.
- Force push warning
- PRs and issues are very welcomed

-----

### Tested device

- renoir (shima/sm7350)

If you used this project and it worked on your phone, you can open a pr to add your device here.

-----

### External Repositories

**Common repositories:**

[AOSPA/android_hardware_qcom_audio](https://github.com/AOSPA/android_hardware_qcom_audio)
 - branch: ```topaz-888```
 - dir: ```vendor/qcom/opensource/audio-hal/primary-hal```

[AOSPA/android_hardware_qcom_media](https://github.com/AOSPA/android_hardware_qcom_media)
 - branch: ```topaz-888```
 - dir: ```hardware/qcom/media```

[AOSPA/android_hardware_qcom_gps](https://github.com/AOSPA/android_hardware_qcom_gps)
 - branch: ```topaz-legacy-component```
 - dir: ```hardware/qcom/gps```

[AOSPA/android_hardware_xiaomi](https://github.com/AOSPA/android_hardware_xiaomi)
 - branch: ```topaz```
 - dir: ```hardware/xiaomi```

[AOSPA/android_vendor_nxp_opensource_halimpl](https://github.com/AOSPA/android_vendor_nxp_opensource_halimpl.git)
 - branch: ```topaz-SN100X-legacy```
 - dir: ```vendor/nxp/opensource/halimpl```

[AOSPA/android_vendor_nxp_opensource_hidlimp](https://github.com/AOSPA/android_vendor_nxp_opensource_hidlimp.git)
 - branch: ```topaz-SN100X-legacy```
 - dir: ```vendor/nxp/opensource/hidlimp```

[pa-lahaina/android_hardware_qcom_display](https://github.com/pa-lahaina/android_hardware_qcom_display)
 - branch: ```topaz-888```
 - dir: ```hardware/qcom/display```

[pa-lahaina/android_vendor_qcom_opensource_recovery-ext](https://github.com/pa-lahaina/android_vendor_qcom_opensource_recovery-ext)
 - branch: ```topaz```
 - dir: ```vendor/qcom/opensource/recovery-ext```

[EndCredits/clang-crepuscular](https://gitlab.com/EndCredits/clang-crepuscular)
 - branch: ```main```
 - dir: ```prebuilts/clang/host/linux-x86/clang-hana```

[pa-lahaina/android_device_xiaomi_sm8350-common](https://github.com/pa-lahaina/android_device_xiaomi_sm8350-common)
 - branch: ```topaz-wip```
 - dir: ```device/xiaomi/sm8350-common```

[pa-lahaina/android_kernel_xiaomi_sm8350](https://github.com/pa-lahaina/android_kernel_xiaomi_sm8350)
 - branch: ```topaz```
 - dir: ```kernel/xiaomi/sm8350```
 - note: KernelSU Submodule needs to be initlized

[pa-lahaina/android_vendor_xiaomi_sm8350-common](https://github.com/pa-lahaina/android_vendor_xiaomi_sm8350-common)
 - branch: ```topaz-wip```
 - dir: ```vendor/xiaomi/sm8350-common```

**renoir device-specific repositories:**

[pa-lahaina/android_device_xiaomi_renoir](https://github.com/pa-lahaina/android_device_xiaomi_renoir)
 - branch: ```topaz-wip```
 - dir: ```device/xiaomi/renoir```

[EndCredits/android_vendor_xiaomi_renoir](https://gitlab.com/EndCredits/android_vendor_xiaomi_renoir)
 - branch: ```topaz-wip```
 - dir: ```vendor/xiaomi/renoir```

[EndCredits/android_vendor_xiaomi-firmware_renoir](https://github.com/EndCredits/android_vendor_xiaomi-firmware_renoir)
 - branch: ```stable```
 - dir: ```vendor/xiaomi-firmware/renoir```
 - required: git-lfs

### What used common components

```makefile
# QTI
TARGET_COMMON_QTI_COMPONENTS := \
    adreno \
    alarm \
    audio \
    av \
    bt \
    gps \
    init \
    display \
    media \
    nfc \
    overlay \
    telephony \
    usb \
    wfd \
    wlan \
    perf
```

I think we need to modify some fields of vibraor HAL to support other xiaomi lahaina devices, so no switching to generic vibraor components

### What blobs decommonlized

- ADSP modules
- Audio Calibration DataBase (ACDB) blobs
- Audio HAL blobs
- Audio Configurations
- Audio Firmwares
- Battery Crypology blobs
- Camera blobs
- Display calibrations
- Fingerprint blobs
- NFC configs
- Sensors blobs && configs
- Thermal config 
- Touchscreen firmwres
- Vibrator effect firmwares