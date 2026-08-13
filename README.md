# Fling

Send photos, videos, and files directly between devices — phone to laptop,
laptop to laptop, from anywhere, not just the same WiFi. No accounts, no
cloud storage, nothing saved on a server.

## How it works

- One device taps **Receive** → gets a 4-character code + QR code.
- The other device scans it (or types the code) and taps **Connect**.
- Files transfer **peer-to-peer** over WebRTC, straight from one browser to
  the other. The only thing that touches a third party is the initial
  handshake (who's trying to reach whom) — the actual file bytes never pass
  through any server, including mine or Vercel's.
- Because it's WebRTC (not local-network mDNS like the desktop app), this
  works **across different networks** too — phone on mobile data, laptop on
  home WiFi, still connects.

