TryHackMe - Networking Basics Write-up

Overview

This write-up covers my first networking fundamentals learning path on TryHackMe.

The goal was to understand the basics of networking and how they apply to cybersecurity.

Topics covered:

IP Address

DNS

Ports

TCP vs UDP

Basic networking commands



---

Tools Used

Kali Linux

Nmap

Terminal

Browser

TryHackMe



---

1. IP Address

What it is

An IP address is a unique address used to identify a device on a network.

It helps devices communicate with each other.


---

Example

192.168.1.10

This could be the address of a laptop connected to a home Wi-Fi network.


---

Why it matters in cybersecurity

Attackers use IP addresses to find and target systems.

Security professionals use them for:

scanning networks

identifying suspicious traffic

locating attack sources


For example, Nmap scans IP addresses to discover active machines.


---

2. DNS

What it is

DNS (Domain Name System) translates domain names into IP addresses.

Instead of remembering an IP address, users type a domain name like google.com.

DNS finds the correct IP address for that website.


---

Example

ping google.com

This command helps show the IP address linked to that domain.


---

Why it matters in cybersecurity

Attackers use DNS for:

finding hidden subdomains

discovering internal systems

phishing attacks using fake domains


Defenders monitor DNS activity to detect suspicious behavior.


---

3. Ports

What it is

Ports are numbered communication channels used by services.

Different services use different ports.


---

Example

22 → SSH
80 → HTTP
443 → HTTPS


---

Why it matters in cybersecurity

If a port is open, it may expose a service that can be attacked.

Example: If port 22 is open, attackers may try to gain SSH access.

This is why port scanning is important.


---

4. TCP vs UDP

What it is

TCP and UDP are two transport protocols used for sending data.

TCP is reliable and checks if data arrives correctly.

UDP is faster but does not confirm delivery.


---

Example

TCP → Login pages, websites

UDP → Streaming, gaming, voice calls



---

Why it matters in cybersecurity

Different scans and attacks behave differently depending on whether the target uses TCP or UDP.

Understanding both helps during network scanning and exploitation.


---

5. Commands Used

Basic Commands

ping google.com
ipconfig
ifconfig
nmap -sV <target-ip>

What they do

ping → checks connectivity

ipconfig → shows IP info on Windows

ifconfig → shows IP info on Linux

nmap → scans open ports and services



---

Lessons Learned

I learned that open ports reveal possible attack surfaces

I understood how DNS helps both users and attackers

I learned why IP addresses are important during scanning

I understood the difference between TCP and UDP



---

How to Prevent Attacks

Security teams can reduce risks by:

closing unnecessary ports

using strong passwords for exposed services

monitoring DNS activity

limiting public exposure of sensitive systems

keeping systems updated
