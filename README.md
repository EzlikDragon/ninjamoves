# NinjaMoves 1.0 - Network Anonymity and MAC Spoofing Tool

**NinjaMoves 1.0** is a powerful network anonymity and security tool designed to help users spoof their MAC address and change their system's hostname. This tool is mainly for Linux-based systems and is crafted for privacy-conscious individuals who want to stay anonymous and protect their data in controlled environments.

Created by **EzlikDragon | SlickLab**, NinjaMoves makes it easy to modify your network identity, ensuring you're not being tracked by your MAC address and hostname.

> **Warning**: This tool should only be used in a legal and ethical manner, within your own systems or with explicit permission from the system owner.

## Features

- **MAC Address Spoofing**: Automatically detects the primary network interface and assigns a random MAC address using the `macchanger` tool.
- **Hostname Change**: Randomizes the system hostname for enhanced anonymity.
- **Cross-Platform**: Works on most Linux-based systems (e.g., Ubuntu, Kali Linux).
- **Simple Command-Line Interface**: Easy-to-use with minimal setup.

## Installation

### Prerequisites

Ensure your system has the following tools installed:

- `macchanger`
- `iproute2`
- `sudo`

On most Debian-based systems (e.g., Ubuntu, Kali), you can install them using:

```bash
sudo apt update
sudo apt install macchanger iproute2 sudo

Steps to Install
Clone the repository:

bash
Copy
Edit
git clone https://github.com/EzlikDragon/ninjamoves.git
Navigate to the project directory:

bash
Copy
Edit
cd ninjamoves
Make the script executable:

bash
Copy
Edit
chmod +x ninjamoves
Optionally, move the script to a global directory like /usr/local/bin:

bash
Copy
Edit
sudo mv ninjamoves /usr/local/bin
Copy the .ico file to the appropriate directory:

bash
Copy
Edit
sudo cp NinjaMoves.ico /usr/share/icons/hicolor/128x128/apps/ninjamoves.ico
Create a .desktop file to enable easier access from the application menu:

bash
Copy
Edit
sudo cp ninjamoves.desktop /usr/share/applications/
Refresh the desktop application database:

bash
Copy
Edit
sudo update-desktop-database
Usage
To run NinjaMoves, simply execute the following command:

bash
Copy
Edit
ninjamoves
The tool will:

Detect the primary network interface.

Spoof the MAC address.

Change the system hostname to a randomly generated one.

Example output:

bash
Copy
Edit
[*] Spoofing MAC address on eth0 ...
[*] Changing hostname to: host-abc123