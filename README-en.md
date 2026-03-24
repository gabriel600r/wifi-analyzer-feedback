<div align="center">
  <!-- Replace the URL below with the actual link to your logo -->
  <img src="./assets/logo.png" alt="EgeaINC WiFi Analyzer Logo" width="150" style="border-radius: 20px;"/>
  <h1>EgeaINC WiFi Analyzer</h1>
  <p><b>Your WiFi and Cellular Network, Under Absolute Control</b></p>
  
  <br/>
  <a href="https://egeainc.com/wifi">
    <img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" alt="Get it on Google Play" height="80"/>
  </a>
</div>

<br/>

<div align="center">
  <a href="README.md">🇦🇷 Español</a> | <b>🇺🇸 English</b>
</div>

<br/>

Professional WiFi and cellular network analyzer, and IT tools suite. Designed for technicians, network administrators, gamers, and power users who need to diagnose, monitor, and optimize all their connections to the highest level.

Monitor your network in real-time with a modern and fluid **"glass" cyberpunk** interface. The Main Dashboard is a command center that shows you in a single view:
- **Global Status:** Real-time animated connection health gauge.
- **WiFi Network:** SSID, Signal Strength (dBm), Link Speed, Standard (e.g., WiFi 6 / 802.11ax), Security, and MAC Address (BSSID).
- **IP Metrics:** Local IP, Subnet Mask, and DNS Servers (1 and 2).
- **Routing:** Gateways (Router IP), Frequency (2.4 / 5 GHz), Channels, and animated historical graph with constant Ping to the Router.
- **Internet Outbound:** Your external Public IP, Provider (ISP), and persistent Ping to global servers (e.g., Google 8.8.8.8) measured directly on continuous charts.

---

## 🔥 NEW IN THIS VERSION (v0.66.2)

### New Tool: Fiber dB Calculator
- **Fiber attenuation calculation:** Supports Single Mode (SM G.652), Multimode 50/125, and Multimode 62.5/125 at multiple wavelengths (850, 1300, 1310, 1550 nm).
- **Freemium model:** Basic attenuation-by-distance calculation is free. Advanced features are Pro:
  - Splices (fusion/mechanical), connectors, and safety margin.
  - Visual loss breakdown bar by component.
  - PASS/FAIL comparison against real OTDR or power meter measurements.
  - dBm ↔ mW converter with real-time conversion.
  - History of up to 50 measurements with detail view and swipe-to-delete.
  - Share results with branding and download link.
- **Built-in glossary:** Info icons next to each field to learn what each parameter means.
- **Persistence:** Remembers your last fiber type, wavelength, splice type, and margin.
- **Non-expert guidance:** Each fiber type includes a description to help you choose the right one.

### Sidebar Reorganized
- Tools are now sorted by logical category: WiFi → Network/Monitoring → Internet/Exploration → Cabling/Fiber → Utilities.
- Free and Pro tools appear interleaved by category instead of separated into blocks.

### Visual Improvements
- **Color-coded selectors:** Each selector (fiber type, wavelength, splice type) has its own distinctive color to break visual monotony.

👉 **[View full changelog](CHANGELOG.md)**

---

## 📸 INTERFACE AND TOOLS

<div align="center">
  <img src="./assets/1.png?v=2" width="23%" alt="Home Screen"/>
  <img src="./assets/2.png?v=2" width="23%" alt="LAN Scanner"/>
  <img src="./assets/3.png?v=2" width="23%" alt="Cellular Monitor"/>
  <img src="./assets/4.png?v=2" width="23%" alt="WiFi Channels"/>
</div>

<div align="center">
  <img src="./assets/5.png?v=2" width="23%" alt="Ping Monitor"/>
  <img src="./assets/6.png?v=2" width="23%" alt="FO Color Code"/>
  <img src="./assets/7.png?v=2" width="23%" alt="Speed Test"/>
  <img src="./assets/8.png?v=2" width="23%" alt="Utilities"/>
</div>

<div align="center">
  <img src="./assets/9.png?v=2" width="23%" alt="Ping Details"/>
  <img src="./assets/10.png?v=2" width="23%" alt="Connected Devices"/>
  <img src="./assets/11.png?v=2" width="23%" alt="Offline LAN Scanner"/>
  <img src="./assets/12.png?v=2" width="23%" alt="Local Services"/>
