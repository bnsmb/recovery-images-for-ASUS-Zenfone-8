**Ugly TWRP images**

----
**Update 19.07.2025**

The new OS image for **/e/** for the **ASUS Zenfone 8** available here [https://images.ecloud.global/community/sake/](https://images.ecloud.global/community/sake/) are now based on the **LineageOS 22.x** (this is **Android 15**).

Unfortunately "ugly" TWRP images created for **LineageOS 22.x** based OS do not work anymore. Therefor there will be no more new ugly TWRP images for **/e/**.  

----

Since **LineageOS verison 20**, the **ASUS Zenfone 8** can no longer boot from the TWRP recovery images when the LineageOS is installed on the phone.

The TWRP images in this directory get around this issue.

The recovery images in this directory are **unofficial** TWRP images created using an unsupported method. These images should only be used for emergency tasks.

Using these TWRP images you can access the files in the **/data** partition while booted from the recovery image.

These TWRP images also support the decryption if the phone access is protected via PIN, password, or pattern.

Access to the phone via adb is possible if the phone has been booted from the TWRP image (even if adb access is not yet enabled in the phone's installed operating system).

Note that the TWRP GUI may not re-appear after it has been disabled due to the timeout. In this case, you can only use the phone via adb in this session.

To avoid this problem, deactivate the screen timeout in the TWRP settings.

---

The script used to create these TWRP images is also available in a github repoitory:  [https://github.com/bnsmb/scripts-for-Android/blob/main/scripts/create_ugly_twrp_image.sh](https://github.com/bnsmb/scripts-for-Android/blob/main/scripts/create_ugly_twrp_image.sh).

see [TWRP images for ASUS Zenfone 8 with /e/](http://bnsmb.de/My_HowTos_for_Android.html#TWRP_images_for_ASUS_Zenfone_8_with_e) for details

see [How to use TWRP if LineageOS 20.x is installed](http://bnsmb.de/My_HowTos_for_Android.html#How_to_use_TWRP_if_LineageOS_20.x_is_installed) for details and why these images should only be used if neccessary

See [How to create a TWRP image for LineageOS based ROMs using a script](http://bnsmb.de/My_HowTos_for_Android.html#How_to_create_a_TWRP_image_for_LineageOS_based_ROMs_using_a_script) for details about the script used to create these images.

The /e/ OS images for the **ASUS Zenfone 8** are available here: [https://images.ecloud.global/community/sake/](https://images.ecloud.global/community/sake/)


---

**WARNING**

**Do not use the TWRP images mentioned in this post if the OS installed on the phone is not the correct OS or not the correct OS version!**

If you have accidentally booted the wrong TWRP image and the phone only displays the ASUS logo, simply press the buttons for **Volume down**, **Volume up**, and **Power** simultaneously for at least 10 seconds to poweroff or reboot the phone.

These TWRP images should only be used to boot the phone using the fastboot command, example:

```
fastboot boot twrp-e-2.7-t-20250112460975-community-sake.img
```

**Do NOT install this TWRP into the boot partition!**

**Use at your own risk!**

---

The TWRP images in this directory are:

| TRWP image file | OS | OS version | Android version | comment |
| ---| ---| ---| ---| ---|
| twrp-e-2.5-t-20241108446630-community-sake.img | /e/ |	2.5.1	| Android 13 | | 
| twrp-e-2.6.3-t-20241217455572-community-sake.img	| /e/ | 2.6.3	| Android 13 | | 
| twrp-e-2.7-t-20250112460975-community-sake.img	| /e/ | 2.7	| Android 13 | | 
| twrp-e-2.8-t-20250219470166-community-sake.img | /e/ | 2.8 | Android 13 | |
| twrp-e-2.9-t-20250322478412-community-sake.img | /e/ | 2.9 | Android 13 | | 
| twrp-e-3.0-t-20250529496537-community-sake.img | /e/ | 3.0 | Android 13 | | 
| twrp-e-3.0.1-t-20250607498934-community-sake.img | /e/ | 3.0.1 | Android 13 |
| twrp-e-3.0.4-t-20250710507809-community-sake.img | /e/ | 3.0.4 | Android 13 |


---
