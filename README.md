Home Network Static IP Guide

This guide explains how I fixed two common home Wi-Fi problems by assigning static IP addresses:

HP DeskJet 2600 printer not scanning or going offline

LG Smart TV frequently disconnecting from Wi-Fi

Static IPs made both devices fully stable.

Overview

Most home routers use dynamic IP addresses.
When the IP changes, devices like printers and TVs disconnect.

A static IP keeps the same address forever and prevents:
offline errors, not found errors, and random disconnections.

1. Fix: HP DeskJet 2600 Scan & Offline Problems
Why HP scan fails on Windows 10/11

HP removed the full driver package for old models.
Windows now installs only a basic print driver with no scanner driver.

HP Smart is the only working way to scan.

Step 1 — Assign a Static IP (Example: 192.168.0.200)

Log into your router → DHCP Settings → Address Reservation
Reserve a permanent IP for your printer.

Example values:

IP Address: 192.168.0.200

MAC Address: find this on the printer’s Wi-Fi or Network Report page

Save the reservation.

Step 2 — Reconnect the Printer to Wi-Fi

Hold Wi-Fi + Cancel on the printer to reset network

Reconnect to your home Wi-Fi

Printer will now always use the reserved static IP

Step 3 — Use HP Smart to Scan

Install HP Smart from the Microsoft Store.
The DeskJet 2600 does not support WebScan.
Visiting http://192.168.0.200/scan
 will always show an error.
Scanning works only through HP Smart.

2. Fix: LG Smart TV Wi-Fi Disconnecting

After assigning a static IP (example: 192.168.0.210):

On the TV, go to:
Settings → Network → Wi-Fi → Advanced Settings

Enter these values:

IP Address: 192.168.0.210

Subnet Mask: 255.255.255.0

Gateway: 192.168.0.1

DNS: 8.8.8.8

Save and reconnect.
Your TV Wi-Fi should now stay stable.
