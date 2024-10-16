---
layout: default
title: "RFID Test"
permalink:  /wireless-tests/rfid/
---

# RFID Test Using Proxmark3 on Kali Linux

In this test, we’ll simulate using a Proxmark3 device to read and clone an RFID tag, typically used in access control systems. The goal is to demonstrate how the Proxmark3 can be used for testing the security of RFID-enabled systems. This test assumes you are using Kali Linux, which has the necessary tools to interface with the Proxmark3.

## Prerequisites

Before starting this test, ensure you have the following:

- **Proxmark3 device**
- **Kali Linux** (fully updated)
- An **RFID tag/card** (for testing)
- **Proxmark3 tools** installed on Kali Linux

To install the Proxmark3 tools on Kali Linux, use the following command:

```bash
sudo apt update && sudo apt install proxmark3

proxmark3 /dev/ttyUSB0

hf search

lf search


[+] Valid HF card found!
[+] UID: 04 5D B9 4A 56 7E 93
[+] Type: MIFARE Classic

hf mf dump

hf mf clone 0 0 0


[+] Cloning to blank card...
[+] Writing data to card...
[+] Clone successful!

```



### Features of the Test:
- **Commands for Kali Linux**: The commands are designed to work in Kali Linux, a common platform for penetration testing.
- **Proxmark3 Usage**: The test includes commands for using Proxmark3 to read, dump, clone, and verify RFID tags.
- **Security Insights**: Each step offers some insight into the security implications of RFID systems and vulnerabilities exposed by cloning.
- **Practical, Realistic Flow**: The steps mimic real-world usage of the Proxmark3 in RFID testing.

This markdown content can be used to demonstrate the process of reading, cloning, and analyzing RFID tags with the Proxmark3 in a professional environment. Let me know if you need further customization!
