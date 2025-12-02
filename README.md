# JAH-Meet
Lightweight live streaming &amp; webinar platform with multi-host support, live Q&amp;A, viewer count, and mobile-friendly WebRTC — no database required.

Live Meet – Lightweight Webinar Platform

Live Meet is a lightweight, browser-based live streaming & webinar platform built using Node.js, Socket.IO, and WebRTC.
It supports multi-host broadcasting, hundreds of viewers, live Q&A, and a clean professional UI — all without a database.

Designed for lectures, religious talks, webinars, and community events.

🚀 Features

✅ Multi-host live video streaming

✅ Unlimited viewers (architecture-ready; bandwidth dependent)

✅ Live viewer count for hosts

✅ Real-time Q&A system

Host-controlled (enable/disable questions)

✅ Mic mute/unmute with visual indicators

✅ Fullscreen video for viewers

✅ Responsive UI

Mobile-optimized

Professional desktop layout

✅ HTTPS & mobile camera support

✅ No database required

✅ Single-server deployment

🧱 Tech Stack

Node.js

Express

Socket.IO

WebRTC

Nginx (reverse proxy)

Let’s Encrypt SSL

📁 Project Structure
project/
 ├ server.js
 ├ public/
 │   ├ index.html
 │   └ images/
 │       └ logo.png

⚙️ Installation
1️⃣ Clone the repository
git clone https://github.com/yourusername/live-meet.git
cd live-meet

2️⃣ Install dependencies
npm install

3️⃣ Start the server
node server.js


App runs on:

http://localhost:3000

🔐 Authentication

Edit passwords directly in server.js:

const HOST_PASSWORD = 'host123';
const VIEWER_PASSWORD = 'view123';

🌐 Production Deployment (Recommended)

✅ Ubuntu 20.04 / 22.04

✅ EC2 instance: c6i.large

✅ Nginx reverse proxy

✅ SSL using Let’s Encrypt

⚠️ HTTPS is required for camera & mic access on mobile devices

📡 Scaling Notes

Current architecture uses peer-to-peer WebRTC

Suitable for:

100–200 viewers with live video

500+ viewers with reduced bitrate

For large-scale events (1k+), integrate an SFU (mediasoup / LiveKit)

✅ Ideal Use Cases

Online lectures

Religious talks & sermons

Community announcements

Small webinars

Hybrid live events

🔮 Planned Improvements

Screen sharing

Question upvoting

Host spotlight

Recording support

SFU integration

Role-based moderation

🤝 Contributing

Pull requests are welcome.
Feel free to fork, improve UI, or extend features.

📜 License

MIT License
