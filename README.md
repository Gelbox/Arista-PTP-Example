# Arista-PTP-Example
PTP Automation Playbook for Arista Switches

Automate Precision Time Protocol (PTP) Configuration on Arista EOS

This Ansible playbook automates the setup of PTP boundary clocks on Arista switches, ensuring precise synchronization across media and ProAV networks.
🔹 Features

✔ Configures PTP domain, boundary clock mode, and priority settings
✔ Assigns leader election roles dynamically based on BMCA
✔ Enables OSPF routing for PTP-enabled interfaces
✔ Applies access control lists (ACLs) for PTP security
✔ Supports multi-switch deployment (Spine-Leaf architecture)
📌 Prerequisites

Ensure you have the following before running the playbook:

1️⃣ Ansible Installed (v2.10+)

2️⃣ Arista EOS Devices with API access enabled

3️⃣ SSH Connectivity to switches

4️⃣ Python & Required Modules: paramiko, netmiko

⚙️ How to Use

1️⃣ Clone the Repository


2️⃣ Define Your Inventory

Edit inventory.yml with your switch details:

all:
  hosts:
    spine-1:
      ansible_host: x.x.x.x


3️⃣ Run the Playbook

ansible-playbook -i <Arista PTP Example inventory.yml Arista PTP Example Playbook.yml

