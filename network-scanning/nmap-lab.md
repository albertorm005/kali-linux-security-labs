# Network Scanning with Nmap

## Objective

The goal of this lab is to discover active hosts and services in a local network using Nmap.

## Network Discovery

Command used:

nmap -sn 192.168.1.0/24

Explanation:

- `-sn` : Ping scan (host discovery)
- Scans the local network to identify active hosts

Example result:

Host is up
Host is up
Host is up
6 hosts discovered on the network

## Service Detection

Command used:

nmap -sS -sV TARGET_IP

Explanation:

- `-sS` : SYN scan
- `-sV` : Service version detection

Example result:

PORT     STATE SERVICE
22/tcp   open  ssh
80/tcp   open  http
443/tcp  open  https

## Conclusion

Network scanning is the first step of a penetration test.  
It allows security analysts to identify active devices and exposed services on a network.