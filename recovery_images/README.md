
***Warning: All recovery images in this repository are unofficial, self-compiled images***

***Use at your own risk!***

---

***OrangeFox-Unofficial-I006D-2024-09-12.img.zip***

***OrangeFox-Unofficial-I006D-2024-09-12.zip***

This an [OrangeFox recovery](https://wiki.orangefox.tech) image for the **ASUS Zenfone 8**.

The source files for the ***OrangeFox recovery*** were checked out ***10.09.204***.

The image was compiled with these custom build vars:

```
export FOX_REPLACE_BUSYBOX_PS=1
export FOX_REPLACE_TOOLBOX_GETPROP=1
export FOX_USE_TAR_BINARY=1
export FOX_USE_SED_BINARY=1
export FOX_USE_ZIP_BINARY=1
export FOX_USE_NANO_EDITOR=1
export FOX_USE_BASH_SHELL=1

export OF_USE_MAGISKBOOT=1
export OF_USE_MAGISKBOOT_FOR_ALL_PATCHES=1
export FOX_DISABLE_APP_MANAGER=0

export FOX_DELETE_AROMAFM=1

export TARGET_DEVICE_ALT="gssi,ASUS_I006D"
```

see [https://gitlab.com/OrangeFox/vendor/recovery/-/blob/master/orangefox_build_vars.txt](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/master/orangefox_build_vars.txt) for a description of the custom build vars

see [https://wiki.orangefox.tech](https://wiki.orangefox.tech) for infos about the OrangeFox recovery

see [https://bnsmb.de/My_HowTos_for_Android.html#How_to_compile_the_OrangeFox_Recovery_for_the_ASUS_Zenfone_8](https://bnsmb.de/My_HowTos_for_Android.html#How_to_compile_the_OrangeFox_Recovery_for_the_ASUS_Zenfone_8)


---
	
***twrp-3.7.0_12-0-I006D-with_Android14_support.img.zip***
	

This is an TWRP image for the **ASUS Zenfone 8**.

The source files for this TWRP image were checked out on **25.11.2023**.

There are additional properties defined in this image:

additional properties in the image:
```
ASUS_I006D:/ # getprop  | grep android_version
[ro.product.bootimage.supported_android_version]: [14]
[ro.product.odm.supported_android_version]: [14]
[ro.product.product.supported_android_version]: [14]
[ro.product.system_ext.supported_android_version]: [14]
[ro.product.vendor.supported_android_version]: [14]
ASUS_I006D:/ # 
```

***Note***

There is now an official new TWRP version for ASUS Zenfone 8 with Android 14 support: [TWRP version 3.7.0.12-1](https://eu.dl.twrp.me/I006D/twrp-3.7.0_12-1-I006D.img.html)


---

***twrp-3.7.0_12-0-I006D-with_Android14_support_and_tools.img.zip***

This is the TWRP image ***twrp-3.7.0_12-0-I006D-with_Android14_support.img*** for the **ASUS Zenfone 8** with these additional binaries:

```
ASUS_I006D:/ # ls -l /system/bin/ed system/bin/gawk /system/bin/gdisk /system/bin/parted /system/bin/sqlite3 /system/bin/vi/system/xbin
-rwxrwxrwx 1 root root  744128 2023-11-26 09:08 /system/bin/ed
-rwxrwxrwx 1 root root  680612 2023-11-26 09:08 /system/bin/gdisk
-rwxrwxrwx 1 root root  470788 2023-11-26 09:08 /system/bin/parted
-rwxrwxrwx 1 root root 1714720 2023-11-26 09:08 /system/bin/sqlite3
-rwxrwxrwx 1 root root 4127280 2023-11-26 09:09 /system/bin/vi
-rwxrwxrwx 1 root root 1777096 2023-11-26 09:08 system/bin/gawk

/system/xbin:
total 4500
-rwxrwxrwx 1 root root  938296 2023-11-26 09:06 cpio
-rwxrwxrwx 1 root root  960496 2023-11-26 09:06 find
-rwxrwxrwx 1 root root 1486120 2023-11-26 09:06 grep
-rwxrwxrwx 1 root root 1216256 2023-11-26 09:06 tar
ASUS_I006D:/ #
```
This image also defines these two new properties:

```
ASUS_I006D:/ # getprop ro.product.type
enhanced
ASUS_I006D:/ #

ASUS_I006D:/ # getprop ro.source_checkout_date
2023-11-25
ASUS_I006D:/ #
```

---

***twrp-3.7.0_12-1-I006D-enhanced.img.zip***

This is a copy of the official ***twrp-3.7.0_12-1-I006D.img*** for the **ASUS Zenfone 8** with some additional files:

```
ASUS_I006D:/system/bin # pwd
/system/bin
ASUS_I006D:/system/bin # ls -l bootctl* lp* ed gawk gdisk parted sqlite3 vi* /system/xbin

-rwxr-x--- 1 root root   34112 2024-01-10 19:54 bootctl
-rwxr-x--- 1 root root   19832 2024-01-10 19:54 bootctl.bin
-rwxr-xr-x 1 root root  744128 2024-01-10 19:54 ed
-rwxr-xr-x 1 root root 1777096 2024-01-10 19:54 gawk
-rwxr-xr-x 1 root root  680612 2024-01-10 19:54 gdisk
-rwxr-xr-x 1 root root   19872 2024-01-10 19:54 lpdump
-rwxr-xr-x 1 root root   31424 2024-01-10 19:54 lpdumpd
-rwxr-xr-x 1 root root  100712 2024-01-10 19:54 lptools
-rwxr-xr-x 1 root root  470788 2024-01-10 19:54 parted
-rwxr-xr-x 1 root root 1714720 2024-01-10 19:54 sqlite3
-rwxr-xr-x 1 root root 4127280 2024-01-10 19:54 vi

/system/xbin:
total 4500
-rwxr-xr-x 1 root root  938296 2024-01-10 19:54 cpio
-rwxr-xr-x 1 root root  960496 2024-01-10 19:54 find
-rwxr-xr-x 1 root root 1486120 2024-01-10 19:54 grep
-rwxr-xr-x 1 root root 1216256 2024-01-10 19:54 tar
ASUS_I006D:/system/bin #  
```
see [How to add additional files to an TWRP image](http://bnsmb.de/My_HowTos_for_Android.html#How_to_add_additional_files_to_an_TWRP) for how to add additional files to a TWRP image

---


***twrp_3.7.1.12-1_ASUS_Zenfone8_2024-12-02_extended.img.zip***
	

This is a TWRP image for the **ASUS Zenfone 8** with additional binaries

The source files for this TWRP image were checked out on **10.09.2024**.

Additional binaries and files in the image are:

```
-rwxr-xr-x 1 root   root    628616 2024-08-12 09:20 system/bin/bmore
-rwxr-xr-x 1 root   root    824328 2024-08-12 09:20 system/bin/bvi
-rwxr-xr-x 1 root   root     99160 2024-09-07 00:15 system/bin/dmctl
-rwxr-xr-x 1 system system  744128 2024-08-10 01:30 system/bin/ed
-rwxr-xr-x 1 system system 1777096 2024-08-10 01:30 system/bin/gawk
-rwxr-xr-x 1 system system  680612 2024-08-10 01:30 system/bin/gdisk
-rwxr-xr-x 1 root   root    999064 2022-08-18 11:41 system/bin/lpadd
-rwxr-xr-x 1 root   root   1907128 2022-08-18 11:45 system/bin/lpdump
-rwxr-xr-x 1 root   root    969144 2022-08-18 11:45 system/bin/lpmake
-rwxr-xr-x 1 root   root    606704 2023-01-25 04:31 system/bin/make_ext4fs
-rwxr-xr-x 1 system system  470788 2024-08-10 01:30 system/bin/parted
-rwxr-xr-x 1 system system 1714720 2024-08-10 01:30 system/bin/sqlite3
lrwxrwxrwx 1 root   root         5 2024-08-12 09:21 system/bin/vi -> ./vim
lrwxrwxrwx 1 root   root         5 2024-08-12 09:21 system/bin/vi -> ./vim
lrwxrwxrwx 1 root   root         5 2024-08-12 09:21 system/bin/view -> ./vim
-rwxr-xr-x 1 root   root        59 2024-09-10 10:52 system/bin/vim
lrwxrwxrwx 1 root   root         5 2024-08-12 09:21 system/bin/vimdiff -> ./vim
-rw-r--r-- 1 root   root    387592 2024-08-10 07:34 system/lib64/libncursesw.so.6
-rw-rw-rw- 1 root   root         0 2024-08-10 07:44 system/usr/share/vim/vim91/defaults.vim
-rwxr-xr-x 1 system system  938296 2024-08-10 01:31 system/xbin/cpio
-rwxr-xr-x 1 system system  960496 2024-08-10 01:31 system/xbin/find
-rwxr-xr-x 1 system system 1486120 2024-08-10 01:31 system/xbin/grep
-rwxr-xr-x 1 system system 1216256 2024-08-10 01:31 system/xbin/tar
```


This image also defines these two new properties:

```
ASUS_I006D:/ # getprop ro.product.type
enhanced
ASUS_I006D:/ #

ASUS_I006D:/ # getprop ro.source_checkout_date
2024-09-10
ASUS_I006D:/ #

ASUS_I006D:/ # getprop ro.image_create_date
2024-12-02
ASUS_I006D:/ #
```

Check [https://gerrit.twrp.me/](https://gerrit.twrp.me/) for a list of changes in the source code

**Update 21.02.2025**

There is a bug in this TWRP image, so it could not be used to install TWRP on the boot partition. This bug is fixed in the new version of the image. 

---

***twrp_3.7.1.12-1_ASUS_Zenfone8_2025-02-21_extended.img***

This is a TWRP image for the **ASUS Zenfone 8** with additional binaries

The source files for this TWRP image were checked out on **10.09.2024**.

Additional binaries and files in the image are:

The additional binaries in this image are

    GNU ed 1.18
    GPT fdisk (gdisk) version 1.0.3
    parted (GNU parted) 3.2
    sqlite3 3.39.3 2022-09-05
    VIM - Vi IMproved 9.1 Included patches: 1-672
    GNU Awk 5.2.0, API 3.2, PMA Avon 7
    cpio (GNU cpio) 2.12
    dd (coreutils) 9.5.58-83ec7
    find (GNU findutils) 4.9.0
    grep (GNU grep) 3.8
    gsed (GNU sed) 4.8
    gzip 1.13
    less 643 (POSIX regular expressions)
    tar (GNU tar) 1.34
    GNU bash, version 5.2.0(1)-release (aarch64-unknown-linux-gnu)
    bvi 1.4.1
    bmore 1.4.1
    dmctl
    lpadd
    lpdump
    lpmake
    make_ext4fs
    lputil (from [https://www.temblast.com/lputil.html](https://www.temblast.com/lputil.html))

(The new versions of the binary files already present in the TWRP image are located in the directory **/system/xbin**.)

There are some new properties defined in this image:

```
ASUS_I006D:/ # getprop ro.product.type
enhanced
ASUS_I006D:/ #
            
ASUS_I006D:/ # getprop ro.source_checkout_date
2024-09-10
ASUS_I006D:/ #
            
ASUS_I006D:/ # getprop ro.image_create_date
2025-02-21
ASUS_I006D:/ #
```

---

The recovery images in the directory **ugly_images** are unofficial TWRP images created using an unsupported method. These images should only be used for emergency tasks.

see [How to use TWRP if LineageOS 20.x is installed](http://bnsmb.de/My_HowTos_for_Android.html#How_to_use_TWRP_if_LineageOS_20.x_is_installed) for details and why these images should only be used if neccessary

See [How to create a TWRP image for LineageOS based ROMs using a script](http://bnsmb.de/My_HowTos_for_Android.html#How_to_create_a_TWRP_image_for_LineageOS_based_ROMs_using_a_script) for details about the script used to create these images.

---



 

