# Lab 3: DHCP and NAT

## 🎯 Objectives
- Configure DHCP server for automatic IP assignment
- Implement NAT for Internet connectivity
- Test DHCP functionality
- Document network configuration

## 📋 Requirements
- Cisco Packet Tracer
- 1 Router
- 1 Switch
- 2-3 PCs
- 1 Server (for DHCP)

## 🔧 Configuration Steps

### 1. Network Topology
```
[PCs] ---- [Switch] ---- [Router] ---- [Internet]
```

### 2. IP Addressing
- Internal Network: 192.168.1.0/24
- External Network: 203.0.113.0/24
- DHCP Pool: 192.168.1.10-192.168.1.50

### 3. Configuration Commands
```
Router(config)# ip dhcp pool INTERNAL
Router(dhcp-config)# network 192.168.1.0 255.255.255.0
Router(dhcp-config)# default-router 192.168.1.1
Router(config)# ip nat inside source list 1 interface FastEthernet0/1 overload
```

## 📝 Verification Steps
1. Verify DHCP assignments on PCs
2. Test NAT functionality
3. Document successful configuration

## 📸 Screenshots
- Network topology
- DHCP server configuration
- NAT configuration
- Successful IP assignment

## 📚 Notes
- DHCP server configuration
- NAT implementation
- Network address translation

## 🎓 Learning Outcomes
- Understanding DHCP
- NAT configuration
- Network automation 