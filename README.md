# flip2
Most info is currently in [the wiki](https://github.com/neutronscott/flip2/wiki)


# Tutorial for Setting Up Your Device

## Known Compatible Models:

- 4058C
- 4058W
- T408DL

**TCL Flip 2** and **TCL Classic** are known compatible.

## Step 1: Flashing the Boot Image

1. **Utilize the Flip2 Repository**
   - Follow [the wiki instructions](https://github.com/neutronscott/flip2/wiki) to flash the new boot image.

2. **Windows PC Requirement**
   - You *must* use a Windows PC for this process. Linux has been tried but did not work as well.
   - The boot image will work unless your device has a recent firmware with OEM locks preventing sideloading.

3. **Magisk Option**
   - After installing the boot image, you can choose whether or not to use Magisk. Either option will enable offline app installs.

## Step 2: Optimizing Your Device

1. **Enable USB Debugging**
   - Not much you can do without it.
   - Enter `*#*#33284#*#*` `(*#*#DEBUG#*#*)` to enable USB Debugging.
   - Likewise, use `*#*#217703#*#*` to bring up your Applications menu (Won't be needed after Step 4).

3. **Install Stable Mouse Service**
   - Recommended: **Simple Mouse** (it is more stable and less prone to crashes).
   - [Get it here.](https://github.com/neutronscott/flip2/releases/download/simple-release1/mouse)
   - Download [Mouse V2](https://github.com/neutronscott/flip2/releases/download/v2/vMouse2.zip) and pack the executable into the zipfile, flash it with Magisk.

4. **Install Niagara Launcher**
   - Download and install [Niagara Launcher](https://niagaralauncher.com/).
   - It supports the device’s keypad well and offers extensive customization.

5. **Enhance Typing with Traditional T9**
   - Install **Traditional T9** from [Sspanak](https://github.com/sspanak/tt9) for a better typing experience compared to the default keyboard.

6. **Debloat Your System**
   - Use [Universal Android Debloater (UAD)](https://github.com/0x192/universal-android-debloater) to remove unnecessary apps.
   - Consider removing:
     - `com.android.launcher3` (the stock launcher, which you won’t need)
     - `com.tct.os.omadm` (the system updater)
   - Feel free to remove other apps, but retain essential system apps such as messaging, calling, and notes unless you have suitable replacements.

## Step 3: Setting Up Activity Launcher Shortcuts

1. **Install Activity Launcher**
   - Download Activity Launcher from [F-Droid](https://f-droid.org/en/packages/de.szalkowski.activitylauncher/).
   - This app is essential for setting up shortcuts.

2. **Create a Shortcut for Recent Apps**
   - **Name:** Recents (or customize as you like)
   - **Package:** `com.android.systemui`
   - **Class:** `com.tcl.recents.RecentsListActivity`
   - **Icon:** Use `com.android.systemui:drawable/icon` (or your chosen icon)

3. **Create a Shortcut for Notifications**
   - **Name:** Notifications (or a custom name)
   - **Package:** `com.android.systemui`
   - **Class:** `com.tcl.recents.NotificationActivity`
   - **Icon:** Use `com.android.systemui:drawable/icon` (or another preferred icon)

4. **Place Shortcuts on Home Screen**
   - Use the “Create Shortcut” option in Activity Launcher to add both shortcuts to your home screen.
