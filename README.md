# Wazuh-SIEM-OSSEC-Installation-on-Ubuntu
Setup and configuration of Wazuh SIEM and OSSEC on an Ubuntu system for real-time security monitoring, log analysis, and intrusion detection.

⚠️ Disclaimer
This project is for educational purposes only. The setup and use of Wazuh SIEM and OSSEC should be conducted in a controlled environment. Unauthorized security monitoring, intrusion detection, or penetration testing on systems without explicit permission is illegal and may result in severe consequences.

Overview
My project documents the process of setting up Wazuh SIEM and OSSEC on an Ubuntu system. Wazuh is an open-source security information and event management (SIEM) solution, while OSSEC is a host-based intrusion detection system (HIDS) that helps monitor and protect systems against security threats.

Project Installation
1. Downloading and Installing Ubuntu ISO
To set up the environment, I installed Ubuntu as the primary operating system on my laptop:
- Download the latest Ubuntu ISO file from the official website.
- Created a bootable USB using Rufus (Windows)
- Restarted the laptop and booted from the USB drive into the bios .
- Installed Ubuntu by following the guided setup, selecting appropriate partitions, and completing the installation process.

2. Installing Wazuh SIEM
Once Ubuntu was set up, I installed Wazuh SIEM, which provides security visibility and monitoring capabilities:
- Updated system packages using:
- sudo apt update && sudo apt upgrade -y
- Installed Wazuh by following the official Wazuh installation guide, which includes setting up the Wazuh manager, API, and dashboard.
- Configured Wazuh to monitor system logs, network traffic, and security events.

3. Installing OSSEC
Host-based security monitoring, I installed OSSEC, which integrates well with Wazuh:
- Downloaded and installed OSSEC using:
- sudo apt install ossec-hids
- Configured OSSEC to work alongside Wazuh for advanced log analysis and real-time alerting.
- Verified that OSSEC was running properly and forwarding logs to Wazuh.

OSSEC Terminal Step-by-Step Guide
Running cd /var/ossec directly won’t work because it is owned by root, resulting in permission being denied.
- sudo bash (to access root user)
- ls (list directory contents)
- cd /var/ossec/etc/subl ossec.conf (To navigate into the etc directory and modify ossec.conf)
- cd /var/ossec/etc/subl ossec.conf

Vulnerability Detector:
Explanation: The Vulnerability Detector was a key focus of my project because it helps identify security weaknesses in the system by scanning for known vulnerabilities in installed software.

Conclusion
This project successfully set up a security monitoring system using Wazuh SIEM and OSSEC on Ubuntu. The system now provides real-time security insights, log analysis, and intrusion detection to enhance system protection.
