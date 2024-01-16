![Wacom Driver Slim Installation Guide](icon.png)

# Wacom Driver Slim Installation Guide

## Introduction
This README provides a guide on how to install the Wacom tablet driver without the additional Wacom Center software. This slim installation is beneficial for users who prefer a lightweight driver setup or have limited system resources.

## Prerequisites
- Windows Operating System.
- Wacom tablet compatible with the driver version.
- Administrative privileges on your computer.

## Getting the Driver
1. Visit the [Wacom Drivers page](https://www.wacom.com/en/support/product-support/drivers).
2. Select your tablet model.
3. Download the appropriate driver for your operating system.

## Installation
1. Save the downloaded driver (e.g., `WacomTablet_6.4.4-3.exe`) to a known location on your system.
2. Create a `.bat` file named `InstallWacomDriver.bat` with the following content:
```bat
@echo off
:: Install Wacom driver without the Wacom Center
WacomTablet_6.4.4-3.exe /opt nowdc
```

## Running the Installation

1. Right-click InstallWacomDriver.bat and select 'Run as Administrator'.
2. If a User Account Control (UAC) prompt appears, click 'Yes' to allow the script to run with administrative privileges.
3. The installation will proceed without installing Wacom Center.

## Post-Installation
After installation, you may need to restart your computer. Once rebooted, you can connect your Wacom tablet and start using it right away.

## Support
For any issues during installation or use, refer to the Wacom Support page for further assistance.
