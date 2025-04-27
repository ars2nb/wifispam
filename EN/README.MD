# WiFi Spammer Tool || US  

![Bash](https://img.shields.io/badge/bash-v5.0%2B-blue)  
![License](https://img.shields.io/badge/license-MIT-green)  
![Platform](https://img.shields.io/badge/platform-Linux-lightgrey)  

A script for creating multiple fake WiFi access points with custom SSIDs  

## 📝 Description  

This tool generates numerous fake WiFi access points for wireless security testing.  
Key features:  
- Predefined SSIDs of popular American networks  
- Common US router prefixes  
- Multiple operation modes  
- Automatic network recovery  

## ⚙️ Requirements  

- Linux OS  
- Wireless adapter supporting monitor mode  
- Root access  
- Packages: `aircrack-ng`, `iw`  

## 📦 Installation  

1. Install dependencies:  
```bash  
sudo apt update && sudo apt install -y aircrack-ng iw  
```  

2. Download the script:  
```bash  
git clone https://github.com/ars3nb/wifispam/US.git  
cd US  # American version  
```  

3. Make it executable:  
```bash  
chmod +x wifi_spammer.sh  
```  

## 🚀 Usage  

Run with root privileges:  
```bash  
sudo ./wifi_spammer.sh  
```  

Follow on-screen instructions. Press Ctrl+C to stop.  

## 📂 Configuration Files  

- `popular.txt` – popular American SSIDs (e.g., "McDonald's FREE WIFI", "attwifi")  
- `router.txt` – common US router prefixes (e.g., "NETGEAR", "Linksys")  
- `custom.txt` – your custom SSIDs  

## ⚠️ Important  

For educational purposes and authorized penetration testing only!  

## American Version Specifics  

- All SSIDs in `popular.txt` and `router.txt` are optimized for US networks  
- Includes common American ISP naming conventions  
- Supports FCC-compliant channel selection
