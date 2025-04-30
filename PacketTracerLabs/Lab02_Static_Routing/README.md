# Lab 2: Static Routing

## 🎯 Objectives
- Configure static routes between multiple networks
- Understand routing tables
- Test connectivity across different networks
- Document routing configuration

## 📋 Requirements
- Cisco Packet Tracer
- 2 Routers
- 3 Networks
- 2 PCs

## 🔧 Configuration Steps

### 1. Network Topology
```
[PC1] ---- [Router1] ---- [Router2] ---- [PC2]
    |           |             |
  Network1   Network2     Network3
```

### 2. IP Addressing
- Network1: 192.168.1.0/24
- Network2: 192.168.2.0/24
- Network3: 192.168.3.0/24

### 3. Configuration Commands
```
Router1(config)# ip route 192.168.3.0 255.255.255.0 192.168.2.2
Router2(config)# ip route 192.168.1.0 255.255.255.0 192.168.2.1
```

## 📝 Verification Steps
1. Verify routing tables on both routers
2. Test connectivity between PC1 and PC2
3. Document successful routing

## 📸 Screenshots
- Network topology
- Router configurations
- Successful ping test between networks

## 📚 Notes
- Static routing configuration
- Network segmentation
- Routing table management

## 🎓 Learning Outcomes
- Understanding static routing
- Network segmentation
- Router configuration 