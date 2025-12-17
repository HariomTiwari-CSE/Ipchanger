# 🔄 IP-Changer

A Bash script tool to change the IP address of a Linux network interface. Useful for cybersecurity labs, network testing, and educational demonstrations on **your own authorized systems**.

> **⚠️ Legal & Ethical Disclaimer:** This tool is created **solely for educational purposes and authorized testing**. Misuse of this tool to interfere with networks you do not own or have explicit permission to test is **illegal and unethical**. The author assumes no liability.

## ✨ Features
- **Dual Mode Operation:** Choose between manual IP entry or automatic assignment.
- **Input Validation:** Basic checks for correct IP address format.
- **Permission Awareness:** Script verifies and requires `sudo` privileges to run.
- **Clear Feedback:** Confirms success or failure of the IP change operation.

## 🚀 Quick Start

### Prerequisites
- A Linux distribution (Tested on Kali Linux, Ubuntu)
- `sudo` or root access
- `figlet` (for the banner): `sudo apt-get install figlet`

### Installation & Execution
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/HariomTiwari-CSE/IP-Changer.git
    cd IP-Changer
    ```
2.  **Install the dependency and run the tool:**
    ```bash
    sudo apt-get install figlet
    bash Ipchanger.sh
    ```

## 🖥️ Screenshot
<p align="center">
  <img src="Ipchanger.png" alt="IP-Changer Tool Screenshot" width="700">
</p>

## 🔧 How It Works: Technical Breakdown
The script's workflow demonstrates core systems concepts:
1.  **Privilege Check:** Verifies the user has root (`sudo`) permissions.
2.  **User Interaction:** Presents a menu for manual (`M`) or automatic (`A`) IP assignment.
3.  **Network Command Execution:**
    - In **Manual Mode**, it configures the user-specified interface with the provided IP using `ifconfig`.
    - In **Automatic Mode**, it assigns a pre-defined IP to the `eth0` interface.
4.  **Verification:** Checks if the IP was successfully assigned and reports the result.

This provides practical experience with **Bash scripting, Linux networking commands, and privilege management**.

## 🛠️ Technology Stack
- **Bash Scripting** (Core logic and user interaction)
- **Linux System Commands** (`ifconfig`, `awk`, `grep`)
- **Network Fundamentals** (IP addressing, interfaces)

## 💡 Project Roadmap & Ideas for Enhancement
Potential features to extend this educational project:
- [ ] Add support for setting the **subnet mask and default gateway**.
- [ ] Improve IP validation using a dedicated tool like `ipcalc`.
- [ ] Create an **installation script** (`install.sh`) to automate dependency setup.
- [ ] Extend **Automatic Mode** to generate a random IP within a valid range.
- [ ] Port the tool to **Python** for cross-platform compatibility and a potential GUI.

## 🧠 Author's Note
This project was developed by **Hariom Tiwari** as a hands-on learning exercise. It bridges the gap between theoretical cybersecurity concepts (learned during CEH certification) and practical system-level scripting. Building this tool solidified my understanding of network configuration and Linux automation—skills crucial for a career in security.

---
**Connect:**  
[![LinkedIn](https://img.shields.io/badge/-Hariom_Tiwari-blue?style=flat&logo=Linkedin&logoColor=white)](https://linkedin.com/in/your-profile)  
**📫 Hariom Tiwari** | B.Tech CSE Graduate | EC-Council CEH Certified
