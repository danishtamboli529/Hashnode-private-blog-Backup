---
title: "🧠 Top 5 Intermediate Level Linux Commands 🐧💻"
seoTitle: "🧠 Top 5 Intermediate Level Linux Commands 🐧💻"
seoDescription: "Learn the top 5 intermediate Linux commands to manage files, processes, permissions, and more efficiently. Ideal for developers and sysadmins"
datePublished: Sat Jul 26 2025 22:39:35 GMT+0000 (Coordinated Universal Time)
cuid: cmdku1rr3000m02lbb87ufffe
slug: top-5-intermediate-level-linux-commands
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/4Mw7nkQDByk/upload/6c7ad3639e866b81ad9101ba9486b988.jpeg
tags: shell-scripting, linux-commands, linux-tips, techlearning, linuxfordevelopers, commandlinemagic, intermediatelinux, sysadminlife

---

These **intermediate-level commands** will help you manage files, processes, permissions, and more efficiently. Let's dive in! 🔧

---

### 1\. 📂 `rsync` – Remote Syncing & Backup Tool

📦 **What it does:**  
`rsync` is a powerful command-line tool to **copy and synchronize files/directories** between local and remote systems.

🛠️ **Real-life Example:**  
Backup your project folder to an external drive or a remote server:

```bash
rsync -avh /home/user/project/ /mnt/backup/project/
```

📌 **Useful Options:**

* `-a`: Archive mode (preserves permissions, links)
    
* `-v`: Verbose (shows progress)
    
* `-h`: Human-readable format
    

🚀 **Pro Tip:**  
Sync with a remote server using SSH:

```bash
rsync -avz /home/user/ user@server:/backup/
```

---

### 2\. 🔍 `grep` – Search Text Using Patterns

📦 **What it does:**  
`grep` searches for **specific text or patterns** in files — great for scanning logs or configuration files.

🛠️ **Real-life Example:**  
Find all errors in a log file:

```bash
grep "ERROR" /var/log/syslog
```

📌 **Other Uses:**

* Case-insensitive search: `grep -i`
    
* Show line numbers: `grep -n`
    
* Invert match (show non-matching lines): `grep -v`
    

🚀 **Pro Tip:**  
Combine with `ps` to find running programs:

```bash
ps aux | grep apache
```

---

### 3\. ⚙️ `chmod` – Change File Permissions

📦 **What it does:**  
`chmod` lets you **change file or folder permissions**, controlling who can read, write, or execute files.

🛠️ **Real-life Example:**  
Make a script file executable:

```bash
chmod +x script.sh
```

📌 **Permission Values:**

* `r` = read = 4
    
* `w` = write = 2
    
* `x` = execute = 1
    

📊 **Numeric Example:**

```bash
chmod 755 myfile.sh
```

Means: Owner (7 = rwx), Group (5 = r-x), Others (5 = r-x)

---

### 4\. 📈 `du` – Disk Usage Analyzer

📦 **What it does:**  
`du` shows how much **disk space** a file or directory is using.

🛠️ **Real-life Example:**  
Check which folders are taking up space:

```bash
du -h --max-depth=1 /home/user/
```

📌 **Useful Options:**

* `-h`: Human-readable (MB, GB)
    
* `--max-depth=1`: Only top-level folders
    

🚀 **Pro Tip:**  
Combine with `sort` to list by size:

```bash
du -sh * | sort -h
```

---

### 5\. 🔄 `kill` – Terminate a Running Process

📦 **What it does:**  
`kill` allows you to **stop a process** using its Process ID (PID).

🛠️ **Real-life Example:**  
Stop a program that’s stuck or using too many resources:

```bash
kill 1234
```

(Where `1234` is the PID)

📌 **Find the PID first:**

```bash
ps aux | grep firefox
```

🚀 **Force Kill:**  
If the process doesn’t stop:

```bash
kill -9 1234
```

---

## ✅ Summary Table

| ⚙️ Command | 💡 What It Does | 🔍 Real-World Use |
| --- | --- | --- |
| `rsync` | Sync and back up files | Backup local projects to server or drive |
| `grep` | Search text with patterns | Find "ERROR" lines in log files |
| `chmod` | Change file permissions | Make scripts executable or restrict access |
| `du` | Check disk usage | Find what’s using up disk space |
| `kill` | Terminate running processes | Stop frozen or high-resource programs |

---

### 🏁 Conclusion

These **intermediate Linux commands** give you greater **control over your system** and are essential for developers, sysadmins, or power users. They’re the bridge between basic navigation and advanced system management. 🧰🔥

Keep practicing, combine them in shell scripts, and soon you’ll be scripting your way through any task like a Linux ninja! 🥷🐧

---