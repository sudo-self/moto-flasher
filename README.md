# moto-flasher mac & linux

This is a minimal shell script for flashing Motorola firmware (`.xml` and `.img` files) using `fastboot`, designed to work on **macOS** and **Linux**. Inspired by RootJunky, adapted and repackaged by **sudo-self**.

---

## 🚀 Features# moto-flasher (macOS & Linux)

This is a minimal shell script for flashing Motorola firmware (`.xml` and `.img` files) using `fastboot`, designed to work on **macOS** and **Linux**.  
Inspired by RootJunky, adapted and repackaged by **sudo-self**.

---

## 🚀 Features

- No installation required.
- Supports `.xml` flash scripts from Motorola firmware packages.
- Automatically validates file checksums (`MD5`).
- Compatible with both **macOS** and **Linux**.
- Does **not** require an unlocked bootloader to flash **official stock firmware**.

---

## 📁 File Structure

Place the following files in the **same directory**:

```
moto-flasher/
├── flash.sh              # The main script
├── servicefile.xml       # XML script from Motorola firmware
├── *.img                 # Image files referenced in XML
├── files/
│   ├── adblinux
│   ├── adbosx
│   ├── fastbootlinux
│   └── fastbootosx
```

> 🧠 **Note:** The `files/` folder must include platform-specific `adb` and `fastboot` binaries.

---

## 🧪 Requirements

- `bash` or `sh` terminal
- Motorola firmware package with `.xml` and `.img` files
- USB cable and Motorola device
- Script permissions:  
  ```bash
  chmod +x flash.sh
  ```

---

## ⚙️ Before You Begin

1. Power off your Motorola device.
2. Boot into **fastboot mode**:  
   - Hold **Power + Volume Down** until the fastboot screen appears.
3. **No bootloader unlock required** to flash **stock firmware** from Motorola.

---

## 🛠️ Usage

1. **Download & extract** your Motorola firmware package.
2. **Place** the `.xml` script and all referenced `.img` files in the same folder as `flash.sh`.
3. **Make the script executable**:
   ```bash
   chmod +x flash.sh
   ```
4. **Run the script** with the XML file:
   ```bash
   ./flash.sh servicefile.xml
   ```
5. Follow the prompts to complete the flash process.

---

## ⚠️ Warnings

- The script will **abort if MD5 checks fail**.
- Flashing firmware may **erase user data**.
- Do not disconnect the device or interrupt the process.

---

## 🤝 Credits

RSD enhanced by **sudo-self**

> Built with simplicity in mind. Flash safely.





