# 💻 VMware Setup Guide (Windows & Mac)

This guide will help you set up **VMware Workstation** (Windows) or **VMware Fusion** (Mac) and install virtual machines for:

- 🪟 Windows 10  
- 🐉 Kali Linux  
- 🪟 Windows 7 (for legacy/security lab use)

---

## 🧰 Requirements

- 8GB RAM minimum (16GB+ recommended)
- At least 60GB free disk space
- Internet connection
- Admin privileges on your computer

---

## 🪟 Installing VMware on Windows

### 1. Download VMware Workstation Player
- Go to: [VMware Workstation Player Download](https://www.vmware.com/products/workstation-player.html)
- Download the **Windows version**
- Run the installer and follow the setup prompts

### 2. Enable Virtualization in BIOS (if needed)
- Restart your PC and enter BIOS/UEFI (usually `F2`, `DEL`, or `ESC`)
- Enable **Intel VT-x** or **AMD-V**
- Save and reboot

---

## 🍎 Installing VMware on Mac

### 1. Download VMware Fusion Player
- Go to: [VMware Fusion Player for Mac](https://www.vmware.com/products/fusion/fusion-evaluation.html)
- Create a free VMware account if needed
- Download **VMware Fusion Player (Free for personal use)**
- Open the `.dmg` file and install Fusion

> 💡 macOS 13+ may require giving VMware additional permissions in **System Settings > Privacy & Security**.

---

## 🛠️ Setting Up Virtual Machines

---

### 🪟 Setting Up Windows 10 VM

1. Download the Windows 10 ISO:  
   [https://www.microsoft.com/en-us/software-download/windows10ISO](https://www.microsoft.com/en-us/software-download/windows10ISO)

2. Open VMware and create a **New Virtual Machine**  
   - Choose: “Installer disc image file (ISO)”  
   - Select your `Win10.iso`

3. Choose settings:  
   - 2 CPUs  
   - 4GB RAM  
   - 60GB disk space

4. Finish setup and install Windows normally

---

### 🐉 Setting Up Kali Linux VM

Option 1: Use the **official VMware image**  
- Download from: [https://www.kali.org/get-kali/#kali-virtual-machines](https://www.kali.org/get-kali/#kali-virtual-machines)

Steps:
1. Download the **Kali VMware 64-bit image** (preconfigured)
2. Extract the `.7z` file using [7-Zip](https://www.7-zip.org/)
3. Open the `.vmx` file with VMware
4. Kali default login:  
   - Username: `kali`  
   - Password: `kali`

Option 2: Install from ISO (more control)  
- Download the ISO from the same page  
- Follow similar steps to Windows 10 setup

---

### 🪟 Setting Up Windows 7 VM (For Legacy Labs)

> ⚠️ Note: Windows 7 is end-of-life and should only be used for learning/testing purposes.

1. Download a Windows 7 ISO (look for a legitimate source or use one from MSDN, TechNet, or education partners)
2. Create a new virtual machine and point it to the ISO
3. Allocate:
   - 2 CPUs  
   - 2–4GB RAM  
   - 40GB disk space

4. Follow the setup process like a regular Windows install

---

## 📦 Tips

- 📁 **Snapshots**: Take snapshots before major changes so you can revert if something breaks.
- 🛡️ **Isolation**: Disable shared folders and drag-drop to keep malware contained inside VMs.
- 📶 **Networking**: Use "NAT" for general internet access, or "Host-only" for isolated labs.

---

## 🙋‍♂️ Need Help?

Feel free to open an issue or reach out if you get stuck. Screenshots or error messages help a lot!

---

> “Virtual machines are the safest way to break stuff while learning how to fix it.”

