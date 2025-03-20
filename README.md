# Wazuh-Open-Source-Security-Platform
It is a free, open-source security platform used for threat detection, incident response, and compliance monitoring. It is an advanced Host-based Intrusion Detection System (HIDS) that helps monitor and protect endpoints, servers, and cloud environments.

![Wazuh Diagram](https://github.com/user-attachments/assets/2dc63569-25c3-431f-a01f-6272537048ed)

# To Install Wazuh on a Virtual Machine (VM) follow the steps

**First install VMware Workstation Player (Free for personal use)** – Download Here (https://www.vmware.com/)

**Install OS: Ubuntu 22.04 LTS in your VM workstation**

**After Ubuntu installation, log in and update the system from Terminal**

# Install Wazuh on Ubuntu#

**Run the Wazuh installation script**

curl -sO https://packages.wazuh.com/4.11/wazuh-install.sh && sudo bash ./wazuh-install.sh -a

- Install Wazuh repository

curl -sO https://packages.wazuh.com/key/GPG-KEY-WAZUH

sudo apt-key add GPG-KEY-WAZUH
echo "deb https://packages.wazuh.com/4.x/apt/ stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list
sudo apt update

- Install Wazuh Manager

sudo apt install -y wazuh-manager

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

