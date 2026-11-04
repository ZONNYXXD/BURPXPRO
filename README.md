
🚀 Burp Suite Professional Installation Guide
<div align="center">
https://img.shields.io/badge/Burp%20Suite-Pro-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white&labelColor=1a1a2e
https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white&labelColor=1a1a2e
https://img.shields.io/badge/Linux-Debian%2FUbuntu-A81D33?style=for-the-badge&logo=linux&logoColor=white&labelColor=1a1a2e
https://img.shields.io/badge/Shell-Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white&labelColor=1a1a2e


https://img.shields.io/badge/Platform-Linux-informational?style=for-the-badge&logo=linux&logoColor=white&color=0f3460
https://img.shields.io/badge/License-Educational-blue?style=for-the-badge&color=533483
https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge&color=00b894
https://img.shields.io/badge/Made%20with-%E2%9D%A4-red?style=for-the-badge&color=e94560


<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=28&duration=3000&pause=800&color=FF6633&center=true&vCenter=true&width=700&height=60&lines=Welcome+to+the+Burp+Suite+Pro+Setup+Guide;Step-by-step+installation+for+Linux;Fast+%7C+Clean+%7C+Reliable;Let's+Hack+the+Planet+%F0%9F%9A%80" alt="Typing SVG" />
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24,30&height=120&section=header&text=Burp%20Suite%20Pro&fontSize=40&fontColor=ffffff&animation=twinkling&fontAlignY=35" width="100%" alt="Header Wave"/></div>
<div align="center">
text
╔══════════════════════════════════════════════════════════════╗
║  🎯  A complete, animated walkthrough to get Burp Suite     ║
║      Professional running on your Linux machine.            ║
╚══════════════════════════════════════════════════════════════╝
</div>
📑 Table of Contents
<div align="center">
📌 Section	🔗 Jump
📋 Prerequisites	Go →
⚙️ Step-by-Step Installation	Go →
🧠 Notes & Troubleshooting	Go →
✅ Verify Installation	Go →
📚 Resources	Go →
</div><details> <summary><b>🔍 Expand Full TOC</b></summary>
📋 Prerequisites

⚙️ Step-by-Step Installation

Step 1 — Download Burp Suite Pro

Step 2 — Install Java 21

Step 3 — Set Java 21 as Default

Step 4 — Download the Loader

Step 5 — Run the Loader

🧠 Notes & Troubleshooting

✅ Verify Installation

📚 Resources

</details>
📋 Prerequisites
<div align="center"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=2500&pause=1000&color=00D9FF&center=true&vCenter=true&width=500&lines=Before+we+begin...;Make+sure+you+have+everything+ready!" alt="Prereq Typing" /></div><div align="center">
✅ Requirement	💡 Description
🐧 OS	Debian / Ubuntu-based Linux distribution
🔐 Privileges	sudo access required
📦 Tools	wget and java installed
🌐 Network	Stable internet connection
</div>
💡 Tip: Verify prerequisites quickly:

bash
which wget && java -version && sudo -v
<div align="center">
https://img.shields.io/badge/Pre--Flight_Check-Ready-success?style=flat-square&logo=checkmarx&logoColor=white

</div>
⚙️ Step-by-Step Installation
<div align="center"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&duration=3000&pause=1000&color=FF6633&center=true&vCenter=true&width=600&lines=Follow+the+5+steps+below;Each+step+is+color+coded+%F0%9F%8E%A8;Take+your+time+and+enjoy+the+ride!" alt="Steps Typing" /></div>
🟠 Step 1 — Download Burp Suite Pro
<div align="center">
https://img.shields.io/badge/STEP-1-FF6633?style=for-the-badge&logo=download&logoColor=white

</div>
Download the official Burp Suite Pro JAR directly from PortSwigger's servers.

bash
wget -O burpsuite_pro.jar --quiet --show-progress \
  "https://portswigger.net/burp/releases/download?product=pro&version=2026.3.3&type=Jar"