</div>

<div align="center">
  <img src="./assets/13.png?v=2" width="23%" alt="Network Statistics"/>
  <img src="./assets/14.png?v=2" width="23%" alt="UPnP Analyzer"/>
  <img src="./assets/15.png?v=2" width="23%" alt="Advanced Settings"/>
  <img src="./assets/16.png?v=2" width="23%" alt="About"/>
</div>

<div align="center">
  <img src="./assets/17.png?v=2" width="23%" alt="More Features"/>
  <img src="./assets/18.png?v=2" width="23%" alt="FO Distribution Center View"/>
  <img src="./assets/19.png?v=2" width="23%" alt="Favorites Home"/>
  <img src="./assets/20.png?v=2" width="23%" alt="FO Port Details"/>
</div>

<br/>

<div align="center">
  <h3>🎥 Demo Video</h3>
  <a href="https://www.youtube.com/shorts/nks--i486GM" target="_blank">
    <img src="https://img.youtube.com/vi/nks--i486GM/0.jpg" alt="Watch the EgeaINC WiFi Analyzer Demo Video" width="250" style="border-radius: 12px;"/>
  </a>
  <br/>
  <p><i>Click the image to watch the YouTube Short in action</i></p>
</div>

---

## 🛠️ INTEGRATED TOOL SUITE

### Connectivity and Diagnostics
- 📶 **WiFi Channels:** Analyzes congestion on 2.4GHz and 5GHz to find the optimal channel.
- 📋 **WiFi History:** Logs your connections with signal and ISP data on expandable cards.
- 🔍 **LAN Scanner:** Discovers devices on your network with smart active/inactive detection.
- 🚪 **Port Scanner:** Detects open TCP ports and active services (HTTP, SSH, etc.).
- ⏱️ **Ping Monitor:** Measures latency in real-time with continuous scrolling graphs.
- 🚀 **Speed Test:** Multi-connection speed test via Cloudflare CDN with bottleneck indicators.
- 📱 **Mobile Network:** Deep analysis of cellular signal.
- 🌍 **Public IP:** Displays your external IP and your ISP.

### Cabling and Fiber Optics
- 🔌 **RJ-45 Pinout:** Visual guide for wiring UTP cables (T-568A/B).
- 🎨 **FO Color Code:** Interactive viewer for TIA-598-C and SIECOR standards.
- 📉 **Fiber dB Calculator:** Calculates expected attenuation for a fiber optic link based on fiber type, wavelength, distance, splices, connectors, and margin. Compare against real measurements (PASS/FAIL) and includes a dBm↔mW converter.

### Utilities and References
- 🔑 **Password Generator:** Creates ultra-secure and customizable passwords.
- 🧮 **IP Calculator:** Calculates subnets, ranges, and CIDR masks.

---

## 💎 EGEAINC PRO (Premium)

Unlock advanced tools and remove all limits:

- 🔎 **DNS Lookup:** Queries DNS records (A, MX, TXT, NS, etc.).
- 🕵️ **Whois:** Gets detailed domain registration and ownership information.
- 🛤️ **Traceroute:** Tracks the route and measures packet hop times across the network.
- ⚡ **Wake on LAN (WoL):** Turns on computers on your network remotely.
- 🔌 **UPnP Scanner:** Discovers devices with Universal Plug and Play enabled.
- ➕ **Additional Pro Features:** Neighboring cell detection (Mobile Network), extended history (Speed Test), and advanced filters.

---

## 📱 HIGHLIGHTED FEATURES

- ✔️ **"Glass" dark design:** Optimized for OLED screens.
- ✔️ **Bilingual Interface:** Available in Spanish and English.
- ✔️ **Educational Glossary:** Tap any metric to learn technical concepts.
- ✔️ **Guaranteed Privacy:** Clean, secure experience with no hidden tracking.

---

## 💬 Feedback and Support

This repository is strictly intended for the community to provide **feedback, report bugs, and suggest new features** for EgeaINC WiFi Analyzer. 

If you found a bug or have a great idea for the app:
👉 **[Open a new Issue here](https://github.com/gabriel600r/wifi-analyzer-feedback/issues)**

Thank you for helping us improve!
