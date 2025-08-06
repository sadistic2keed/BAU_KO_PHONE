# 🚀 BAU KO PHONE - Android Exploitation Toolkit

An advanced all-in-one hacking framework written in `Python` for remotely exploiting Android devices using `ADB` (Android Debug Bridge) and `Metasploit-Framework`.

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)](CONTRIBUTING.md)

</div>

## 🔥 Features

### Core Capabilities

- **One-Click Meterpreter Session**: Fully automated payload creation, installation, and execution
- **ADB Toolkit**: Comprehensive suite for Android device management
- **Cross-Platform**: Works on Windows, Linux, and macOS
- **WiFi & USB Support**: Connect to devices via both wireless and wired connections

### Exploitation Features

- **Remote Code Execution**
- **Data Exfiltration** (Files, SMS, Contacts, Call Logs)
- **Real-time Device Control** (Screen mirroring, input injection)
- **Persistence Mechanisms**
- **Metasploit Integration** for advanced post-exploitation

### Device Management

- 📸 Screenshot capture & automatic download
- 🎥 Screen recording with configurable duration
- 📁 File system exploration and transfer
- 📱 App management (install/uninstall/launch)
- 🔄 Advanced reboot options (recovery, bootloader)

# Requirements  
* [`python3`](https://www.python.org/) : Python 3.10 or Newer
* [`pip`](https://pip.pypa.io/en/stable/installation/) : Package installer for Python
* [`adb`](https://developer.android.com/studio/command-line/adb) : Android Debug Bridge (ADB) from `Android SDK Platform Tools`
* [`metasploit-framework`](https://www.metasploit.com/) : Metasploit-Framework (`msfvenom` and `msfconsole`)
* [`scrcpy`](https://github.com/Genymobile/scrcpy) : Scrcpy
* [`nmap`](https://nmap.org/) : Nmap

## DOWNLOAD REQUIREMENTS (LINUX ONLY)
``` bash 
# Update & Upgrade system
sudo apt update && sudo apt full-upgrade -y

# Install Python 3 and pip
sudo apt install -y python3 python3-pip

# Verify Python version (needs to be 3.10+)
python3 --version

# Install ADB (Android Debug Bridge)
sudo apt install -y android-tools-adb android-tools-fastboot

# Install Metasploit Framework
sudo apt install -y metasploit-framework

# Install scrcpy (for Android screen mirroring/control)
sudo apt install -y scrcpy

# Install Nmap
sudo apt install -y nmap
```

## VERIFY DOWNLOAD

```bash 
python3 --version
pip3 --version
adb version
msfconsole --version
scrcpy --version
nmap --version
```
## 👷‍⚖️ Installation

```bash
git clone https://github.com/sadistic2keed/bau_ko_phone.git
cd bau_ko_phone
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
python niqqachu.py
```
# Tutorial


## Setting up Android Phone for the first time

* __Enabling the Developer Options__

1. Open `Settings`.
2. Go to `About Phone`.
3. Find `Build Number`.
4. Tap on `Build Number` 7 times.
5. Enter your pattern, PIN or password to enable the `Developer options` menu.
6. The `Developer options` menu will now appear in your Settings menu.

* __Enabling USB Debugging__

1. Open `Settings`.
2. Go to `System` > `Developer options`.
3. Scroll down and Enable `USB debugging`.

* __Connecting with Computer__

1. Connect your Android device and `adb` host computer to a common Wi-Fi network.
2. Connect the device to the host computer with a USB cable.
3. Open a terminal in the computer and enter the following command :
```
adb devices
```
4. A pop-up will appear in the Android phone when you connect your phone to a new PC for the first time : `Allow USB debugging?`.
5. Click on `Always allow from this computer` check-box and then click `Allow`.
6. Then in the terminal enter the following command :
```
adb tcpip 5555
```
7. Now you can connect the Android Phone with the computer over Wi-Fi using `adb`.
8. Disconnect the USB cable.
9. Go to `Settings` >  `About Phone` > `Status` > `IP address` and note the phone's `IP Address`.
10. Run BAU_KO_PHONE and select `Connect a device` and enter the target's `IP Address` to connect over Wi-Fi.



## Connecting the Android phone for the next time

1. Connect your Android device and host computer to a common Wi-Fi network.
2. Run __PhoneSploit Pro__ and select `Connect a device` and enter the target's `IP Address` to connect over Wi-Fi.