<div align="center"> <img src="https://progress-bar.xyz/20?title=Downloading&width=500&color=FF6633&suffix=%20" alt="Progress 20%"/> </div><div align="center">
https://img.shields.io/badge/Status-Downloading-orange?style=flat-square&logo=wget&logoColor=white
https://img.shields.io/badge/Size-~70MB-blue?style=flat-square

</div>
🟡 Step 2 — Install Java 21
<div align="center">
https://img.shields.io/badge/STEP-2-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white

</div>
Update your package index and install OpenJDK 21.

bash
sudo apt update
sudo apt install openjdk-21-jdk -y
⚡ This step may take a few minutes depending on your connection speed.

<div align="center"> <img src="https://progress-bar.xyz/40?title=Installing%20Java&width=500&color=ED8B00&suffix=%20" alt="Progress 40%"/> </div><div align="center">
https://img.shields.io/badge/OpenJDK-21-ED8B00?style=flat-square&logo=openjdk&logoColor=white
https://img.shields.io/badge/Status-Installing-yellow?style=flat-square

</div>
🟢 Step 3 — Set Java 21 as Default
<div align="center">
https://img.shields.io/badge/STEP-3-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white

</div>
Switch the system's default Java to version 21:

bash
sudo update-alternatives --config java
📌 Interactive step: A numbered list appears. Type the number corresponding to Java 21 and hit Enter.

Verify the change:

bash
java -version
Expected output:

text
openjdk version "21.x.x" 2024-xx-xx
OpenJDK Runtime Environment ...
<div align="center"> <img src="https://progress-bar.xyz/60?title=Configuring&width=500&color=4EAA25&suffix=%20" alt="Progress 60%"/> </div><div align="center">
https://img.shields.io/badge/Java-21_Active-brightgreen?style=flat-square&logo=openjdk&logoColor=white
https://img.shields.io/badge/Status-Configured-success?style=flat-square

</div>
🔵 Step 4 — Download the Loader
<div align="center">
https://img.shields.io/badge/STEP-4-1E90FF?style=for-the-badge&logo=github&logoColor=white

</div>
Download burp-loader.jar from the repository:

bash
wget https://github.com/ZONNYXXD/BURPXPRO/blob/main/burp-loader.jar
⚠️ Important: Ensure both burpsuite_pro.jar and burp-loader.jar are in the same directory.

<div align="center"> <img src="https://progress-bar.xyz/80?title=Loader%20Ready&width=500&color=1E90FF&suffix=%20" alt="Progress 80%"/> </div><div align="center">
https://img.shields.io/badge/Loader-Downloaded-blue?style=flat-square&logo=github&logoColor=white
https://img.shields.io/badge/Status-Ready-informational?style=flat-square

</div>
🟣 Step 5 — Run the Loader
<div align="center">
https://img.shields.io/badge/STEP-5-9B59B6?style=for-the-badge&logo=jetbrains&logoColor=white

</div>
Launch the loader using Java:

bash
java -jar burp-loader.jar
Once the loader GUI appears:

🖱️ Click Run

🚀 Burp Suite Pro will launch automatically

🎉 Complete any remaining in-app prompts

<div align="center"> <img src="https://progress-bar.xyz/100?title=Complete&width=500&color=00C853&suffix=%20" alt="Progress 100%"/> </div><div align="center">
text
╔════════════════════════════════════════════╗
║   ✅  Installation Complete               ║
║   🕵️  Happy Testing, Hacker!              ║
╚════════════════════════════════════════════╝
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=22&duration=2500&pause=800&color=00C853&center=true&vCenter=true&width=500&lines=Burp+Suite+Pro+is+Ready!+%F0%9F%8E%89;Time+to+Hack+the+Planet+%F0%9F%9A%80" alt="Done Typing" /></div>
🧠 Notes & Troubleshooting
<div align="center"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=2500&pause=1000&color=FF6B6B&center=true&vCenter=true&width=550&lines=Ran+into+an+issue%3F;Don't+panic+-+we've+got+you+covered!" alt="Troubleshoot Typing" /></div><details> <summary><b>📁 1. Loader cannot find Burp JAR</b></summary>
Ensure both files live in the same directory:

