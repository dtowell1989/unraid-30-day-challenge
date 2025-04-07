
# 🧻 TOWELLNAS — Week 2: Docker & Self-Hosted Apps  
**Theme:** Explore Docker, start automation, compare media servers, and lay the groundwork for remote access and gaming  
**Estimated Time:** 4–6 hours (flexible)

---

## 🧠 Goals

- Learn how Docker works in Unraid (appdata, volume mapping, ports)
- Run your first containers using your existing shares
- Explore file and media tools (automation, access, playback)
- Set up secure remote access (Tailscale)
- Bonus: experiment with a game server

---

## 📁 Prep Checklist

- [x] Shares set up (`downloads`, `media`, `bulk`, `appdata`)
- [x] Tinker SSD mounted and formatted
- [x] User account (`dtowell1989`) created
- [x] Community Apps & User Scripts installed
- [x] Notifications and config backups working

---

## 🔧 Weekly Breakdown

### 📅 Day 1–2: File Access with FileBrowser
- Install FileBrowser via Community Apps
- Map volumes:
  - `/mnt/user` → `/srv`
- Test uploads/downloads/renames in the browser

---

### 📅 Day 3–4: Torrent Client + VPN (qBittorrent + Mullvad)
- Install `binhex-qbittorrentvpn`
- Provide Mullvad `.ovpn` or WireGuard config
- Map:
  - `/mnt/user/downloads/incomplete` → `/data/incomplete`
  - `/mnt/user/downloads/complete` → `/data/complete`
- Confirm VPN protection & torrent functionality

---

### 📅 Day 5: Automated Media Downloading
- Install:
  - Sonarr (TV)
  - Radarr (Movies)
  - Jackett or Prowlarr (Indexers)
- Configure:
  - Download paths to `downloads` share
  - Indexers & test library automation

---

## 🎉 Bonus Projects

### 🎞️ Plex vs Jellyfin
- Install both
- Point to same `media` share
- Compare interfaces, transcoding, performance

### 🌐 Tailscale
- Install and connect to Tailscale
- Test access to TOWELLNAS from outside LAN

### 🎮 Game Server Trial (Docker)
- Choose a lightweight game (Valheim, Minecraft, etc.)
- Install via Community Apps
- Use `games` share or Tinker SSD for save data

---

## 🧠 Reflection Ideas (for notes.md)
- Which apps will I keep long-term?
- Which container gave me the most insight or frustration?
- Do I actually *need* remote access or gaming, or was it just fun?

