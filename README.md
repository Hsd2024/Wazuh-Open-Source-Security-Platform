# Wazuh-Open-Source-Security-Platform
It is a free, open-source security platform for threat detection, incident response, and compliance monitoring. It is an advanced Host-based Intrusion Detection System (HIDS) that helps monitor and protect endpoints, servers, and cloud environments.

![Wazuh Diagram](https://github.com/user-attachments/assets/3cb4b6e0-5ef6-4646-b4c4-8e2272259c3a)

# To Install Wazuh on a Virtual Machine (VM) follow the steps

**First install VMware Workstation Player (Free for personal use)** – Download Here (https://www.vmware.com/)

**See how to install VM (https://github.com/Hsd2024/Vertual-Machine-installation)**

**Install OS: Ubuntu 22.04 LTS in your VM workstation**

**After Ubuntu installation, log in and update the system from Terminal**

this is the script    _""sudo apt update && sudo apt upgrade -y && sudo apt autoremove -y && sudo apt clean""_

<img width="685" alt="Screenshot 2025-03-29 051922" src="https://github.com/user-attachments/assets/9aa63188-cdec-49bf-adc6-2b234d579ab9" />

# Install Wazuh on Ubuntu#

**This is the script**    _""curl -sO https://packages.wazuh.com/4.11/wazuh-install.sh && sudo bash ./wazuh-install.sh -a""_

**Run the Wazuh installation script in termenal**

<img width="632" alt="wa-1" src="https://github.com/user-attachments/assets/65a1b412-e618-4f2d-bbd2-ab5fe27ab995" />

- Installing Wazuh

<img width="815" alt="wa-2" src="https://github.com/user-attachments/assets/bf062d9a-80a0-4bae-bcc4-2c355ae03413" />

Wazuh is installed successfully! 🎉

(Find your VM's IP using ip a or hostname -I.)

- Access the Wazuh web interface with https://<WAZUH_DASHBOARD_IP_ADDRESS> inter the IP address,

# Log in using the default credentials.

Username: admin
Password: XXXXXXXX

