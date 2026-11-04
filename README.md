# 🚀 Burp Suite Professional Installation Guide

<div align="center">

![Burp Suite Pro](https://img.shields.io/badge/Burp%20Suite-Pro-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white)
![Java](https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Debian%2FUbuntu-A81D33?style=for-the-badge&logo=linux&logoColor=white)
![Bash](https://img.shields.io/badge/Shell-Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

![Platform](https://img.shields.io/badge/Platform-Linux-informational?style=flat-square)
![License](https://img.shields.io/badge/License-Educational-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![Made with](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red?style=flat-square)

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=800&color=FF6633&center=true&vCenter=true&width=600&lines=Welcome+to+the+Burp+Suite+Pro+Setup+Guide;Step-by-step+installation+for+Linux;Fast+%7C+Clean+%7C+Reliable" alt="Typing SVG" />

</div>

---

## 📑 Table of Contents

- [📋 Prerequisites](#-prerequisites)
- [⚙️ Step-by-Step Installation](#️-step-by-step-installation)
  - [Step 1 — Download Burp Suite Pro](#step-1--download-burp-suite-pro)
  - [Step 2 — Install Java 21](#step-2--install-java-21)
  - [Step 3 — Set Java 21 as Default](#step-3--set-java-21-as-default)
  - [Step 4 — Download the Loader](#step-4--download-the-loader)
  - [Step 5 — Run the Loader](#step-5--run-the-loader)
- [🧠 Notes & Troubleshooting](#-notes--troubleshooting)
- [✅ Verify Installation](#-verify-installation)
- [📚 Resources](#-resources)

---

## 📋 Prerequisites

<div align="center">

| ✅ Requirement | 💡 Description |
|:---|:---|
| 🐧 **OS** | Debian / Ubuntu-based Linux distribution |
| 🔐 **Privileges** | `sudo` access required |
| 📦 **Tools** | `wget` and `java` installed |
| 🌐 **Network** | Stable internet connection |

</div>

> 💡 **Tip:** Verify prerequisites quickly:
> ```bash
> which wget && java -version && sudo -v
> ```

---

## ⚙️ Step-by-Step Installation

### Step 1 — Download Burp Suite Pro

Download the official Burp Suite Pro JAR directly from PortSwigger's servers.

```bash
wget -O burpsuite_pro.jar --quiet --show-progress \
  "https://portswigger.net/burp/releases/download?product=pro&version=2026.3.3&type=Jar"
```

<div align="center">
  <img src="https://progress-bar.xyz/20?title=Progress&width=400&color=FF6633" alt="Progress 20%"/>
</div>

---

### Step 2 — Install Java 21

Update your package index and install **OpenJDK 21**.

```bash
sudo apt update
sudo apt install openjdk-21-jdk -y
```

> ⚡ This step may take a few minutes depending on your connection speed.

<div align="center">
  <img src="https://progress-bar.xyz/40?title=Progress&width=400&color=FF6633" alt="Progress 40%"/>
</div>

---

### Step 3 — Set Java 21 as Default

Switch the system's default Java to version 21:

```bash
sudo update-alternatives --config java
```

> 📌 **Interactive step:** A numbered list appears. Type the number corresponding to **Java 21** and hit `Enter`.

Verify the change:

```bash
java -version
```

Expected output:
```
openjdk version "21.x.x" 2024-xx-xx
OpenJDK Runtime Environment ...
```

<div align="center">
  <img src="https://progress-bar.xyz/60?title=Progress&width=400&color=FF6633" alt="Progress 60%"/>
</div>

---

### Step 4 — Download the Loader

Download `burp-loader.jar` from the repository:

```bash
wget https://github.com/ZONNYXXD/BURPXPRO/blob/main/burp-loader.jar
```

> ⚠️ **Important:** Ensure both `burpsuite_pro.jar` and `burp-loader.jar` are in the **same directory**.

<div align="center">
  <img src="https://progress-bar.xyz/80?title=Progress&width=400&color=FF6633" alt="Progress 80%"/>
</div>

---

### Step 5 — Run the Loader

Launch the loader using Java:

```bash
java -jar burp-loader.jar
```

Once the loader GUI appears:

1. 🖱️ Click **Run**
2. 🚀 Burp Suite Pro will launch automatically
3. 🎉 Complete any remaining in-app prompts

<div align="center">
  <img src="https://progress-bar.xyz/100?title=Done&width=400&color=00C853" alt="Progress 100%"/>
</div>

<div align="center">

```
✅ Installation Complete — Happy Testing! 🕵️‍♂️
```

</div>

---

## 🧠 Notes & Troubleshooting

<details>
<summary><b>📁 1. Loader cannot find Burp JAR</b></summary>

Ensure both files live in the same directory:

```bash
ls -la | grep burp
# -rw-r--r--  burpsuite_pro.jar
# -rw-r--r--  burp-loader.jar
```
</details>

<details>
<summary><b>☕ 2. Java version conflicts</b></summary>

Re-run the Java alternatives selector and confirm Java 21 is active:

```bash
sudo update-alternatives --config java
java -version
```
</details>

<details>
<summary><b>🔄 3. Keeping Burp Suite updated</b></summary>

Always check the official [PortSwigger Releases page](https://portswigger.net/burp/releases) for the latest version and re-download the JAR when a new release drops.
</details>

<details>
<summary><b>🛑 4. Permission denied when running the JAR</b></summary>

Make the files executable:

```bash
chmod +x burpsuite_pro.jar burp-loader.jar
```
</details>

<details>
<summary><b>🧱 5. GUI not displaying (headless server)</b></summary>

Burp Suite requires a graphical environment. Use VNC, X11 forwarding, or a desktop session:

```bash
ssh -X user@server
```
</details>

---

## ✅ Verify Installation

Run these checks to confirm everything works:

```bash
# Java check
java -version

# File check
ls -lh burpsuite_pro.jar burp-loader.jar

# Launch
java -jar burp-loader.jar
```

<div align="center">

| Check | Expected |
|:---|:---:|
| Java 21 installed | ✅ |
| Both JARs present | ✅ |
| Loader GUI opens | ✅ |
| Burp Suite launches | ✅ |

</div>

---

## 📚 Resources

<div align="center">

| 🔗 Resource | 📝 Description |
|:---|:---|
| [PortSwigger Burp Releases](https://portswigger.net/burp/releases) | Official Burp Suite downloads |
| [OpenJDK Downloads](https://openjdk.org/) | Java runtime & JDK |
| [Burp Suite Docs](https://portswigger.net/burp/documentation) | Official documentation |
| [BURPXPRO Repo](https://github.com/ZONNYXXD/BURPXPRO) | Loader source |

</div>

---

<div align="center">

### ⭐ If this guide helped you, consider giving it a star!

![Footer](https://capsule-render.vercel.app/api?type=waving&color=FF6633&height=100&section=footer)

**Made with ❤️ for the security community**

![Visitors](https://api.visitorbadge.io/api/visitors?path=burpxpro-guide&label=Visitors&countColor=%23FF6633)

</div>
