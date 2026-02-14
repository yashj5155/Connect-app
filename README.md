# 🎥 Connect – WiFi Stream Viewer (Android APK)
#Best work with our WiFi File Share App (Windows)#
A lightweight Android application that automatically discovers and connects to local network video streams running on port **5000**.

Connect instantly using:
- 🔍 Automatic Network Scan
- 📷 QR Code Scan
- ⌨ Manual IP Entry

---

## 🚀 Overview

**Connect** is designed to simplify accessing local camera streams hosted on a WiFi network.

Instead of manually typing IP addresses or troubleshooting connections, this app allows you to:

- Scan your network for active streaming servers
- Scan a QR code to connect instantly
- Enter an IP address manually as fallback
- View live stream inside the app
- Switch to fullscreen landscape mode

Ideal for:
- Python Flask video servers
- Raspberry Pi camera setups
- Local IP camera streams
- Developer testing environments

---

## 📥 Download APK

👉 Download the latest APK from the **Releases** section of this repository.

After downloading:

1. Enable **Install from Unknown Sources**
2. Install the APK
3. Connect to the same WiFi network as your server
4. Open the app and connect

---

## ✨ Features

### 🔍 Automatic Network Discovery
- Scans the entire local subnet
- Detects servers running on port `5000`
- Displays discovered servers instantly
- Shows real-time scan progress
- Smart timeout handling

---

### 📷 QR Code Scanner
- Custom camera overlay UI
- Supports HTTP/HTTPS links
- Accepts raw IP addresses
- Smart validation and error handling
- Instant connection after scan

---

### ⌨ Manual IP Connection
Supports:
```
192.168.1.100
192.168.1.100:5000
http://192.168.1.100:5000
```

The app automatically normalizes the input to a valid URL.

---

### 🎥 Built-in Stream Viewer
- WebView-based streaming
- JavaScript & DOM support
- Smooth loading experience
- Loading indicator
- Friendly connection error messages

---

### ⛶ Fullscreen Mode
- One-tap landscape streaming
- Screen orientation lock
- Auto-reset on disconnect

---

### 🔄 Smart Navigation Handling
- Back button closes QR scanner
- Back button disconnects stream
- Safe cleanup on exit

---


## 📡 How It Works

1. The app retrieves your device's local IP address.
2. Extracts the subnet prefix (e.g., 192.168.1.x).
3. Scans all addresses in that range on port `5000`.
4. Displays responsive servers.
5. Connects via embedded WebView.

Connection timeout is controlled using AbortController for stability.

---

## 📱 Requirements

- Android 7.0+
- WiFi connection
- Server running on port `5000`
- Same local network

---

## 🧠 Example Server Setup (Python Flask)

Typical server address:
```
http://192.168.x.x:5000
```

Make sure:

- Devices are on same WiFi
- Firewall allows Python
- Port 5000 is open

---

## 🔐 Permissions Used

| Permission | Purpose |
|------------|----------|
| Camera | QR code scanning |
| Network | Stream loading & subnet scanning |
| Screen Orientation | Fullscreen landscape mode |

---

## 🛠 Built With

- React Native
- Expo
- React Native WebView

---

## 📈 Future Improvements

- Save previous server history
- Auto-reconnect option
- Stream quality selector
- Server authentication
- HTTPS verification
- Play Store release

---

## 📊 Version

**v1.0.0**
- QR scan support
- LAN auto-discovery
- Manual IP connection
- Fullscreen streaming

---

## 📄 License

MIT License

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.

```
screenshots/
```
<img width="480px" alt="home" src="https://github.com/user-attachments/assets/e2df25ef-8a8d-40f8-aa82-0cf9bd6f1e45" />
<img width="480px" alt="Qrcode" src="https://github.com/user-attachments/assets/1be01daa-3836-41cb-915a-bb2e1283a9f2" />
<img width="480px" alt="afterconnect" src="https://github.com/user-attachments/assets/03c9e6bf-87a9-476b-a090-792b81f92fcf" />
