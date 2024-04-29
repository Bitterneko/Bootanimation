# bootanimation
A Custom Boot Animation for Android (Root Required!)

# Press (+ Release) to show more Bootanimation!

# How To Use It?
1. **Gain Root Access**: Ensure your device has been rooted. The rooting process can vary depending on your device and the Android version you're using. Typically, you would use tools like Magisk or SuperSU to gain root access.

2. **Move Boot Animation**: Move or copy the bootanimation.zip file to the system directory on your device. Usually, the boot animation is located in /system/media/. You can use a file manager app that supports root access to do this.

3. **Change Permissions**: Make sure the permissions of the bootanimation.zip file are correct. Typically, you'll need to set its permissions to 644 (rw-r--r--).

4. **Reboot**: After you've copied the bootanimation.zip file to the system directory and set its permissions, reboot your device. Upon reboot, your device should play the new boot animation.

# ADB Method
1. **Connect Device**: Connect your Android device to your computer via USB.

2. **Enable USB Debugging**: On your Android device, navigate to Settings > Developer Options, then enable USB debugging. If Developer Options are not visible, go to Settings > About phone, and tap on "Build number" multiple times until you see a message indicating that Developer Options are enabled.

3. **Open Command Prompt or Terminal**: Open a command prompt or terminal window on your computer.

4. **Navigate to ADB Directory**: Navigate to the directory where ADB is installed. If you haven't installed ADB, you can download it as part of the Android SDK Platform Tools package from the official Android developer website.

4. **Push Boot Animation**: Use the following command to push the bootanimation.zip file to the appropriate location on your device:
```
adb push path/to/bootanimation.zip /data/local/bootanimation.zip
```
5. **Set Permissions**: Set the correct permissions for the bootanimation.zip file using the following command
```
adb shell chmod 644 /data/local/bootanimation.zip
```
6. **Reboot Your Device**
```
adb reboot
```
**After the device reboots, it should play the new boot animation. Make sure the boot animation file is compatible with your device's screen resolution to avoid any issues. Additionally, be cautious when using ADB commands, as modifying system files incorrectly can cause problems with your device.**
