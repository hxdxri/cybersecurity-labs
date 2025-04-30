# Lab 4: VLANs and Trunking

## 🎯 Objectives
- Create and configure VLANs
- Implement trunking between switches
- Test VLAN isolation
- Document network segmentation

## 📋 Requirements
- Cisco Packet Tracer
- 2 Switches
- 4 PCs (2 per VLAN)
- 1 Router (optional for inter-VLAN routing)

## 🔧 Configuration Steps

### 1. Network Topology
```
[PC1] ---- [Switch1] ---- [Switch2] ---- [PC3]
[PC2] ---- [Switch1] ---- [Switch2] ---- [PC4]
```

### 2. VLAN Configuration
- VLAN 10: Sales (192.168.10.0/24)
- VLAN 20: Engineering (192.168.20.0/24)

### 3. Configuration Commands
```
Switch1(config)# vlan 10
Switch1(config-vlan)# name Sales
Switch1(config)# vlan 20
Switch1(config-vlan)# name Engineering
Switch1(config)# interface FastEthernet0/1
Switch1(config-if)# switchport mode trunk
```

## 📝 Verification Steps
1. Verify VLAN assignments
2. Test connectivity within VLANs
3. Test isolation between VLANs
4. Document successful configuration

## 📸 Screenshots
- Network topology
- VLAN configuration
- Trunk configuration
- Successful VLAN isolation tests

## 📚 Notes
- VLAN creation and management
- Trunking configuration
- Network segmentation

## 🎓 Learning Outcomes
- Understanding VLANs
- Trunking implementation
- Network segmentation 