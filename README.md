# 🐱‍💻 Top Kali Linux Commands: A Complete Cheat Sheet

<img src="https://www.kali.org/wallpapers/images/2024/kali-ferrofluid.jpg" alt="Kali Linux" width="1000" height="500"/>

## 👋 Welcome, Curious Hackers & Self-Starters!

This cheat sheet was crafted from the ground up by a Linux enthusiast with a non-technical background, proving that with enough curiosity and consistency, anyone can break into the world of ethical hacking and system operations.

---

## 📚 Contents

- [1. File & Directory Management](#1-file--directory-management)
- [2. File Viewing & Editing](#2-file-viewing--editing)
- [3. User Management](#3-user-management)
- [4. Network Commands](#4-network-commands)
- [5. Package Management (APT)](#5-package-management-apt)
- [6. Permissions & Ownership](#6-permissions--ownership)
- [7. Archiving & Compression](#7-archiving--compression)
- [8. System Monitoring](#8-system-monitoring)
- [9. Search & Filter Commands](#9-search--filter-commands)
- [10. Process Management](#10-process-management)
- [11. Disk, Mount & USB Tools](#11-disk-mount--usb-tools)
- [12. Boot & Service Management](#12-boot--service-management)
- [13. Pentesting Tools (Kali)](#13-pentesting-tools-kali)
- [14. Miscellaneous Commands](#14-miscellaneous-commands)
- [15. Fun & Eye-Candy Commands](#15-fun--eye-candy-commands)
- [🧠 Tips & Tricks](#-tips--tricks)
- [📄 References](#-references)
---

## 📁 1. File & Directory Management

| Command     | Description               | Common Options                                             |
|-------------|---------------------------|------------------------------------------------------------|
| `ls`        | List directory contents   |`-a`(include hidden),`-l`(long format),-h`(human-readable)  |
| `cd`        | Change directory          | `..`, `~`                                                  |
| `pwd`       | Show current directory    | —                                                          |
| `mkdir`     | Create new directory      | `-p` (create parent)                                       |
| `rm`        | Delete files/directories  | `-r` (recursive), `-f` (force)                             |
| `cp`        | Copy files/directories    | `-r` (recursive), `-v` (verbose)                           |
| `mv`        | Move or rename files      | —                                                          |
| `touch`     | Create empty file         | —                                                          |
| `tree`      | Directory structure       | `-L` (limit depth)                                         |

---

## 🧠 2. File Viewing & Editing

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `cat`       | Display file contents     | `-n` (line numbers)                             |
| `less`      | Scrollable file view      | `/`, `q`                                        |
| `more`      | Paged file view           | Space, `q`                                      |
| `head`      | View beginning of file    | `-n` (lines)                                    |
| `tail`      | View end of file          | `-f` (follow live)                              |
| `nano`      | Simple editor             | Ctrl+O (save), Ctrl+X (exit)                    |
| `vim`       | Advanced editor           | `:wq`, `i`, `ESC`                               |

---

## 👥 3. User Management

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `whoami`    | Show current user         | —                                               |
| `id`        | Show user ID/group        | —                                               |
| `adduser`   | Add a user                | `adduser <username>`                            |
| `passwd`    | Change user password      | —                                               |
| `su`        | Switch user               | `su -`                                          |
| `sudo`      | Superuser privilege       | `sudo <cmd>`                                    |
| `users`     | Logged in users           | —                                               |
| `groups`    | Show groups               | `groups <username>`                             |

---

## 🌐 4. Network Commands

| Command       | Description               | Common Options                                  |
|---------------|---------------------------|-------------------------------------------------|
| `ifconfig`    | Show network interfaces   | (legacy)                                        |
| `ip`          | Interface management      | `ip a`, `ip r`                                  |
| `ping`        | Test connection           | `-c` (count), `-i` (interval)                   |
| `netstat`     | Network stats             | `-tulpn`                                        |
| `ss`          | Socket stats              | `-ltnp`                                         |
| `traceroute`  | Trace route               | `traceroute <host>`                             |
| `nslookup`    | DNS lookup                | —                                               |
| `dig`         | Advanced DNS tool         | `ANY`, `+short`, `MX`                           |
| `nmap`        | Port scanner              | `-A` (aggressive), `-T4`, `-p-` (all ports)     |
| `wget`        | Download via HTTP         | `-c` (resume), `-O` (output file)               |
| `curl`        | Data transfer             | `-I` (headers), `-X` (method), `-d` (data)      |

---

## 📦 5. Package Management (APT)

| Command           | Description               | Common Options                                  |
|-------------------|---------------------------|-------------------------------------------------|
| `apt update`      | Update package lists      | —                                               |
| `apt upgrade`     | Upgrade installed packages| `-y` (auto yes)                                 |
| `apt install`     | Install packages          | `--no-install-recommends`, `-y`                 |
| `apt remove`      | Remove a package          | `--purge` (config too)                          |
| `apt autoremove`  | Clean unused packages     | —                                               |
| `dpkg -i`         | Install `.deb` manually   | —                                               |
| `apt-cache search`| Search for packages       | —                                               |

---

## 🔐 6. Permissions & Ownership

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `chmod`     | Change file permissions   | `+x`, `755`, `u+x`                              |
| `chown`     | Change file owner         | `user:group`                                    |
| `umask`     | Default permissions mask  | `umask 022`                                     |
| `ls -l`     | Show permissions          | —                                               |

---

## 🗜️ 7. Archiving & Compression

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `tar`       | Archive files             | `-cvf`, `-xvf`, `-czvf`, `-xzvf`                |
| `gzip`      | Compress file             | —                                               |
| `gunzip`    | Decompress `.gz`          | —                                               |
| `zip`       | Create zip file           | `-r` (recursive)                                |
| `unzip`     | Extract zip               | —                                               |

---

## 📊 8. System Monitoring

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `top`       | Realtime monitor          | —                                               |
| `htop`      | Enhanced top              | (install required)                              |
| `df -h`     | Disk usage                | `-h` (human-readable)                           |
| `du -sh`    | Folder sizes              | `-s` (summary), `-h` (human)                    |
| `free -h`   | Memory usage              | —                                               |
| `uptime`    | System load/uptime        | —                                               |

---

## 🔍 9. Search & Filter Commands

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `grep`      | Search text               | `-i` (ignore case), `-r` (recursive), `--color` |
| `find`      | Search files              | `-name`, `-type`, `-exec`                       |
| `locate`    | Fast file search          | —                                               |
| `which`     | Command path              | —                                               |

---

## ⚙️ 10. Process Management

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `ps aux`    | Show all processes        | —                                               |
| `kill`      | Kill by PID               | `-9` (force)                                    |
| `killall`   | Kill by name              | `killall firefox`                              |
| `jobs`      | Show jobs                 | —                                               |
| `fg` / `bg` | Foreground/background     | —                                               |
| `nice`      | Set priority              | `-n` (nice value)                               |
| `renice`    | Change process priority   | `-p` (PID), `-n`                                |

---

## 💽 11. Disk, Mount & USB Tools

| Command     | Description               | Common Options                                  |
|-------------|---------------------------|-------------------------------------------------|
| `lsblk`     | List block devices        | —                                               |
| `blkid`     | Show UUID info            | —                                               |
| `mount`     | Mount device              | `mount /dev/sdb1 /mnt`                          |
| `umount`    | Unmount device            | `umount /mnt`                                   |
| `fdisk -l`  | Partition info            | —                                               |
| `parted`    | Partition manager         | `parted /dev/sda`                               |

---

## 🧩 12. Boot & Service Management

| Command        | Description             | Common Options                                  |
|----------------|-------------------------|-------------------------------------------------|
| `systemctl`    | Manage systemd services | `start`, `stop`, `status`, `restart`           |
| `service`      | Legacy service mgmt     | —                                               |
| `journalctl`   | View logs               | `-xe`, `-u`, `--since`                          |
| `reboot`       | Restart system          | —                                               |
| `shutdown`     | Shutdown system         | `-h now` (halt now)                             |

---

## 🧪 13. Pentesting Tools (Kali)

| Tool          | Description              | Common Usage                                   |
|---------------|--------------------------|------------------------------------------------|
| `nmap`        | Port scanner             | `-A`, `-T4`, `-p-`                              |
| `metasploit`  | Exploit framework        | `msfconsole`                                   |
| `hydra`       | Brute-force tool         | `-l`, `-P`, `-t`                                |
| `sqlmap`      | SQL injection tester     | `--dbs`, `-u`                                   |
| `john`        | Password cracker         | `john hashes.txt`                              |
| `airmon-ng`   | Enable monitor mode      | `airmon-ng start wlan0`                        |
| `aircrack-ng` | Crack WiFi passwords     | `aircrack-ng file.cap`                         |
| `dirb`        | Web directory brute force| `dirb http://site.com`                         |
| `nikto`       | Web vulnerability scan   | `nikto -h <target>`                            |
| `burpsuite`   | Web proxy tool           | GUI launcher                                   |

---

## 🎨 14. Miscellaneous Commands

| Command     | Description               | Notes                                           |
|-------------|---------------------------|-------------------------------------------------|
| `uname -a`  | Kernel info               | `-r` for version only                          |
| `date`      | Date/time display         | `"+%Y-%m-%d"`                                  |
| `cal`       | Calendar view             | `cal 2025`                                     |
| `hostname`  | Show/set hostname         | `hostnamectl`                                  |
| `clear`     | Clear terminal            | —                                               |
| `echo`      | Output text               | `echo $HOME`                                   |
| `env`       | Show environment          | —                                               |
| `sleep`     | Delay execution           | `sleep 5`                                      |
| `watch`     | Run periodically          | `watch -n 1 uptime`                            |

---

## 🎯 15. Fun & Eye-Candy Commands

| Command     | Description               | Notes                                           |
|-------------|---------------------------|-------------------------------------------------|
| `figlet`    | ASCII art text            | `figlet Hello`                                 |
| `toilet`    | Fancy ASCII art           | `toilet -F metal Kali`                         |
| `cowsay`    | Cow with message          | `cowsay Moo!`                                  |
| `lolcat`    | Rainbow output            | `echo Kali | lolcat`                           |
| `cmatrix`   | Matrix effect             | Terminal matrix rain                           |
| `sl`        | Steam engine animation    | Funny alias for mistyping `ls`                 |

---

## 🧠 Tips & Tricks

| Tip / Trick                          | Description                                    |
|--------------------------------------|------------------------------------------------|
| `!!`                                 | Re-run last command                            |
| `!sudo`                              | Rerun last with sudo                           |
| `ctrl + r`                           | Search command history                         |
| `cmd1 && cmd2`                       | Run 2nd only if 1st succeeds                   |
| `cmd1 || cmd2`                       | Run 2nd only if 1st fails                      |
| `ls | grep txt`                      | Search listing output                          |
| `du -sh *`                           | Show size of all folders/files                 |
| `rsync -avh source/ dest/`           | Fast directory sync                            |
| `scp file user@host:/path/`          | Copy over SSH                                  |
| `chmod +x script.sh && ./script.sh` | Make and run script                            |
| `cd -`                               | Go to previous directory                       |

---

## 📄 References

- [Kali Linux Official Docs](https://www.kali.org/docs/)
- [Debian APT Guide](https://wiki.debian.org/apt)
- [Linux Kernel Docs](https://www.kernel.org/doc/html/latest/)

