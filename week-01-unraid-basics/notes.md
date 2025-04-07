# 🗂️ Week 1: Unraid Setup & File Management  
**Focus Area:** System Administration / Storage / Networking  
**Time Spent:** ~5–6 hours

---

## ✅ Tasks Completed

- Set up Unraid array with 2x 18TB HDDs + 1 parity disk
- Configured a 2-drive SSD cache pool (2x 128GB M.2 drives)
- Created core user shares:
  - `downloads` (Cache ➜ Array with mover enabled)
  - `media`, `bulk`, `appdata`
- Configured SMB settings for share access from Windows
- Learned best practices for organizing folders by share vs by subfolder
- Installed **Community Apps** plugin
- Set up **notifications** via Gmail + SMS (Spectrum Mobile via `vtext.com`)
- Explored Unassigned Devices:
  - Mounted and formatted 256GB SSD (`Tinker`)
  - Created subfolders: `docker_scratch/`, `unraid_backups/`
- Installed **User Scripts** plugin
- Wrote and tested a flash config backup script with timestamped folders

---

## 🧠 What I Learned

- How Unraid separates storage into array, cache, and unassigned pools
- Why shares are the key unit of organization (and tuning!) in Unraid
- The importance of setting cache behavior and using the mover properly
- That Unraid doesn't manage subfolders—you do that via SMB or command line
- How to mount and repurpose unused hardware (SSD) with Unassigned Devices
- How to configure and test SMTP email alerts and email-to-text for real-time notifications

---

## 🧩 Challenges or Things I Spent Extra Time On

- Understanding when/why to split data into multiple shares vs one bulk share
- Formatting the unassigned SSD manually since Unraid doesn’t expose ZFS formatting in the UI
- Figuring out the Gmail app password setup for Unraid SMTP notifications

---

## 📌 Notes to Future Me

- I should review mover settings occasionally to ensure cache isn't filling up
- Consider scheduling a cleanup script for old backups on the Tinker SSD
- Eventually I may want to snapshot `/docker_scratch/` or test ZFS again
- Look into Unraid flash backup via CA Appdata Backup plugin later

---

## 🚀 Ready for Week 2

- Docker apps next: I’ll start with something simple like FileBrowser or qBittorrent
- I’ll map volumes to my structured shares and test automation tools like Watchtower
- Might use `/mnt/disks/Tinker/docker_scratch` for testing or temp workloads

