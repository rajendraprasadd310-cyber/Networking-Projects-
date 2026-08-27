# 🌐 Static Routing Network using Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the implementation of **Static Routing** in a small enterprise network using **Cisco Packet Tracer**. The network consists of multiple LANs connected through two Cisco routers, enabling communication between different departments and servers.

---

## 🛠 Technologies Used

- Cisco Packet Tracer
- Cisco 2911 Routers
- Cisco 2960 Switches
- Static Routing
- IPv4 Addressing

---

## 📖 Network Topology

The network contains:

- 2 Cisco 2911 Routers
- 2 Cisco 2960 Switches
- 4 PCs
- 2 Servers

### Networks

| Network | Purpose |
|----------|---------|
| 10.0.0.0/24 | HR Department |
| 20.0.0.0/24 | Finance Department |
| 30.0.0.0/24 | Web Server |
| 40.0.0.0/24 | FTP Server |
| 50.0.0.0/24 | Router-to-Router WAN Link |

---

## 📂 IP Addressing

### Router0

| Interface | IP Address |
|-----------|------------|
| GigabitEthernet0/0 | 10.0.0.3/24 |
| GigabitEthernet0/1 | 20.0.0.3/24 |
| GigabitEthernet0/2 | 50.0.0.1/24 |

### Router2

| Interface | IP Address |
|-----------|------------|
| GigabitEthernet0/0 | 30.0.0.3/24 |
| GigabitEthernet0/1 | 40.0.0.3/24 |
| GigabitEthernet0/2 | 50.0.0.2/24 |

### End Devices

| Device | IP Address |
|---------|------------|
| HR-PC1 | 10.0.0.1 |
| HR-PC2 | 10.0.0.2 |
| FIN-PC1 | 20.0.0.1 |
| FIN-PC2 | 20.0.0.2 |
| Web Server | 30.0.0.1 |
| FTP Server | 40.0.0.1 |

---

## ⚙️ Static Routes

### Router0

```bash
ip route 30.0.0.0 255.255.255.0 50.0.0.2
ip route 40.0.0.0 255.255.255.0 50.0.0.2
```

### Router2

```bash
ip route 10.0.0.0 255.255.255.0 50.0.0.1
ip route 20.0.0.0 255.255.255.0 50.0.0.1
```

---

## ✅ Features

- Static routing between multiple networks
- Router-to-router communication
- End-to-end connectivity
- Multiple LAN segments
- Web and FTP server connectivity
- Routing table verification
- Network testing using ping and traceroute

---

## 🧪 Verification

The following commands were used to verify the network configuration:

```bash
show ip interface brief
show ip route
show running-config
ping
tracert
```

---

## 📷 Project Screenshots

Add the following screenshots:

- Network Topology
- Router0 Routing Table
- Router2 Routing Table
- Successful Ping Results
- Traceroute Results

---

## 📚 Learning Outcomes

Through this project, I learned:

- IPv4 network addressing
- Static routing configuration
- Cisco router configuration
- LAN and WAN connectivity
- Routing table analysis
- Network troubleshooting
- End-to-end connectivity testing

---

## 🚀 Future Improvements

- Implement Dynamic Routing (RIP, OSPF, EIGRP)
- Configure VLANs
- Add Access Control Lists (ACLs)
- Configure DHCP and DNS services
- Enable SSH for secure remote management
- Implement network security features

---

## 👨‍💻 Author

**Rajendra Prasad D**

Aspiring SOC Analyst | Cybersecurity Enthusiast
