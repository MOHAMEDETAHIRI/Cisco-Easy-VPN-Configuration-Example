# Cisco Easy VPN Configuration Example

## Description
This repository contains a sample configuration for Cisco's Easy VPN technology. It simplifies the process of creating LAN-to-LAN VPN tunnels with minimal configuration, enabling VPN connections through simple user authentication.

## Features
- Simplified VPN configuration
- AES-256 encryption
- Pre-shared key (PSK) authentication
- Integration with a Radius server for user authentication
- IPsec with dynamic encryption and ISAKMP policies

## Prerequisites
- Cisco Router with VPN capabilities
- Radius server
- Basic networking knowledge

## Configuration Example
### AAA Configuration
```bash
  aaa new-model
  aaa authentication login VPNAUTH group radius local
  aaa authorization network VPNAUTH local
'''bash
