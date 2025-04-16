#  Documentation: Operating System - Ubuntu


| Created     | Version | Author        | Comment | Reviewer         |
|-------------|---------|---------------|---------|------------------|
| 15-04-2025  | V1      | Adil Nawaz    |         | Pritam           |
---

Here’s a clean and working **Table of Contents (ToC)** based on your sections and GitHub Markdown anchor format:

---

## 📚 Table of Contents

1. [Introduction](#-1-introduction)  
2. [Why to use Ubuntu?](#-2-why-to-use-ubuntu)  
   - [2.1. Free & Open Source](#-21-free--open-source)  
   - [2.2. User-Friendly](#-22-user-friendly)  
   - [2.3. Developer-Friendly](#-23-developer-friendly)  
   - [2.4. Strong Community & Documentation](#-24-strong-community--documentation)  
   - [2.5. Regular & Reliable Updates](#-25-regular--reliable-updates)  
   - [2.6. Secure by Design](#-26-secure-by-design)  
   - [2.7. Cloud & DevOps Ready](#-27-cloud--devops-ready)  
   - [2.8. Lightweight & Flexible](#-28-lightweight--flexible)  
3. [Ubuntu Versions & Releases](#-3-ubuntu-versions--releases)  
4. [Security Features](#-4-security-features)  
5. [Ubuntu Use Cases](#-5-ubuntu-use-cases)  
6. [What Are Flavours in Linux?](#-6-what-are-flavours-in-linux)  
   - [6.1 Major Flavours of Linux (Distros)](#-61-major-flavours-of-linux-distros)  
7. [Ubuntu Architecture Overview](#-7-ubuntu-architecture-overview)  
   - [7.1. Hardware Layer](#-71-hardware-layer)  
   - [7.2. Linux Kernel](#-72-linux-kernel)  
   - [7.3. System Libraries](#-73-system-libraries)  
   - [7.4. Shell / CLI Interface](#-74-shell--cli-interface)  
   - [7.5. System Services & Daemons](#-75-system-services--daemons)  
   - [7.6. Graphical User Interface (GUI)](#-76-graphical-user-interface-gui)  
   - [7.7. Application Layer](#-77-application-layer)  
8. [What is Software Management in Ubuntu?](#-8-what-is-a-software-management-in-ubuntu)  
   - [8.1. APT (Advanced Package Tool)](#-81-apt-advanced-package-tool)  
   - [8.2. DPKG (Debian Package Manager)](#-82-dpkg-debian-package-manager)  
   - [8.3. Snap](#-83-snap)  
   - [8.4. Ubuntu Software Center (GUI)](#-84-ubuntu-software-center-gui)  
9. [Common Commands](#-9-common-commands)  
   - [9.1 Check if a Package Is Installed](#-91-check-if-a-package-is-installed)  
10. [Service Commands in Ubuntu](#-9-service-commands-in-ubuntu)  
    - [9.1 Common Service Commands](#-91-common-service-commands)  
    - [9.2 List All Services](#-92-list-all-services)  
11. [Conclusion](#-10-conclusion)  
12. [Contacts](#11-contacts)  
13. [References](#12-references)  

---

Let me know if you want this inserted into your README directly or need a downloadable version.


## 📘 1. Introduction
Ubuntu is a **free and open-source Linux-based operating system** developed and maintained by **Canonical Ltd.** It is one of the most popular Linux distributions in the world, known for its ease of use, regular updates, and strong community support.

- First released in **October 2004**
- Based on **Debian Linux**
- Uses **APT package manager** and `.deb` packages
- Available in **Desktop**, **Server**, **Cloud**, and **Core (IoT)** versions

---

## 🧠 2. **Why to use Ubuntu?**

Ubuntu is widely chosen by developers, system admins, and even casual users because it's:

---

### ✅ **2.1. Free & Open Source**
- No licensing fees
- You have full access to the source code
- Supported by a large open-source community

---

### ✅ **2.2. User-Friendly**
- Simple and clean **GNOME desktop interface**
- Easy to install and use, even for Linux beginners
- Large library of preinstalled and easily installable software

---

### ✅ **2.3. Developer-Friendly**
- Built-in support for:
  - Python, Java, Node.js, Docker, Git, etc.
- Great for **coding, scripting, and automation**

---

### ✅ **2.4. Strong Community & Documentation**
- Huge online community (AskUbuntu, StackOverflow)
- Extensive official docs and tutorials
- Tons of support for troubleshooting

---

### ✅ **2.5. Regular & Reliable Updates**
- **LTS (Long Term Support)** versions with 5 years of updates
- Predictable release cycles
- Frequent security patches and bug fixes

---

### ✅ **2.6. Secure by Design**
- Built-in firewall (UFW)
- AppArmor security module
- Unattended upgrades available
- Full-disk encryption optional at install time

---

### ✅ **2.7. Cloud & DevOps Ready**
- Official support by **AWS, Azure, GCP**
- Common base image for Docker containers
- Works well with Jenkins, Ansible, Kubernetes, etc.

---

### ✅ **2.8. Lightweight & Flexible**
- Can run on old hardware or minimal VMs
- Great for IoT devices with **Ubuntu Core**
  
---

## 💻 3. Ubuntu Versions & Releases

| Version       | Type  | Release Month | Support Until |
|---------------|-------|----------------|----------------|
| Ubuntu 22.04  | LTS   | April 2022     | April 2027 (standard) |
| Ubuntu 20.04  | LTS   | April 2020     | April 2025     |
| Ubuntu 23.10  | Interim | Oct 2023      | July 2022     |
| Ubuntu 24.04  | Interim | Oct 2023      | April 2024      |


- **LTS** = Long-Term Support (5 years support)
- Non-LTS releases are supported for 9 months

Great topic! Let's break it down 👇

---

## 🔒 4. Security Features

- Built-in **firewall** (UFW)
- **AppArmor** for application-level security
- **Unattended security updates**
- Optional full-disk encryption during install

---

## ☁️ 5. Ubuntu Use Cases

| Use Case         | Example                   |
|------------------|---------------------------|
| Desktop OS       | Personal laptops, offices |
| Web Servers      | Apache/Nginx hosting      |
| DevOps & CI/CD   | Jenkins, Ansible, Docker  |
| Cloud Images     | AWS EC2 Ubuntu AMIs       |
| Containers       | Docker base images        |
| IoT              | Ubuntu Core (lightweight) |


## 🐧 6. What Are **Flavours in Linux**?

**"flavours"** (or **distributions/distros**) refer to **different versions** of the Linux operating system, built with different goals, tools, and user experiences — but **all share the same Linux kernel**.

---

## 📦 6.1 Major Flavours of Linux (Distros)

| Flavour         | Base       | Package Manager | Target Audience / Use Case |
|-----------------|------------|------------------|-----------------------------|
| **Ubuntu**      | Debian     | APT (`.deb`)     | Beginners, developers, servers, cloud |
| **Debian**      | N/A        | APT (`.deb`)     | Stable, minimal, servers, advanced users |
| **Linux Mint**  | Ubuntu     | APT (`.deb`)     | Beginners, Windows-like interface |
| **Fedora**      | Red Hat    | DNF (`.rpm`)     | Developers, bleeding-edge |
| **CentOS**      | Red Hat    | YUM/DNF (`.rpm`) | Servers (no longer supported, now CentOS Stream) |
| **Rocky Linux** | Red Hat    | DNF (`.rpm`)     | Replacement for CentOS (stable server use) |
| **Arch Linux**  | N/A        | Pacman           | Advanced users, DIY, rolling release |
| **Manjaro**     | Arch       | Pacman           | User-friendly Arch-based |
| **openSUSE**    | SUSE       | Zypper           | Developers, power users, enterprise |
| **Kali Linux**  | Debian     | APT (`.deb`)     | Cybersecurity, ethical hacking |
| **Zorin OS**    | Ubuntu     | APT (`.deb`)     | Windows users switching to Linux |
| **elementary OS** | Ubuntu   | APT (`.deb`)     | Mac-like interface, design-focused |
| **Pop!_OS**     | Ubuntu     | APT (`.deb`)     | Developers, System76 laptops, tiling window manager |
| **Alpine Linux**| N/A        | APK              | Lightweight, containers (e.g. Docker) |

---




## 🏗️ 7. **Ubuntu Architecture Overview**

Ubuntu is built on the **Linux kernel** and structured into multiple **layers** — from the core system up to the graphical interface and applications.

![linux architecture](https://github.com/user-attachments/assets/a476d87b-c185-47db-8058-50f58e03d5a6)



### 🔧 **7.1. Hardware Layer**
- Physical components: CPU, memory, disk, GPU, etc.
- Accessed via drivers managed by the kernel.

---

### 🧠 **7.2. Linux Kernel**
- Core of the system.
- Handles:
  - **Process management**
  - **Memory management**
  - **File systems**
  - **Device drivers**
  - **Networking**
- Ubuntu uses a slightly customized version of the **mainline Linux kernel**.

---

### 📚 **7.3. System Libraries**
- Provides standard APIs and functions used by applications.
- Common ones:
  - `glibc` (C standard library)
  - `libstdc++` (C++ standard library)
  - `libsystemd` (systemd integration)
- Interfaces between user programs and the kernel.

---

### 💻 **7.4. Shell / CLI Interface**
- Bash, Zsh, Fish, etc.
- Enables users to run commands directly.
- Essential for system administration, scripting, and automation.

---

### ⚙️ **7.5. System Services & Daemons**
- Background services (daemons) that run system tasks:
  - `systemd` – init system and service manager
  - `cron` – scheduled jobs
  - `NetworkManager` – network configs
  - `udev` – device management

---

### 🖥️ **7.6. Graphical User Interface (GUI)**
- Desktop Environment (DE): GNOME (default), KDE, XFCE, etc.
- Window Manager: Manages windows, appearance, and user interaction.
- Display Server: X11 (older), Wayland (modern, default in Ubuntu 22.04+)

---

### 📦 **7.7. Application Layer**
- Software installed via package managers:
  - APT (`.deb`)
  - Snap
- User applications: Firefox, LibreOffice, VSCode, GIMP, etc.

---

## 🧠 8. **What is a Software Management in Ubuntu?**

> Software management in Ubuntu refers to the **tools, services, and processes** used to **install, update, upgrade, remove, and maintain software packages** on your system.

---

## 📦 **Key Software Management Tools in Ubuntu**

Ubuntu is based on **Debian**, so it uses **APT** (Advanced Package Tool) for package management.

### 🔹 8.1. **APT (Advanced Package Tool)**
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
### 🔹 8.2. **DPKG (Debian Package Manager)**
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

### 🔹 8.3. **Snap**
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

### 🔹 8.4. **Ubuntu Software Center (GUI)**
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

## 🛠️ 9. Common Commands

```bash
sudo apt update           # Update package index
sudo apt install nginx    # Install a package
sudo systemctl status     # Check service status
```
## 🔍 9.1 **Check if a Package Is Installed**

```bash
dpkg -l | grep <package-name>
```
Example:
```bash
dpkg -l | grep nginx
```

---

## 🧠 9. **Service commands in Ubuntu**

**`service` commands** are used to manage system services (start, stop, restart, etc.). These commands are wrappers around `systemctl` (for systemd) or older init systems.

List of **commonly used `service` commands** in Ubuntu:

---

### ✅ Basic Syntax

```bash
sudo service <service_name> <command>
```
**Example:**
```bash
sudo service apache2 start
sudo service ssh status
sudo service nginx restart
sudo service mysql stop
```
---

### 🔧 9.1 Common Service Commands

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

### 🔍 9.2 List All Services

```bash
# Using service (limited list)
service --status-all

# Using systemctl (preferred)
systemctl list-units --type=service
```
---

## 🏁 10. **Conclusion**

Ubuntu stands out as one of the most reliable, user-friendly, and versatile Linux distributions available today. Whether you're a beginner exploring Linux for the first time, a developer building modern applications, or a system administrator managing large-scale infrastructure, **Ubuntu provides a powerful and secure environment** to get the job done.

From its rich ecosystem of open-source tools and frequent LTS releases to its seamless integration with cloud, container, and DevOps technologies, Ubuntu offers everything you need to build, deploy, and manage software effectively.

With robust software management options (`APT`, `Snap`, `DPKG`), intuitive service control (`service`, `systemctl`), and strong community support, Ubuntu continues to empower millions of users and organizations around the globe.

---

## 11. Contacts

| Name         | Email Address                                 |
|--------------|-----------------------------------------------|
| Adil Nawaz | adil.nawaz.snaatak@mygurukulam.co           |

---

## 12. References

| **Title**                        | **Link**                                                                                      |
|----------------------------------|-----------------------------------------------------------------------------------------------|
| Ubuntu Official Documentation  | (https://help.ubuntu.com)          |
| Ubuntu Releases List           | (https://wiki.ubuntu.com/Releases) |

