# Lab 5: Access Control Lists

## 🎯 Objectives
- Configure standard and extended ACLs
- Implement traffic filtering
- Test ACL effectiveness
- Document security policies

## 📋 Requirements
- Cisco Packet Tracer
- 1 Router
- 2 Switches
- 3 PCs
- 1 Server

## 🔧 Configuration Steps

### 1. Network Topology
```
[PC1] ---- [Switch1] ---- [Router] ---- [Switch2] ---- [Server]
[PC2] ---- [Switch1]                           |
[PC3] ---- [Switch1]                           |
```

### 2. IP Addressing
- Internal Network: 192.168.1.0/24
- Server Network: 192.168.2.0/24

### 3. Configuration Commands
```
Router(config)# access-list 1 deny 192.168.1.10
Router(config)# access-list 1 permit any
Router(config)# interface FastEthernet0/0
Router(config-if)# ip access-group 1 in
```

## 📝 Verification Steps
1. Verify ACL configuration
2. Test traffic filtering
3. Document successful implementation

## 📸 Screenshots
- Network topology
- ACL configuration
- Successful traffic filtering tests

## 📚 Notes
- Standard ACL configuration
- Extended ACL configuration
- Traffic filtering rules

## 🎓 Learning Outcomes
- Understanding ACLs
- Traffic filtering
- Network security policies 