bash
ls -la | grep burp
# -rw-r--r--  burpsuite_pro.jar
# -rw-r--r--  burp-loader.jar
</details><details> <summary><b>☕ 2. Java version conflicts</b></summary>
Re-run the Java alternatives selector and confirm Java 21 is active:

bash
sudo update-alternatives --config java
java -version
</details><details> <summary><b>🔄 3. Keeping Burp Suite updated</b></summary>
Always check the official PortSwigger Releases page for the latest version and re-download the JAR when a new release drops.

</details><details> <summary><b>🛑 4. Permission denied when running the JAR</b></summary>
Make the files executable:

bash
chmod +x burpsuite_pro.jar burp-loader.jar
</details><details> <summary><b>🧱 5. GUI not displaying (headless server)</b></summary>
Burp Suite requires a graphical environment. Use VNC, X11 forwarding, or a desktop session:

bash
ssh -X user@server
</details>
✅ Verify Installation
<div align="center"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=2500&pause=1000&color=00D9FF&center=true&vCenter=true&width=550&lines=Let's+double-check+everything;Run+the+checks+below+to+confirm+success!" alt="Verify Typing" /></div>
Run these checks to confirm everything works:

bash
# Java check
java -version

# File check
ls -lh burpsuite_pro.jar burp-loader.jar

# Launch
java -jar burp-loader.jar
<div align="center">
🔎 Check	🎯 Expected	📊 Status
Java 21 installed	✅	https://img.shields.io/badge/Pass-success?style=flat-square
Both JARs present	✅	https://img.shields.io/badge/Pass-success?style=flat-square
Loader GUI opens	✅	https://img.shields.io/badge/Pass-success?style=flat-square
Burp Suite launches	✅	https://img.shields.io/badge/Pass-success?style=flat-square
</div>
📚 Resources
<div align="center">
🔗 Resource	📝 Description
PortSwigger Burp Releases	Official Burp Suite downloads
OpenJDK Downloads	Java runtime & JDK
Burp Suite Docs	Official documentation
BURPXPRO Repo	Loader source
</div><div align="center">
https://img.shields.io/badge/PortSwigger-Official-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white
https://img.shields.io/badge/OpenJDK-Downloads-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white
https://img.shields.io/badge/BURPXPRO-Repo-181717?style=for-the-badge&logo=github&logoColor=white

</div>
<div align="center"><img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24,30&height=140&section=footer&text=Thanks%20for%20Reading!&fontSize=32&fontColor=ffffff&animation=twinkling&fontAlignY=50" width="100%" alt="Footer Wave"/>
⭐ If this guide helped you, consider giving it a star!
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=FF6633&center=true&vCenter=true&width=500&lines=Made+with+%E2%9D%A4%EF%B8%8F+for+the+security+community;Stay+curious.+Stay+ethical.+Keep+hacking!" alt="Footer Typing" />
https://api.visitorbadge.io/api/visitors?path=burpxpro-guide&label=Visitors&countColor=%23FF6633&style=for-the-badge


https://img.shields.io/badge/Made%20with-%E2%9D%A4-red?style=for-the-badge
https://img.shields.io/badge/For-The%20Security%20Community-FF6633?style=for-the-badge&logo=shield&logoColor=white
https://img.shields.io/badge/Use-Responsibly-00C853?style=for-the-badge&logo=checkmarx&logoColor=white


text
╔══════════════════════════════════════════════════════════════╗
║          🎉  You're all set — go break some things!         ║
║                    (ethically, of course)                    ║
╚══════════════════════════════════════════════════════════════╝
</div>
<div align="center">
<sub>🔐 Disclaimer: This guide is intended for educational and authorized security testing purposes only. Always obtain proper permission before testing any system you do not own.</sub>

</div>
