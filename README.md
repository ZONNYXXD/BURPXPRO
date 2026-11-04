# Burp Suite Pro Installation Guide

A step-by-step guide to installing and setting up Burp Suite Professional.

---

## Prerequisites

- A Debian/Ubuntu-based Linux system
- `sudo` privileges
- `wget` and `java` installed

---

## Step 1: Download Burp Suite Pro

Download the official Burp Suite Pro JAR from the PortSwigger server:


wget -O burpsuite_pro.jar --quiet --show-progress "https://portswigger.net/burp/releases/download?product=pro&version=2026.3.3&type=Jar"
## Step 2: Install Java 21
Update your package list and install OpenJDK 21:

bash
sudo apt update
sudo apt install openjdk-21-jdk -y
## Step 3: Set Java 21 as Default
Configure the default Java version to 21:

bash
sudo update-alternatives --config java
Select the entry corresponding to Java 21 from the list.

## Step 4: Download the Loader
Download burp-loader.jar from the repository:

🔗 https://github.com/ZONNYXXD/BURPXPRO/blob/main/burp-loader.jar

## Step 5: Run the Loader
Launch the loader with Java:

bash
java -jar burp-loader.jar
Once the loader window opens, click Run to start Burp Suite Pro.

Notes
Ensure burpsuite_pro.jar and burp-loader.jar are located in the same directory if the loader requires it.

If you encounter Java version conflicts, re-run sudo update-alternatives --config java and verify the selection.

Keep your installation updated by checking the official PortSwigger releases page.
```bash
