# Elevate-Labs-Task-4
🔐 Linux Firewall Configuration using UFW
This project was created as part of a Cyber Security Internship to demonstrate the setup and use of a firewall on a Linux system using UFW (Uncomplicated Firewall).

📌 Objective
To configure and test basic firewall rules to allow or block network traffic using UFW on a Linux-based system.

🧰 Tools Used
Linux Terminal

UFW (Uncomplicated Firewall)

Telnet (for testing blocked ports)

⚙️ Steps Performed
Install UFW

sudo apt install ufw
Check UFW Status

ufw status verbose
Enable UFW

sudo ufw enable
List Existing Rules

sudo ufw status numbered
Block a Specific Port (e.g., Telnet - Port 23)

sudo ufw deny 23
Test the Rule with Telnet


sudo apt install telnet
telnet localhost 23
Expected Result: Connection refused or timed out.

Allow SSH Access (Port 22)

sudo ufw allow 22
Remove the Test Rule
List rules:

sudo ufw status numbered
Delete rule (e.g., rule #3):

sudo ufw delete 3
🧠 Key Concepts
Firewalls filter incoming and outgoing traffic using rule-based logic.

UFW provides a user-friendly interface for configuring iptables.

Rules can specify:

IP addresses

Port numbers

Protocols

Default policy can be set to allow all or deny all.

Stateful inspection ensures return traffic for valid outbound requests is allowed.
