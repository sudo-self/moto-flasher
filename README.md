# moto-flasher mac & linux

This is a minimal shell script for flashing Motorola firmware (`.xml` and `.img` files) using `fastboot`, designed to work on **macOS** and **Linux**. Inspired by RootJunky, adapted and repackaged by **sudo-self**.

---

## 🚀 Features

- No installation required.
- Supports `.xml` flash scripts from Motorola firmware packages.
- Automatically validates file checksums (`MD5`).
- Compatible with both **macOS** and **Linux**.

---

## 📁 File Structure

Place the following in the same folder:


> 🧠 **Note:** `files/` folder is required and must include `adb` and `fastboot` binaries for your platform.

---

## 🧪 Requirements

- `bash` or `sh` terminal
- Motorola firmware with `.xml` script
- Executable permissions: `chmod +x flash.sh`

---

## 🛠️ Usage

1. **Download and extract** your Motorola firmware.

2. **Place** the extracted `.xml` and all referenced `.img` files in the same folder as this script.

3. Make the script executable:

   ```
   chmod +x flash.sh
   ```
4. flash the device:
   
   ```
   ./flash.sh servicefile.xml
   ```



