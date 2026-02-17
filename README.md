# VirtualBox & Ubuntu: Step-by-step guide

This repository explains how to install Oracle VirtualBox and set up an Ubuntu virtual machine (VM). It’s aimed at beginners who are learning Linux and want a safe environment to practice.

---

## 1. Prerequisites

- **Host OS:** Windows, macOS, or Linux
- **Hardware:** At least 8 GB RAM recommended, 20+ GB free disk space
- **Downloads:**
  - VirtualBox: https://www.virtualbox.org/wiki/Downloads
  - Ubuntu Desktop ISO (e.g., LTS version): https://ubuntu.com/download/desktop

---

## 2. Install VirtualBox

1. **Download VirtualBox**
   - Go to the VirtualBox downloads page.
   - Choose the installer for your host OS (Windows, macOS, or Linux).

2. **Run the installer**
   - Double-click the installer.
   - Accept the default options unless you have a specific reason to change them.
   - Approve any network or driver prompts.
   - Launch VirtualBox after installation.

---

## 3. Create a new Ubuntu virtual machine

1. **Start VirtualBox** and click **“New”**.
2. **Name and OS type**
   - **Name:** `Ubuntu-VM` (or anything you like)
   - **Type:** `Linux`
   - **Version:** `Ubuntu (64-bit)`
3. **Memory size (RAM)**
   - Recommended: **2048 MB (2 GB)** minimum, **4096 MB (4 GB)** if you have enough RAM.
4. **Hard disk**
   - Choose **“Create a virtual hard disk now”**.
   - Disk type: **VDI (VirtualBox Disk Image)**.
   - Storage: **Dynamically allocated**.
   - Size: **20 GB** or more.

Click **Create**.

---

## 4. Attach the Ubuntu ISO

1. Select your new VM and click **“Settings”**.
2. Go to **“Storage”**.
3. Under **Controller: IDE** (or SATA), click the empty optical drive.
4. On the right, click the disk icon and choose **“Choose a disk file…”**.
5. Select the downloaded Ubuntu ISO file.
6. Click **OK**.

---

## 5. Boot the VM and install Ubuntu

1. Select the VM and click **“Start”**.
2. The VM should boot from the Ubuntu ISO.
3. When prompted, choose **“Install Ubuntu”**.

Follow the installer steps:

- **Keyboard layout:** Choose your layout and test it.
- **Updates and other software:** You can leave defaults or enable updates/third-party software.
- **Installation type:** For a VM, **“Erase disk and install Ubuntu”** is safe (it only affects the virtual disk).
- **Timezone:** Select your region.
- **User account:**
  - Choose a **name**, **computer name**, **username**, and **password**.
  - Remember this password—you’ll use it with `sudo`.

Click **Install** and wait for the process to finish. Then **restart** the VM when prompted. If asked to remove the installation medium, just press **Enter**.

---

## 6. First boot and basic checks

After reboot:

1. Log in with the username and password you created.
2. Open a terminal:
   - Press `Ctrl + Alt + T` inside the VM.
3. Run basic commands:

```bash
