# Basic Network Sniffer

## Overview

The objective of this project is to build a real-time packet 
capturing tool using Python and Scapy that helps visualize 
how network communication works at the packet level, including 
protocol identification and traffic analysis.

## Technologies & Libraries

- Python 3
- Scapy Library
- Npcap (Windows) / libpcap (Linux/macOS)
- Command Line / Terminal

## Capabilities

- Listens on any available network interface
- Captures and parses TCP, UDP and ICMP packets
- Extracts and displays source IP, destination IP and ports
- Shows packet size and a decoded payload preview
- BPF filter support to target specific traffic
- Saves captured session to a log file

## Installation & Usage

```bash
pip install scapy

# Basic capture on wlan0
sudo python3 sniffer.py -i wlan0

# Capture only DNS traffic and save to file
sudo python3 sniffer.py -i wlan0 -f "udp port 53" -o log.txt
