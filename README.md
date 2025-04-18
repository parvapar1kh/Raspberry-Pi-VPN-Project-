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

## Outcome/Purpose

This project led to a fully working VPN server built on a Raspberry Pi, using WireGuard for secure and private connections. Setting it up gave me hands-on experience with networking basics, Linux commands, and system configuration. The VPN is lightweight, runs reliably, and allows for secure remote access to my home network --- whether for personal use, testing, or just browsing privately on public Wi-Fi. I wanted something that was both practical and a good learning tool, and this setup delivered. It’s especially useful when traveling, since I can route traffic through my home network and avoid restrictions or tracking. On top of that, working through this lab helped me better understand key topics like firewalls, NAT, DNS, and VPN tunneling. It’s a solid project for anyone building a cybersecurity portfolio or wanting to get real experience setting up secure infrastructure on a budget.


