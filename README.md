#  Documentation: Operating System - Ubuntu

---

## 📚 Table of Contents

1. [🐧 Documentation: Operating System - Ubuntu](#-documentation-operating-system---ubuntu)
2. [📘 1. What is Ubuntu?](#-1-what-is-ubuntu)
3. [🧠 Why Use Ubuntu?](#-why-use-ubuntu)
4. [💻 3. Ubuntu Versions & Releases](#-3-ubuntu-versions--releases)
5. [🔧 4. System Requirements](#-4-system-requirements)
6. [🔒 5. Security Features](#-5-security-features)
7. [☁️ 6. Ubuntu Use Cases](#-6-ubuntu-use-cases)
8. [🛠️ 7. Common Commands](#-7-common-commands)
9. [🧠 What is Software Management in Ubuntu?](#-what-is-software-management-in-ubuntu)
10. [📦 Key Software Management Tools in Ubuntu](#-key-software-management-tools-in-ubuntu)
11. [🔍 Check if a Package Is Installed](#-check-if-a-package-is-installed)
12. [✅ Summary: Removal Commands](#-summary-removal-commands)
13. [🧠 Service Command Used in Ubuntu](#-service-command-used-in-ubuntu)
14. [🏁 Conclusion](#-conclusion)

---




## 📘 1. What is Ubuntu?
Ubuntu is a **free and open-source Linux-based operating system** developed and maintained by **Canonical Ltd.** It is one of the most popular Linux distributions in the world, known for its ease of use, regular updates, and strong community support.

- First released in **October 2004**
- Based on **Debian Linux**
- Uses **APT package manager** and `.deb` packages
- Available in **Desktop**, **Server**, **Cloud**, and **Core (IoT)** versions

---

## 🧠 **Why Use Ubuntu?**

Ubuntu is widely chosen by developers, system admins, and even casual users because it's:

---

### ✅ **1. Free & Open Source**
- No licensing fees
- You have full access to the source code
- Supported by a large open-source community

---

### ✅ **2. User-Friendly**
- Simple and clean **GNOME desktop interface**
- Easy to install and use, even for Linux beginners
- Large library of preinstalled and easily installable software

---

### ✅ **3. Developer-Friendly**
- Built-in support for:
  - Python, Java, Node.js, Docker, Git, etc.
- Great for **coding, scripting, and automation**
- Large ecosystem of development tools

---

### ✅ **4. Strong Community & Documentation**
- Huge online community (AskUbuntu, StackOverflow)
- Extensive official docs and tutorials
- Tons of support for troubleshooting

---

### ✅ **5. Regular & Reliable Updates**
- **LTS (Long Term Support)** versions with 5 years of updates
- Predictable release cycles
- Frequent security patches and bug fixes

---

### ✅ **6. Secure by Design**
- Built-in firewall (UFW)
- AppArmor security module
- Unattended upgrades available
- Full-disk encryption optional at install time

---

### ✅ **7. Cloud & DevOps Ready**
- Official support by **AWS, Azure, GCP**
- Common base image for Docker containers
- Works well with Jenkins, Ansible, Kubernetes, etc.

---

### ✅ **8. Lightweight & Flexible**
- Can run on old hardware or minimal VMs
- Great for IoT devices with **Ubuntu Core**
  
---

## 💻 3. Ubuntu Versions & Releases

| Version       | Type  | Release Month | Support Until |
|---------------|-------|----------------|----------------|
| Ubuntu 22.04  | LTS   | April 2022     | April 2027 (standard) |
| Ubuntu 20.04  | LTS   | April 2020     | April 2025     |
| Ubuntu 23.10  | Interim | Oct 2023      | July 2024      |

- **LTS** = Long-Term Support (5 years support)
- Non-LTS releases are supported for 9 months

## 🔧 4. System Requirements

### Ubuntu Desktop (Minimal):

- **2 GHz dual-core CPU**
- **4 GB RAM**
- **25 GB disk space**
- **Internet connection**

For servers and containers, requirements are much lower.

## 🔒 5. Security Features

- Built-in **firewall** (UFW)
- **AppArmor** for application-level security
- **Unattended security updates**
- Optional full-disk encryption during install

## ☁️ 6. Ubuntu Use Cases

| Use Case         | Example                   |
|------------------|---------------------------|
| Desktop OS       | Personal laptops, offices |
| Web Servers      | Apache/Nginx hosting      |
| DevOps & CI/CD   | Jenkins, Ansible, Docker  |
| Cloud Images     | AWS EC2 Ubuntu AMIs       |
| Containers       | Docker base images        |
| IoT              | Ubuntu Core (lightweight) |

## 🛠️ 7. Common Commands

```bash
sudo apt update           # Update package index
sudo apt install nginx    # Install a package
sudo systemctl status     # Check service status
lsb_release -a            # Show Ubuntu version
```

## 🧠 **What is a Software Management in Ubuntu?**

> Software management in Ubuntu refers to the **tools, services, and processes** used to **install, update, upgrade, remove, and maintain software packages** on your system.

---

## 📦 **Key Software Management Tools in Ubuntu**

Ubuntu is based on **Debian**, so it uses **APT** (Advanced Package Tool) for package management.

### 🔹 1. **APT (Advanced Package Tool)**
```bash
sudo apt update          # Refreshes the package index
sudo apt install nginx   # Installs a package
sudo apt upgrade         # Updates installed packages
```
- Backend tool that manages `.deb` packages
- Resolves dependencies automatically
- Pulls from online repositories

## 🔧 ** If Installed Using APT how to remove the package**

### 🔹 Remove a package:
```bash
sudo apt remove <package-name>
```
➡️ Removes the software **but keeps** configuration files.

### 🔹 Example:
```bash
sudo apt remove nginx
```
### 🔹 Remove + config files (cleaner):
```bash
sudo apt purge <package-name>
```
➡️ Removes software **and** its config files (from `/etc/`).

### 🔹 Example:
```bash
sudo apt purge nginx
```
### 🔹 Clean unused dependencies:
```bash
sudo apt autoremove
```
➡️ Cleans leftover packages no longer needed (e.g. after uninstalling).

---
### 🔹 2. **DPKG (Debian Package Manager)**
```bash
sudo dpkg -i package.deb   # Install a local .deb package
sudo dpkg -l               # List all installed packages
```
- Lower-level tool
- No dependency resolution (APT is smarter)

## 📦 ** If Installed Using DPKG how to remove the package**

```bash
sudo dpkg -r <package-name>
```
➡️ Use this if you installed a `.deb` file manually.

Example:
```bash
sudo dpkg -r google-chrome-stable
```
---

### 🔹 3. **Snap**
```bash
sudo snap install vlc
```
- Containerized packages
- Developed by Canonical (Ubuntu’s parent company)
- Updates automatically in the background

---
## 📦 ** If Installed Using Snap, how to remove**

```bash
sudo snap remove <package-name>
```
Example:
```bash
sudo snap remove vlc
```
---

### 🔹 4. **Ubuntu Software Center (GUI)**
- User-friendly graphical interface
- Lets you search, install, and remove software
- Ideal for non-terminal users

---

## 🖱️ ** Remove via GUI (Ubuntu Software Center)**

1. Open **Ubuntu Software Center**
2. Go to **Installed**
3. Find the software and click **"Remove"**

✅ Useful for users who prefer a graphical interface.

---

## 🔍 **Check if a Package Is Installed**

```bash
dpkg -l | grep <package-name>
```
Example:
```bash
dpkg -l | grep nginx
```

---

## ✅ Summary: Removal Commands

| Installation Type | Remove Command                         |
|-------------------|-----------------------------------------|
| APT               | `sudo apt remove <pkg>`                |
| APT + Config      | `sudo apt purge <pkg>`                 |
| Snap              | `sudo snap remove <pkg>`               |
| DPKG (.deb)       | `sudo dpkg -r <pkg>`                   |
| GUI               | Ubuntu Software > Installed > Remove   |

---

## 🧠 **Service commands in Ubuntu**

In Ubuntu, **`service` commands** are used to manage system services (start, stop, restart, etc.). These commands are wrappers around `systemctl` (for systemd) or older init systems.

Here’s a list of **commonly used `service` commands** in Ubuntu:

---

### ✅ Basic Syntax

```bash
sudo service <service_name> <command>
```

**Example:**
```bash
sudo service apache2 start
```
---

### 🔧 Common Service Commands

| Command | Description |
|--------|-------------|
| `start` | Starts the service |
| `stop` | Stops the service |
| `restart` | Restarts the service |
| `reload` | Reloads config without stopping the service (if supported) |
| `status` | Shows the current status of the service |
| `enable` | Not supported with `service`; use `systemctl` |
| `disable` | Not supported with `service`; use `systemctl` |

---

### 💡 Examples

```bash
sudo service ssh status
sudo service nginx restart
sudo service mysql stop
sudo service cron reload
```
---

### 🆚 `service` vs `systemctl`

Ubuntu (since 15.04) uses **`systemd`**, so `systemctl` is preferred now:

#### Equivalent `systemctl` Commands

| Old `service` Command       | New `systemctl` Command                      |
|----------------------------|----------------------------------------------|
| `sudo service nginx start` | `sudo systemctl start nginx`                 |
| `sudo service nginx stop`  | `sudo systemctl stop nginx`                  |
| `sudo service nginx status`| `sudo systemctl status nginx`               |
| N/A                        | `sudo systemctl enable nginx`                |
| N/A                        | `sudo systemctl disable nginx`               |

---

### 🔍 List All Services

```bash
# Using service (limited list)
service --status-all

# Using systemctl (preferred)
systemctl list-units --type=service
```
---

## 🏁 **Conclusion**

Ubuntu stands out as one of the most reliable, user-friendly, and versatile Linux distributions available today. Whether you're a beginner exploring Linux for the first time, a developer building modern applications, or a system administrator managing large-scale infrastructure, **Ubuntu provides a powerful and secure environment** to get the job done.

From its rich ecosystem of open-source tools and frequent LTS releases to its seamless integration with cloud, container, and DevOps technologies, Ubuntu offers everything you need to build, deploy, and manage software effectively.

With robust software management options (`APT`, `Snap`, `DPKG`), intuitive service control (`service`, `systemctl`), and strong community support, Ubuntu continues to empower millions of users and organizations around the globe.

---

## Contacts

| Name         | Email Address                                 |
|--------------|-----------------------------------------------|
| Adil Nawaz | adil.nawaz.snaatak@mygurukulam.co           |

---

## References

| **Title**                        | **Link**                                                                                      |
|----------------------------------|-----------------------------------------------------------------------------------------------|
| Ubuntu Official Documentation  | (https://help.ubuntu.com)          |
| Ubuntu Releases List           | (https://wiki.ubuntu.com/Releases) |

