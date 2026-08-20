<div align="center">
<!-- Retro Window Chrome Header -->
<img src="https://img.shields.io/badge/🦋%20MeshLink-v1.0.0-4A90E2?style=for-the-badge&labelColor=357ABD&color=E3F2FD" alt="MeshLink Badge">
<img src="https://img.shields.io/badge/📡%20Offline-Ready-32CD32?style=for-the-badge&labelColor=228B22&color=E8F5E9" alt="Offline Badge">
<img src="https://img.shields.io/badge/💬%20P2P-Mesh-FFB6C1?style=for-the-badge&labelColor=FF69B4&color=FFF0F5" alt="P2P Badge">
<!-- Retro ASCII / Styled Title -->
<h1>
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Animals/Butterfly.png" width="35" />
  <span style="color:#4A90E2; font-family:'Tahoma',sans-serif;">MeshLink</span>
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Animals/Butterfly.png" width="35" />
</h1>
<p align="center">
  <b style="font-size:18px; color:#6B7280; font-family:'Verdana',sans-serif;">
    ✨ Offline Mesh Communication Platform ✨
  </b>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Windows%20XP-Vibes-4A90E2?style=flat-square&logo=windowsxp&logoColor=white&labelColor=357ABD">
  <img src="https://img.shields.io/badge/Y2K-Aesthetic-FFB6C1?style=flat-square&labelColor=FF69B4">
  <img src="https://img.shields.io/badge/BLE-Mesh-C8A2DB?style=flat-square&labelColor=9370DB">
</p>
</div>
<!-- XP-Style Window Container -->
<div style="border: 2px solid #7DA2CE; border-radius: 6px; background: linear-gradient(180deg, #A8C8EC 0%, #E8F1FA 100%); padding: 16px; margin: 16px 0; box-shadow: 2px 2px 6px rgba(0,0,0,0.15);">
<h3 style="margin:0; font-family:'Tahoma',sans-serif; color:#1A1A1A; font-size:14px;">
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Computer%20Disk.png" width="18" /> 
  🟢 <b>MeshLink.exe</b> — README.md
</h3>
</div>
📟 Overview
MeshLink is a retro-styled, peer-to-peer messaging application that lets you chat with nearby devices without internet, cellular data, or centralized servers.
Inspired by the golden era of instant messengers (MSN Messenger 7.5, Windows XP, Y2K digital aesthetics), MeshLink combines nostalgic UI design with modern decentralized networking — creating an ad-hoc mesh network using Bluetooth Low Energy (BLE) and Wi-Fi Direct.
Whether you're at a music festival, on a remote hike, in an emergency situation, or just vibing offline — MeshLink keeps you connected. 🦋💬
<div align="center">
Table
🌐 No Internet	🔒 Encrypted	🔋 Battery Aware
Works completely offline	AES-256 end-to-end	Adaptive scanning
</div>
🎨 UI Theme & Aesthetic
"It's not a bug, it's a feature from 2005."
MeshLink is designed with Digital Nostalgia in mind:
🪟 Windows XP Chrome — Gradient title bars, glossy buttons, 1px borders
💗 Y2K Bubblegum — Pastel pinks, soft blues, rainbow accents
👾 Pixel Art Icons — 1px outlined emoticons and retro system icons
💻 CRT Scanlines — Subtle lo-fi texture on mesh visualization screens
🎵 Now Playing — MSN-style music status integration
<div align="center">
plain
┌─────────────────────────────────────────┐
│  🦋 MeshLink — Chat with Sarah :D    [_][□][X] │
├─────────────────────────────────────────┤
│  Sarah :D (Away) — I love music! <3    │
│  ┌────────┐                            │
│  │ 👤     │  hey wats up? ~~~~~~~~~~>  │
│  └────────┘                            │
│         <~~~~~~~~ not much, hbu? :P    │
│                                        │
│  [Type a message...]              [Send]│
└─────────────────────────────────────────┘
</div>
✨ Key Features
Table
Feature	Status	Description
📴 Offline Messaging	✅	No internet or servers required
📡 BLE Communication	✅	Bluetooth Low Energy peer discovery
📶 Wi-Fi Direct	✅	High-bandwidth peer connections (Android)
🔍 Auto Discovery	✅	Nearby devices detected automatically
🔐 End-to-End Encryption	✅	AES-256 with secure key exchange
🕸️ Mesh Forwarding	✅	Messages relay through intermediate devices
👥 Group Conversations	✅	Broadcast to all connected peers
📬 Delivery Status	✅	Sent / Delivered / Read receipts
🔄 Offline Sync	✅	Messages queue and send on reconnect
👤 User Profiles	✅	Custom display names, status messages, avatars
🔋 Battery Optimization	✅	Adaptive scan intervals based on power level
🌙 Dark & Light Themes	✅	XP Blue + Kawaii Pink + Terminal Green
🍎 Cross-Platform	🔄	Flutter — Android primary, iOS via Multipeer
🏗️ Technical Architecture
<div align="center">
plain
┌─────────────────────────────────────────────────────────────┐
│                    PRESENTATION LAYER                        │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────┐  │
│  │  Contact List │  │ Chat Window  │  │ Mesh Radar Map   │  │
│  │  (MSN Style)  │  │ (Bubbles)    │  │ (Node Graph)     │  │
│  └──────────────┘  └──────────────┘  └──────────────────┘  │
├─────────────────────────────────────────────────────────────┤
│                     STATE MANAGEMENT                         │
│                    Riverpod (Flutter)                        │
├─────────────────────────────────────────────────────────────┤
│                     DOMAIN LAYER                             │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────┐  │
│  │  Mesh Router  │  │ Crypto Serv. │  │ Message Handler  │  │
│  │  (Flooding)   │  │ (AES-256)    │  │ (Queue + Sync)   │  │
│  └──────────────┘  └──────────────┘  └──────────────────┘  │
├─────────────────────────────────────────────────────────────┤
│                    DATA LAYER                                │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────┐  │
│  │  Hive (Local) │  │ BLE Transport│  │ WiFi Transport   │  │
│  │  Messages/Peers│  │ (Peripheral+│  │ (Nearby Conn.)   │  │
│  │               │  │  Central)    │  │                  │  │
│  └──────────────┘  └──────────────┘  └──────────────────┘  │
├─────────────────────────────────────────────────────────────┤
│              BACKGROUND SERVICE (Android)                   │
│         Foreground Service + BLE State Restoration          │
└─────────────────────────────────────────────────────────────┘
</div>
Stack
Table
Layer	Technology
Framework	Flutter 3.x
Language	Dart
State Management	Riverpod
Local Database	Hive
BLE	flutter_blue_plus
Wi-Fi Direct	nearby_connections (Android)
iOS Fallback	multipeer_connectivity
Encryption	encrypt (AES-256-GCM)
Background	flutter_background_service
Notifications	flutter_local_notifications
🚀 Getting Started
Prerequisites
📱 Android 8.0+ (API 26) with BLE support
🍎 iOS 14+ (limited — Multipeer Connectivity fallback)
🛠️ Flutter SDK 3.16 or higher
🔧 Android Studio or VS Code
📲 2+ Physical Devices (BLE does not work on emulators)
Installation
bash
# 1. Clone the repo
git clone https://github.com/yourusername/meshlink.git
cd meshlink

