# ubtech-alpha2-root
it only works on android 5.1 with rk3288 cpu system, earlier android 4.4 with samsung cpu system can't be used.

there are mainly 2 firmware for alpha2, one is for alpha2 and other is for lynx/qrobot, both can be rooted with this method.

while alpha2 firmware is more pure asop style, lynx/qrobot add many background service from amazon/tencent. both image dump has been added here for backup perference.


right click RKDevTool.exe and use admin to run.
you will see ADB device below if you connect to the working robot.

press 切換 switch to roboot the roboit, it will become loader mode.


<img width="970" height="461" alt="image" src="https://github.com/user-attachments/assets/a50b8e51-55ac-4784-b902-da0dbcb7a7c5" />


press 設備分類表 to renew the image address

<img width="970" height="461" alt="image" src="https://github.com/user-attachments/assets/9862a560-46d5-4751-82bf-0dffe96f8faa" />

you can see only boot.img is clicked.
then click 強制按地址寫 below, and press 執行 to run to software

<img width="970" height="461" alt="image" src="https://github.com/user-attachments/assets/a6a43d6e-3311-4007-a93e-05fce345527a" />

if the robot reboot normally, it means your alpha2 has been root.

if your roboot just flash head led and nothing more, something bad happen to your robot, open image folder, delete boot.img, rename orginal.boot.img to boot.img, and redo the above steps, it can reinstall official boot.img to robot, then it should run again.

if you want to install magisk, v25.2 is the last one to support android 5.1, you can download it here.
https://github.com/topjohnwu/Magisk/releases/tag/v25.2

you might see abnormal status, as there are 2 su in your system, you have to use these commands to delele bulit-in  AOSP debug su.

adb root
adb remount
adb shell rm /system/xbin/su


<img width="476" height="664" alt="image" src="https://github.com/user-attachments/assets/18f381e7-27dd-496f-be0c-9262b7b0a2b2" />
