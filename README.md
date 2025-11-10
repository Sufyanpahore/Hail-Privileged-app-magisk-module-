# Hail PrivApp (Magisk Module)

A Magisk module that installs **Hail** (`com.aistra.hail`) as a **privileged system app** for faster and smoother performance on rooted Android devices.

Hail is an advanced app freezer and controller. By installing it as a privileged app, it gains system-level control similar to preloaded system utilities — eliminating the slow root calls and offering seamless freezing/unfreezing without using superuser commands.

---

## ⚙️ Features

- Installs Hail as a privileged system app (`/system/priv-app/Hail`)
- Grants necessary privileged permissions automatically  
- Works systemlessly through Magisk — no direct modification to /system  
- Faster and smoother app operations  
- No root prompt lag (since it doesn’t rely on su)  

---

## 🧩 Module Overview

This module places the Hail APK and permission configuration directly into your system partition in a systemless way, using Magisk’s overlay structure.



---

## 📦 Installation

1. Download the latest release ZIP from the [Releases](../../releases) section.  
2. Open **Magisk Manager** → **Modules** → **Install from storage**.  
3. Select `hail-privapp.zip`.  
4. Wait for the installation to complete, then reboot.  
5. Open **Hail** — Go to settings and select **System app - Disable** it should now work instantly in system mode without asking for root.

---

## 🧾 Permissions Granted

These permissions are granted automatically by the module:

```xml
<privapp-permissions package="com.aistra.hail">
    <permission name="android.permission.PACKAGE_USAGE_STATS"/>
    <permission name="android.permission.FORCE_STOP_PACKAGES"/>
    <permission name="android.permission.CHANGE_COMPONENT_ENABLED_STATE"/>
    <permission name="android.permission.MANAGE_APP_OPS_MODES"/>
</privapp-permissions> 
```


💡 Notes

Requires Magisk installed (tested with Magisk 26+).


🧠 Credits

Hail by [Aistra](https://github.com/aistra0528/Hail/blob/master/README_EN.md)

Module template and structure by the Android modding community

Systemization script and testing by [Sufyan Zahoor](https://github.com/Sufyanpahore)

