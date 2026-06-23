# CodeAlpha_NetworkSniffer
# Basic Network Sniffer

## Objective

The objective of this project is to capture and analyze live network 
packets using Python and Scapy, and to understand how data flows 
through a network at the protocol level.

## Tools Used

- Python 3
- Scapy
- Npcap (Windows Packet Capture Driver) / libpcap (Linux)

## Features

- Captures live network packets in real time
- Displays source and destination IP addresses
- Identifies protocol type (TCP, UDP, ICMP)
- Shows source and destination port numbers
- Displays packet length and payload preview
- Supports BPF filters (e.g. capture only HTTP or DNS)
- Optional session logging to a text file

## How to Run

```bash
pip install scapy
sudo python3 sniffer.py -i eth0
