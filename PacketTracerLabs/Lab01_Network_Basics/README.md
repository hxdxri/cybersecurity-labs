# Lab 1: Network Basics

## 🎯 Objectives
- Set up a basic network with two PCs
- Configure IP addresses manually
- Test connectivity using ping
- Document network configuration

## 📋 Requirements
- Cisco Packet Tracer
- 2 PCs
- 1 Switch

## 🔧 Configuration Steps

### 1. Network Topology
```
[PC1] ---- [Switch] ---- [PC2]
```

### 2. IP Addressing
- PC1: 192.168.1.10/24
- PC2: 192.168.1.20/24

### 3. Configuration Commands
```
PC1> ipconfig /ip 192.168.1.10 255.255.255.0
PC2> ipconfig /ip 192.168.1.20 255.255.255.0
```

## 📝 Verification Steps
1. Verify IP configuration on both PCs
2. Test connectivity using ping
3. Document successful connection

## 📸 Screenshots
- Network topology
- IP configuration
- Successful ping test

## 📚 Notes
- Basic network setup
- IP addressing fundamentals
- Connectivity testing

## 🎓 Learning Outcomes
- Understanding basic network components
- Manual IP configuration
- Network connectivity verification 