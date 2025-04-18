# Secure VPN Server with Raspberry Pi

---

## Objective

This project involved building a secure, self-hosted VPN using WireGuard on a Raspberry Pi. The goal was to enable encrypted remote access for private computing and gaming while learning core networking and Linux administration concepts. It focused on configuring firewall rules, managing keys, and setting up DNS and NAT to replicate real-world privacy and network segmentation techniques.

---

## How to Complete

Download the zip file attached which holds all neccearey items to complete the project - Follow the given steps below, if you expeirirnece roadblocks, self-troubleshooting is your path to victory! Good luck and have fun!

---

## Skills Learned

- Understanding VPN protocols and secure tunneling with WireGuard  
- Linux system configuration and use of command-line tools  
- Firewall setup using `iptables` and basic network security rules  
- DNS resolution and prevention of DNS leaks through custom resolvers  
- Port forwarding and NAT setup for remote device access  
- Key management and secure client provisioning  
- Troubleshooting system connectivity and remote access

---

## Tools Used

- Raspberry Pi OS Lite (headless setup)  
- WireGuard VPN  
- Linux CLI utilities (systemctl, ip, ufw, nano)  
- `iptables` for firewall and NAT configuration  
- Unbound DNS resolver (optional, for added privacy)  
- PiVPN for streamlined installation and client management  
- QR code generation tools for mobile device setup  

---

## Steps

### 1. System Preparation

- Flashed Raspberry Pi OS Lite onto a microSD card and booted the device headlessly with SSH enabled  
- Performed system updates and enabled IP forwarding in `sysctl.conf`  
- Installed essential networking packages and configured static IP

### 2. WireGuard Installation and Configuration

- Installed WireGuard using PiVPN  
- Generated private/public key pairs for server and clients  
- Created `wg0.conf` with static IP address, listening port, and post-up/down firewall rules

### 3. NAT and Firewall Setup

- Enabled `iptables` rules for forwarding and NAT masquerading  
- Ensured VPN traffic could route through the Raspberry Pi to the external internet  
- Saved firewall rules to persist across reboots

### 4. DNS Setup (Optional)

- Installed and configured Unbound for local DNS resolution  
- Tuned resolver settings to block DNS leaks and improve privacy  
- Pointed client configurations to use the Pi as the DNS server

### 5. Client Provisioning

- Generated `.conf` files for each client using PiVPN  
- Created QR codes for easy mobile setup  
- Connected external devices to the VPN and verified IP address masking

---

## Outcome

This project successfully resulted in a lightweight, fully functional VPN server deployed on a Raspberry Pi. It provided practical experience with networking, Linux administration, and secure communication fundamentals. The final setup supports secure remote access, encrypted traffic routing, and can be reused or expanded for homelab environments and travel privacy needs.
