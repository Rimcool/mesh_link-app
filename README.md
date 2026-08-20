  
 MeshLink 
 ✨ Offline Mesh Communication Platform ✨ 
  

 🟢 MeshLink.exe — README.md
📟 Overview
MeshLink is a retro-styled, peer-to-peer messaging application that lets you chat with nearby devices without internet, cellular data, or centralized servers.
Inspired by the golden era of instant messengers (MSN Messenger 7.5, Windows XP, Y2K digital aesthetics), MeshLink combines nostalgic UI design with modern decentralized networking — creating an ad-hoc mesh network using Bluetooth Low Energy (BLE) and Wi-Fi Direct.
Whether you’re at a music festival, on a remote hike, in an emergency situation, or just vibing offline — MeshLink keeps you connected. 🦋💬
🌐 No Internet	🔒 Encrypted	🔋a Battery Aware
Works completely offline	AES-256 end-to-end	Adaptive scanning

🎨 UI Theme & Aesthetic
“It’s not a bug, it’s a feature from 2005.”
MeshLink is designed with Digital Nostalgia in mind:
•🪟 Windows XP Chrome — Gradient title bars, glossy buttons, 1px borders
•💗 Y2K Bubblegum — Pastel pinks, soft blues, rainbow accents

•👾 Pixel Art Icons — 1px outlined emoticons and retro system icons
•💻 CRT Scanlines — Subtle lo-fi texture on mesh visualization screens
•🎵 Now Playing — MSN-style music status integration
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

✨ Key Features
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
Stack
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
•📱 Android 8.0+ (API 26) with BLE support
•🍎 iOS 14+ (limited — Multipeer Connectivity fallback)
•🛠️ Flutter SDK 3.16 or higher
•🔧 Android Studio or VS Code
•📲 2+ Physical Devices (BLE does not work on emulators)
Installation
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
1.Phone A: Tap Start Advertising 🟢
2.Phone B: Tap Start Scanning 🔍
3.Wait — devices will appear in the contact list
4.Tap Connect — complete the handshake 🤝
5.Start chatting — no internet required! 💬

🧠 How It Works
The Mesh Protocol (Simplified)
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
Rules: - 🔁 Flooding: Messages propagate to all connected peers (minus sender) - ⏳ TTL: Time-To-Live prevents infinite loops (default: 5 hops) - 🧠 Deduplication: Every device tracks the last 1,000 message IDs - 🔐 Encryption: Payload encrypted with AES-256-GCM before transmission - 📦 Chunking: Large messages split into 180-byte BLE packets

🗺️ Roadmap
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
•AES-256-GCM encryption on all messages
•Per-session keys via ECDH key exchange (roadmap)
•No cloud storage — everything is local
•No metadata leaks — no servers, no logs, no tracking

🤝 Contributing
This is a passion project exploring decentralized communication. Contributions welcome!
1.Fork the repo
2.Create your feature branch: git checkout -b feature/amazing-feature
3.Commit your changes: git commit -m 'Add amazing feature'
4.Push to the branch: git push origin feature/amazing-feature
5.Open a Pull Request
Please read our Code of Conduct first. 💙

📜 License
Distributed under the MIT License. See LICENSE for more information.
MIT License

Copyright (c) 2026 MeshLink Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...

Made with 💙 & a lot of nostalgia for the 2000s
  
“wanna chat? bring ur phone, leave ur wifi at home.”
