# WiFi Spammer Tool

![Bash](https://img.shields.io/badge/bash-v5.0%2B-blue) 
![License](https://img.shields.io/badge/license-MIT-green) 
![Platform](https://img.shields.io/badge/platform-Linux-lightgrey)

A powerful Bash script for creating multiple fake WiFi access points to test wireless network security and client behavior.

## 📝 Description

This tool creates multiple fake WiFi access points (APs) using your wireless interface in monitor mode. It can generate:
- Popular SSIDs from a predefined list
- Custom SSIDs from your own list
- Router-like SSIDs with random suffixes
- Completely random alphanumeric SSIDs
- Combinations of all the above modes

## ✨ Features

- Multiple spamming modes
- Random MAC address generation
- Automatic channel selection
- Clean network restoration on exit
- Interactive menu interface
- Combine different spamming modes
- Automatic monitor mode setup

## ⚙️ Requirements

- Linux system
- Bash (v5.0+)
- Wireless interface supporting monitor mode
- Root privileges
- `aircrack-ng` suite installed
- `iw` tool installed

## 📦 Installation

1. Install dependencies:
```bash
sudo apt update && sudo apt install -y aircrack-ng iw
```

2. Clone the repository:
```bash
git clone https://github.com/your-repo/wifi-spammer.git
cd wifi-spammer
```

3. Make the script executable:
```bash
chmod +x wifi_spammer.sh
```

## 🚀 Usage

1. Run the script as root:
```bash
sudo ./wifi_spammer.sh
```

2. Follow the on-screen instructions:
   - Select your wireless interface
   - Choose the spamming mode
   - Let it run (press Ctrl+C to stop)

## 📂 File Configuration

The script uses three text files for SSID sources:

1. `popular.txt` - Contains common/public WiFi names
2. `custom.txt` - For your custom SSIDs
3. `router.txt` - Contains router manufacturer prefixes

Edit these files to customize the generated access points.

## 🎛️ Modes

1. **Popular SSIDs** - Spams common WiFi names from `popular.txt`
2. **Custom SSIDs** - Uses your custom SSIDs from `custom.txt`
3. **Routers** - Generates router-like names (e.g., "TP-Link_AB123")
4. **Random** - Creates completely random alphanumeric SSIDs
5. **Combined** - Mixes all selected modes together

## ⚠️ Disclaimer

This tool is for **educational and testing purposes only**. Use it only on networks you own or have permission to test. The authors are not responsible for any misuse or illegal activities.

## 📜 License

MIT License - See [LICENSE](LICENSE) file for details.

## 💡 Tips

- For best results, use a wireless card that supports packet injection
- Combine with Wireshark or tcpdump to analyze client behavior
- The more SSIDs you generate, the more "noise" you create
- Some clients may automatically connect to familiar-looking SSIDs

Press Ctrl+C at any time to stop the spamming and restore your network interface.
