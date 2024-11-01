![Wacom Driver Slim Installation Guide](icon.png)

# Wacom Driver Slim Installation Guide

## Introduction
This README provides a guide on how to install the Wacom tablet driver without the additional Wacom Center software. This slim installation is beneficial for users who prefer a lightweight driver setup or have limited system resources.

## Prerequisites
- Windows or macOS operating system.
- Wacom tablet compatible with the driver version.
- Administrative privileges on your computer.

## Getting the Driver
1. Visit the [Wacom Drivers page](https://www.wacom.com/en/support/product-support/drivers).
2. Select your tablet model.
3. Download the appropriate driver for your operating system.

---

## Installation

### Windows

1. Save the downloaded driver (e.g., `WacomTablet_6.4.4-3.exe`) to a known location on your system.
2. Create a `.bat` file named `InstallWacomDriver.bat` with the following content:

    ```bat
    @echo off
    :: Install Wacom driver without the Wacom Center
    WacomTablet_6.4.4-3.exe /opt nowdc
    ```

3. Right-click `InstallWacomDriver.bat` and select 'Run as Administrator'.
4. If a User Account Control (UAC) prompt appears, click 'Yes' to allow the script to run with administrative privileges.
5. The installation will proceed without installing Wacom Center.

### macOS

1. Save the downloaded `.dmg` driver file (e.g., `WacomTablet_6.4.7-2.dmg`) to your desktop.
2. Open the Terminal and execute the following commands:

    ```bash
    # Mount the .dmg file
    hdiutil attach ~/Desktop/WacomTablet_6.4.7-2.dmg
    ```

3. Once the image is mounted, install the driver package using:

    ```bash
    sudo installer -pkg "/Volumes/WacomTablet/Install Wacom Tablet.pkg" -target /
    ```

4. After installation, unmount the image:

    ```bash
    hdiutil detach /Volumes/WacomTablet
    ```

---

## Post-Installation
After installation, you may need to restart your computer. Once rebooted, you can connect your Wacom tablet and start using it right away.

## Support
For any issues during installation or use, refer to the Wacom Support page for further assistance.
