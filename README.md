# Wazuh-Open-Source-Security-Platform
It is a free, open-source security platform for threat detection, incident response, and compliance monitoring. It is an advanced Host-based Intrusion Detection System (HIDS) that helps monitor and protect endpoints, servers, and cloud environments.

![Wazuh Diagram](https://github.com/user-attachments/assets/3cb4b6e0-5ef6-4646-b4c4-8e2272259c3a)

# To Install Wazuh on a Virtual Machine (VM) follow the steps

**First install VMware Workstation Player (Free for personal use)** – Download Here (https://www.vmware.com/)

**See how to install VM (https://github.com/Hsd2024/Vertual-Machine-installation)**

**Install OS: Ubuntu 22.04 LTS in your VM workstation**

**After Ubuntu installation, log in and update the system from Terminal**

this is the script    _""sudo apt update && sudo apt upgrade -y && sudo apt autoremove -y && sudo apt clean""_

<img width="632" alt="wa-1" src="https://github.com/user-attachments/assets/5eccd840-e94b-4717-a195-0af6e03e8333" />

# Install Wazuh on Ubuntu#

**This is the script**    _""curl -sO https://packages.wazuh.com/4.11/wazuh-install.sh && sudo bash ./wazuh-install.sh -a""_

**Run the Wazuh installation script in termenal**

![1](https://github.com/user-attachments/assets/43832070-2dca-4ac7-9ce2-7ebd51e7ce47)

- Install Wazuh Manager

sudo apt install -y wazuh-manager

![3](https://github.com/user-attachments/assets/2b99f6d3-f427-41ba-a993-e425bb476424)

- Start and enable Wazuh Manager

sudo systemctl enable wazuh-manager --now

- Verify Wazuh is Running

sudo systemctl status wazuh-manager
If it says “active (running)”, Wazuh is installed successfully! 🎉

(Find your VM's IP using ip a or hostname -I.)

- Access the Wazuh web interface with https://<WAZUH_DASHBOARD_IP_ADDRESS> inter the IP address,

# Log in using the default credentials.

Username: admin
Password: wazuh

