# 🐱‍💻 Top Kali Linux Commands: Ultimate Cheat Sheet for Hackers & Power Users

![Kali Linux Wallpaper](https://www.kali.org/wallpapers/images/2024/kali-ferrofluid.jpg)

---

## 👋 Welcome, Curious Hackers & Self-Starters!

> Crafted by a Linux enthusiast from a non-technical background, this cheat sheet proves that with **curiosity and consistency**, anyone can break into the world of ethical hacking, cybersecurity, and system mastery.

Use this guide as your terminal-sidekick — whether you're learning, testing, or pwning.

---

## 🧭 Table of Contents

- [📁 1. File & Directory Management](#1-file--directory-management)
- [🧠 2. File Viewing & Editing](#2-file-viewing--editing)
- [👥 3. User Management](#3-user-management)
- [🌐 4. Network Commands](#4-network-commands)
- [📦 5. Package Management (APT)](#5-package-management-apt)
- [🔐 6. Permissions & Ownership](#6-permissions--ownership)
- [🗜️ 7. Archiving & Compression](#7-archiving--compression)
- [📊 8. System Monitoring](#8-system-monitoring)
- [🔍 9. Search & Filter Commands](#9-search--filter-commands)
- [⚙️ 10. Process Management](#10-process-management)
- [💽 11. Disk, Mount & USB Tools](#11-disk-mount--usb-tools)
- [🧩 12. Boot & Service Management](#12-boot--service-management)
- [🧪 13. Pentesting Tools (Kali)](#13-pentesting-tools-kali)
- [🎨 14. Miscellaneous Commands](#14-miscellaneous-commands)
- [🎯 15. Fun & Eye-Candy Commands](#15-fun--eye-candy-commands)
- [💡 Tips & Tricks](#-tips--tricks)
- [📄 References](#-references)

---

## ✨ Quick Tip

> 💬 Use `man <command>` to read manual pages. Example: `man grep`

---

## 📁 1. File & Directory Management

| Command   | Description             | Options                                          |
|-----------|-------------------------|--------------------------------------------------|
| `ls`      | List directory contents | `-a`, `-l`, `-h`                                 |
| `cd`      | Change directory        | `cd ..`, `cd ~`                                  |
| `pwd`     | Print working directory |                                                  |
| `mkdir`   | Make directory          | `-p` (create parents)                            |
| `rm`      | Remove file/folder     | `-r` (recursive), `-f` (force)                    |
| `cp`      | Copy file/folder       | `-r`, `-v`                                        |
| `mv`      | Move or rename         |                                                   |
| `touch`   | Create empty file      |                                                   |
| `tree`    | Visual directory view  | `-L` (limit depth)                                |

---

## 🧠 2. File Viewing & Editing

| Command   | Description            | Options                                           |
|-----------|------------------------|---------------------------------------------------|
| `cat`     | Print file             | `-n` (line numbers)                               |
| `less`    | Scrollable view        | `/` (search), `q` (quit)                          |
| `more`    | Paged view             | Space, `q`                                        |
| `head`    | First lines            | `-n` (number of lines)                            |
| `tail`    | Last lines             | `-f` (follow live output)                         |
| `nano`    | Simple editor          | Ctrl+O (save), Ctrl+X (exit)                      |
| `vim`     | Advanced editor        | `i`, `:wq`, `ESC`                                 |

---

## 👥 3. User Management

| Command     | Description             | Notes                         |
|-------------|-------------------------|-------------------------------|
| `whoami`    | Current user            |                               |
| `id`        | UID, GID info          |                                |
| `adduser`   | Add user               | `adduser <name>`               |
| `passwd`    | Change password        |                                |
| `su`        | Switch user            | `su -`                         |
| `sudo`      | Superuser privilege    | `sudo <command>`               |
| `users`     | Show logged in users   |                                |
| `groups`    | Show user groups       | `groups <username>`            |

---

## 🌐 4. Network Commands

| Command      | Description             | Notes                          |
|--------------|-------------------------|--------------------------------|
| `ifconfig`   | Show interfaces         | (legacy)                       |
| `ip`         | Network management      | `ip a`, `ip r`                 |
| `ping`       | Test connection         | `-c`, `-i`                     |
| `netstat`    | Network stats           | `-tulpn`                       |
| `ss`         | Socket stats            | `-ltnp`                        |
| `traceroute` | Trace route             | `traceroute <host>`            |
| `nslookup`   | DNS lookup              |                                |
| `dig`        | DNS tool                | `+short`, `ANY`, `MX`          |
| `nmap`       | Port scan               | `-A`, `-T4`, `-p-`             |
| `wget`       | Download from URL       | `-c`, `-O`                     |
| `curl`       | Web requests            | `-I`, `-X`, `-d`               |

---

## 📦 5. Package Management (APT)

| Command            | Description           | Options                        |
|--------------------|-----------------------|--------------------------------|
| `apt update`       | Refresh package list  |                                |
| `apt upgrade`      | Upgrade packages      | `-y`                           |
| `apt install`      | Install package       | `-y`, `--no-install-recommends`|
| `apt remove`       | Remove package        | `--purge`                      |
| `apt autoremove`   | Clean unused packages |                                |
| `dpkg -i`          | Install `.deb` file   |                                |
| `apt-cache search` | Search packages       |                                |

---

## 🔐 6. Permissions & Ownership

| Command    | Description              | Examples               |
|------------|--------------------------|------------------------|
| `chmod`    | Set permissions          | `+x`, `755`, `u+x`     |
| `chown`    | Set ownership            | `user:group`           |
| `umask`    | Default permissions mask | `umask 022`            |
| `ls -l`    | Show perms/owners        |                        |

---

## 🗜️ 7. Archiving & Compression

| Command   | Description         | Examples                         |
|-----------|---------------------|----------------------------------|
| `tar`     | Archive files       | `-cvf`, `-xvf`, `-czvf`          |
| `gzip`    | Compress file       |                                  |
| `gunzip`  | Decompress `.gz`    |                                  |
| `zip`     | Create zip          | `-r`                             |
| `unzip`   | Extract zip         |                                  |

---

## 📊 8. System Monitoring

| Command   | Description       | Notes                     |
|-----------|-------------------|---------------------------|
| `top`     | Real-time monitor |                           |
| `htop`    | Visual top        | `apt install htop`        |
| `df -h`   | Disk usage        | Human-readable            |
| `du -sh`  | Folder size       |                           |
| `free -h` | Memory usage      |                           |
| `uptime`  | System uptime     |                           |

---

## 🔍 9. Search & Filter Commands

| Command   | Description         | Examples                            |
|-----------|---------------------|-------------------------------------|
| `grep`    | Search text         | `-i`, `-r`, `--color`               |
| `find`    | Find files          | `-name`, `-type`, `-exec`           |
| `locate`  | Fast file search    | `locate <filename>`                 |
| `which`   | Find binary path    | `which python`                      |

---

## ⚙️ 10. Process Management

| Command    | Description         | Notes                    |
|------------|---------------------|--------------------------|
| `ps aux`   | List processes      |                          |
| `kill`     | Kill by PID         | `-9` (force)             |
| `killall`  | Kill by name        | `killall firefox`        |
| `jobs`     | Show background jobs|                          |
| `fg`/`bg`  | Foreground/bg job   |                          |
| `nice`     | Start with priority | `-n`                     |
| `renice`   | Change priority     | `-p`, `-n`               |

---

## 💽 11. Disk, Mount & USB Tools

| Command     | Description           | Notes                     |
|-------------|-----------------------|---------------------------|
| `lsblk`     | List block devices    |                           |
| `blkid`     | Show UUID             |                           |
| `mount`     | Mount drive           | `mount /dev/sdb1 /mnt`    |
| `umount`    | Unmount               | `umount /mnt`             |
| `fdisk -l`  | Partition info        |                           |
| `parted`    | Partition tool        | `parted /dev/sda`         |

---

## 🧩 12. Boot & Service Management

| Command       | Description        | Options                       |
|---------------|--------------------|-------------------------------|
| `systemctl`   | Manage services    | `start`, `stop`, `status`     |
| `service`     | Legacy control     |                               |
| `journalctl`  | System logs        | `-xe`, `--since`, `-u`        |
| `reboot`      | Restart system     |                               |
| `shutdown`    | Shutdown system    | `-h now`, `-r now`            |

---

## 🧪 13. Pentesting Tools (Kali)

| Tool         | Description             | Example                          |
|--------------|-------------------------|----------------------------------|
| `nmap`       | Network scanner         | `-A -T4 -p-`                     |
| `metasploit` | Exploit framework       | `msfconsole`                     |
| `hydra`      | Brute-force             | `-l user -P passlist -t 4`       |
| `sqlmap`     | SQLi tool               | `-u <url> --dbs`                 |
| `john`       | Password cracker        | `john hashes.txt`                |
| `airmon-ng`  | Monitor mode            | `airmon-ng start wlan0`          |
| `aircrack-ng`| WiFi cracking           | `aircrack-ng file.cap`           |
| `dirb`       | Web dir brute force     | `dirb http://target.com`         |
| `nikto`      | Web vulnerability scan  | `nikto -h <host>`                |
| `burpsuite`  | Web proxy toolkit       | GUI-based                        |

---

## 🎨 14. Miscellaneous Commands

| Command     | Description          | Notes                      |
|-------------|----------------------|----------------------------|
| `uname -a`  | Kernel/system info   | `-r` for version only      |
| `date`      | Show date            | `"+%Y-%m-%d"`              |
| `cal`       | Calendar             | `cal 2025`                 |
| `hostname`  | Show/set hostname    | `hostnamectl`              |
| `clear`     | Clear terminal       |                            |
| `echo`      | Output text/vars     | `echo $HOME`               |
| `env`       | Show environment     |                            |
| `sleep`     | Wait time            | `sleep 5`                  |
| `watch`     | Repeat command       | `watch -n 1 uptime`        |

---

## 🎯 15. Fun & Eye-Candy Commands

| Command     | Description         | Example                   |
|-------------|---------------------|---------------------------|
| `figlet`    | ASCII text art      | `figlet Hello`            |
| `toilet`    | Fancier text art    | `toilet -F metal Kali`    |
| `cowsay`    | Talking cow         | `cowsay Moo!`             |
| `lolcat`    | Rainbow output      | `echo Kali | lolcat`      |
| `cmatrix`   | Matrix rain         | `cmatrix`                 |
| `sl`        | Steam train         | Fun if you mistype `ls`   |

---

## 💡 Tips & Tricks

| Shortcut / Tip                   | Description                        |
|----------------------------------|------------------------------------|
| `!!`                             | Repeat last command                |
| `!sudo`                          | Repeat last as sudo                |
| `ctrl + r`                       | Search command history             |
| `cmd1 && cmd2`                   | Run 2nd if 1st succeeds            |
| `cmd1 || cmd2`                   | Run 2nd if 1st fails               |
| `ls | grep txt`                  | Search in output                   |
| `du -sh *`                       | Show folder/file sizes             |
| `rsync -avh src/ dest/`          | Sync directories                   |
| `scp file user@host:/path/`      | Secure copy via SSH                |
| `chmod +x script.sh && ./script.sh` | Make & run script               |
| `cd -`                           | Go back to previous directory      |

---

## 📄 References

- [Kali Linux Docs](https://www.kali.org/docs/)
- [Debian APT Guide](https://wiki.debian.org/apt)
- [Linux Kernel Documentation](https://www.kernel.org/doc/html/latest/)

---

> 🔐 Stay curious, stay ethical. Happy hacking!