# 2. Install dependencies
flutter pub get

# 3. Configure Android permissions
# Already included in AndroidManifest.xml — just verify:
# BLUETOOTH_SCAN, BLUETOOTH_ADVERTISE, BLUETOOTH_CONNECT, LOCATION

# 4. Run on a physical device
flutter run
First Mesh Test
Phone A: Tap Start Advertising 🟢
Phone B: Tap Start Scanning 🔍
Wait — devices will appear in the contact list
Tap Connect — complete the handshake 🤝
Start chatting — no internet required! 💬
🧠 How It Works
The Mesh Protocol (Simplified)
plain
┌──────┐      BLE/WiFi      ┌──────┐      BLE/WiFi      ┌──────┐
│ You  │ ◄────────────────► │ Alex │ ◄────────────────► │ Mia  │
└──────┘                    └──────┘                    └──────┘
    │                           │                           │
    │  "Hey Mia!" (TTL: 5)      │                           │
    │──────────────────────────►│                           │
    │                           │  "Hey Mia!" (TTL: 4)      │
    │                           │──────────────────────────►│
    │                           │                           │
    │                           │  ACK: "Got it!"           │
    │  ACK relayed back         │◄──────────────────────────│
    │◄──────────────────────────│                           │
Rules:
🔁 Flooding: Messages propagate to all connected peers (minus sender)
⏳ TTL: Time-To-Live prevents infinite loops (default: 5 hops)
🧠 Deduplication: Every device tracks the last 1,000 message IDs
🔐 Encryption: Payload encrypted with AES-256-GCM before transmission
📦 Chunking: Large messages split into 180-byte BLE packets
🗺️ Roadmap
Table
Phase	Feature	Status
✅ V1.0	Offline text messaging via BLE	Done
✅ V1.0	Mesh relay & forwarding	Done
🔄 V1.1	Voice messages over mesh	In Progress
🔄 V1.1	Image & file sharing	In Progress
📋 V1.2	Multi-hop routing optimization	Planned
📋 V1.2	Emergency SOS broadcast	Planned
📋 V1.3	Offline location sharing	Planned
📋 V1.3	QR-code secure pairing	Planned
📋 V2.0	Desktop support (Windows/Linux)	Planned
📋 V2.0	Mesh network visualization	Planned
🛡️ Security
AES-256-GCM encryption on all messages
Per-session keys via ECDH key exchange (roadmap)
No cloud storage — everything is local
No metadata leaks — no servers, no logs, no tracking
🤝 Contributing
This is a passion project exploring decentralized communication. Contributions welcome!
Fork the repo
Create your feature branch: git checkout -b feature/amazing-feature
Commit your changes: git commit -m 'Add amazing feature'
Push to the branch: git push origin feature/amazing-feature
Open a Pull Request
Please read our Code of Conduct first. 💙
📜 License
Distributed under the MIT License. See LICENSE for more information.
plain
MIT License

Copyright (c) 2026 MeshLink Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
<div align="center">
<h3 style="font-family:'Tahoma',sans-serif; color:#4A90E2;">
  Made with 💙 & a lot of nostalgia for the 2000s
</h3>
<p>
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Blue%20Heart.png" width="24">
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Mobile%20Phone.png" width="24">
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Rainbow.png" width="24">
</p>
<p style="font-size:11px; color:#6B7280; font-family:'Verdana',sans-serif;">
  <i>"wanna chat? bring ur phone, leave ur wifi at home."</i>
</p>
</div>
