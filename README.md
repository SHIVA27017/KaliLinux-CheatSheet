# 🐱‍💻 Top Kali Linux Commands: A Complete Cheat Sheet

<img src="images/kali-banner.png" alt="Kali Linux" width="600"/>

## 👋 Welcome, Curious Hackers & Self-Starters!

This cheat sheet was crafted from the ground up by a Linux enthusiast with a non-technical background, proving that with enough curiosity and consistency, anyone can break into the world of ethical hacking and system operations.

---

A beginner-to-advanced reference guide to mastering Kali Linux commands. Organized into clear categories, it includes essential system commands, networking tools, user management, file operations, pentesting utilities, and productivity tips — all with brief explanations for fast learning and real-world application.

## 📚 Contents

- [🐱‍💻 Kali Linux Commands Cheat Sheet](#-kali-linux-commands-cheat-sheet)
  - [📚 Contents](#-contents)
  - [📁 1. File \& Directory Management](#-1-file--directory-management)
  - [🧠 2. File Viewing \& Editing](#-2-file-viewing--editing)
  - [👥 3. User Management](#-3-user-management)
  - [🌐 4. Network Commands](#-4-network-commands)
  - [🗃️ 5. Package Management (APT)](#️-5-package-management-apt)
  - [🔐 6. Permissions \& Ownership](#-6-permissions--ownership)
  - [📦 7. Archiving \& Compression](#-7-archiving--compression)
  - [🧪 8. System Monitoring](#-8-system-monitoring)
  - [🔍 9. Search \& Filter Commands](#-9-search--filter-commands)
  - [🛠️ 10. Process Management](#️-10-process-management)
  - [📡 11. Disk, Mount \& USB Tools](#-11-disk-mount--usb-tools)
  - [⚙️ 12. Boot \& Service Management](#️-12-boot--service-management)
  - [🎯 13. Pentesting Tools (Kali)](#-13-pentesting-tools-kali)
  - [🧩 14. Miscellaneous Commands](#-14-miscellaneous-commands)
  - [🎨 15. Fun \& Eye-Candy Commands](#-15-fun--eye-candy-commands)
  - [📌 Tips](#-tips)
  - [✅ References](#-references)

---

## 📁 1. File & Directory Management

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `ls`      | List directory contents   | `-l`, `-a`, `-h`                    |
| `cd`      | Change directory          | `cd ..`, `cd ~`                     |
| `pwd`     | Show current directory    | —                                   |
| `mkdir`   | Create new directory      | `-p`                                |
| `rm`      | Delete files/directories  | `-r`, `-f`                          |
| `cp`      | Copy files/directories    | `-r`, `-v`                          |
| `mv`      | Move or rename            | —                                   |
| `touch`   | Create empty file         | —                                   |
| `tree`    | Display directory tree    | `-L <level>`                        |

---

## 🧠 2. File Viewing & Editing

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `cat`     | View file content         | `-n`                                |
| `less`    | Scrollable view           | `/`, `q`                            |
| `more`    | Paged view                | Space, `q`                          |
| `head`    | First lines of file       | `-n <number>`                       |
| `tail`    | Last lines of file        | `-f`                                |
| `nano`    | Simple text editor        | Ctrl+O, Ctrl+X                      |
| `vim`     | Advanced text editor      | `:wq`, `i`                          |

---

## 👥 3. User Management

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `whoami`  | Show current user         | —                                   |
| `id`      | Show UID/GID              | —                                   |
| `adduser` | Add a user                | `adduser <username>`                |
| `passwd`  | Change password           | —                                   |
| `su`      | Switch user               | `su -`                              |
| `sudo`    | Run as superuser          | `sudo <command>`                    |
| `users`   | Show logged in users      | —                                   |
| `groups`  | Show user groups          | `groups <username>`                 |

---

## 🌐 4. Network Commands

| Command      | Description             | Common Options                      |
|--------------|-------------------------|-------------------------------------|
| `ifconfig`   | Show interfaces         | (deprecated)                        |
| `ip`         | Modern alternative      | `ip a`, `ip r`                      |
| `ping`       | Test connection         | `-c`, `-i`                          |
| `netstat`    | Network stats           | `-tulpn`                            |
| `ss`         | Socket stats            | `-ltnp`                             |
| `traceroute` | Trace route to host     | `traceroute <host>`                |
| `nslookup`   | DNS lookup              | `nslookup google.com`              |
| `dig`        | Advanced DNS tool       | `+short`, `ANY`, `MX`              |
| `nmap`       | Network scanner         | `-sS -A -T4 -p- <target>`          |
| `wget`       | Download from URL       | `-c`, `-O`                         |
| `curl`       | Transfer via URL        | `-I`, `-O`, `-X POST`, `-d`        |

---

## 🗃️ 5. Package Management (APT)

| Command             | Description              | Common Options                      |
|---------------------|--------------------------|-------------------------------------|
| `apt update`        | Refresh package list     | —                                   |
| `apt upgrade`       | Upgrade packages         | `-y`                                |
| `apt install`       | Install package          | `-y`, `--no-install-recommends`     |
| `apt remove`        | Remove package           | `--purge`                           |
| `apt autoremove`    | Remove unused packages   | —                                   |
| `dpkg -i file.deb`  | Manual .deb install      | —                                   |
| `apt-cache search`  | Search for packages      | —                                   |

---

## 🔐 6. Permissions & Ownership

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `chmod`   | Change file permissions   | `+x`, `755`, `644`, `u+x`           |
| `chown`   | Change owner              | `user:group`                        |
| `umask`   | Default permission mask   | `umask 022`                         |
| `ls -l`   | View permissions          | —                                   |

---

## 📦 7. Archiving & Compression

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `tar`     | Archive files             | `-cvf`, `-xvf`, `-czvf`, `-xzvf`    |
| `gzip`    | Compress file             | —                                   |
| `gunzip`  | Decompress `.gz`          | —                                   |
| `zip`     | Create zip archive        | `-r`                                |
| `unzip`   | Extract zip               | —                                   |

---

## 🧪 8. System Monitoring

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `top`     | Real-time process viewer | —                                   |
| `htop`    | Advanced viewer           | (requires install)                  |
| `df -h`   | Disk usage                | `-h`                                |
| `du -sh`  | Directory size            | `-s`, `-h`                          |
| `free -h` | Memory usage              | —                                   |
| `uptime`  | System uptime/load        | —                                   |

---

## 🔍 9. Search & Filter Commands

| Command   | Description               | Common Options                      |
|-----------|---------------------------|-------------------------------------|
| `grep`    | Search in files           | `-i`, `-r`, `-n`, `--color`         |
| `find`    | Find files                | `-name`, `-type`, `-exec`          |
| `locate`  | Fast file search          | Use `updatedb` to refresh           |
| `which`   | Show command path         | —                                   |

---

## 🛠️ 10. Process Management

| Command       | Description                 | Common Options             |
|---------------|-----------------------------|----------------------------|
| `ps aux`      | Show processes              | —                          |
| `kill`        | Terminate by PID            | `-9`                       |
| `killall`     | Terminate by name           | `killall firefox`          |
| `jobs`        | Show background jobs        | —                          |
| `bg` / `fg`   | Resume background/foreground| —                          |
| `nice`        | Set process priority        | `-n`                       |
| `renice`      | Change priority of PID      | `-n`, `-p`                 |

---

## 📡 11. Disk, Mount & USB Tools

| Command     | Description               | Common Options                      |
|-------------|---------------------------|-------------------------------------|
| `lsblk`     | List block devices        | —                                   |
| `blkid`     | Show UUIDs                | —                                   |
| `mount`     | Mount devices             | `/dev/sdb1 /mnt`                    |
| `umount`    | Unmount devices           | `/mnt`                              |
| `fdisk -l`  | List partitions           | —                                   |
| `parted`    | Partition tool            | `parted /dev/sda`                   |

---

## ⚙️ 12. Boot & Service Management

| Command        | Description               | Common Options            |
|----------------|---------------------------|---------------------------|
| `systemctl`    | Manage services/systemd   | `start`, `stop`, `status` |
| `service`      | Init system services      | —                         |
| `journalctl`   | View logs                 | `-xe`, `-u`, `--since`    |
| `reboot`       | Reboot system             | —                         |
| `shutdown`     | Power off system          | `-h now`                  |

---

## 🎯 13. Pentesting Tools (Kali)

| Tool         | Description             | Common Usage                    |
|--------------|-------------------------|----------------------------------|
| `nmap`       | Port scanner            | `-A -T4 -p- <IP>`               |
| `metasploit` | Exploitation framework  | `msfconsole`                    |
| `hydra`      | Brute force login       | `-l user -P pass.txt <host>`    |
| `sqlmap`     | SQL injection test      | `--dbs -u <url>`                |
| `john`       | Password cracker        | `john hash.txt`                 |
| `airmon-ng`  | Monitor mode            | `start wlan0`                   |
| `aircrack-ng`| Crack Wi-Fi passwords   | `aircrack-ng capture.cap`       |
| `dirb`       | Web dir brute-forcer    | `dirb http://example.com/`      |
| `nikto`      | Web scanner             | `nikto -h <host>`              |
| `burpsuite`  | Web proxy GUI           | GUI tool                        |

---

## 🧩 14. Miscellaneous Commands

| Command       | Description              | Notes                          |
|---------------|--------------------------|--------------------------------|
| `uname -a`    | Kernel/system info       | `-r` for kernel version        |
| `date`        | Current date/time        | `"+%Y-%m-%d"` format           |
| `cal`         | Calendar                 | `cal 2025`                     |
| `hostname`    | Hostname info            | `hostnamectl set-hostname`    |
| `clear`       | Clear screen             | —                              |
| `echo`        | Output text/var          | `echo $PATH`                   |
| `env`         | Environment variables    | —                              |
| `sleep`       | Delay execution          | `sleep 5`                      |
| `watch`       | Run periodically         | `watch -n 2 uptime`            |
| `basename`    | Strip path               | `basename /file/path.txt`      |
| `dirname`     | Directory from path      | `dirname /file/path.txt`       |

---

## 🎨 15. Fun & Eye-Candy Commands

| Command     | Description           | Notes                             |
|-------------|------------------------|-----------------------------------|
| `figlet`    | ASCII banner text     | `figlet Hello`                    |
| `toilet`    | Fancy ASCII           | `toilet -F metal "Hack"`          |
| `cowsay`    | ASCII cow speaks      | `cowsay Hello`                    |
| `lolcat`    | Rainbow output        | `echo Hello | lolcat`             |
| `cmatrix`   | Matrix animation      | `cmatrix`                         |
| `sl`        | Steam loco animation  | `sl` (joke tool)                  |

---

## 📌 Tips

- Use `man <command>` or `<command> --help` for more info.
- Combine: `cmd1 && cmd2`
- Pipe output: `ls | grep txt`
- Redirect: `ls > out.txt`
- Background: `sleep 10 &`

---

## ✅ References

- [Kali Linux Docs](https://www.kali.org/docs/)
- [Linux Command TLDR](https://tldr.sh/)
- [Linux Handbook](https://linuxhandbook.com/)
