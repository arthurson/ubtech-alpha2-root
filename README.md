# ubtech-alpha2-root
it only works on android 5.1 with rk3288 cpu system, earlier android 4.4 with samsung cpu system can't be used.

there are mainly 2 firmware for alpha2, one is for alpha2 and other is for lynx/qrobot, both can be rooted with this method.

while alpha2 firmware is more pure asop style, lynx/qrobot add many background service from amazon/tencent. both image dump has been added here for backup perference.

magisk v25.2 is the last one to support android 5.1, you can download it here.
https://github.com/topjohnwu/Magisk/releases/tag/v25.2

after you rooted the alpha2, you have to use these commands to delele bulit-in  AOSP debug su.

adb root
adb remount
adb shell rm /system/xbin/su
