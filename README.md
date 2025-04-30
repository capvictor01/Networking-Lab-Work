

# 8-Floor Building Network Topology Design

This project outlines the network topology and configuration plan for an 8-floor building. Each floor employs a distinct network topology and integrates various network services including DHCP, DNS, HTTP, and Email, showcasing a realistic and modular network setup suitable for educational, testing, or small enterprise simulation environments.

## 📐 Floor-by-Floor Topology

| Floor | Topology Type           | Devices | Network ID        | Special Configuration           |
|-------|-------------------------|---------|-------------------|----------------------------------|
| 1     | Hybrid                  | 8 PCs   | 193.168.11.0      | None                             |
| 2     | Hybrid (Mesh + Star)    | 8 PCs   | 193.168.11.16     | None                             |
| 3     | Hybrid (Ring + Star)    | 8 PCs   | 193.168.11.32     | None                             |
| 4     | Mesh                    | 8 PCs   | 193.168.11.48     | None                             |
| 5     | Mesh                    | 3 PCs + DHCP Server | 193.168.11.66 | DHCP Configuration              |
| 6     | Mesh                    | 8 PCs + DNS Server | 193.168.11.80 | DNS Configuration               |
| 7     | Bus                     | 8 PCs + HTTP Server | 193.168.11.96 | HTTP Server Configuration       |
| 8     | Bus                     | 8 PCs + Email Server | 193.168.11.112 | Email Server Configuration     |

## 🔁 Dynamic Routing

The building uses dynamic routing implemented through 8 routers to ensure inter-floor connectivity and network resilience. Each router is placed to manage routing operations per floor, supporting scalable communication.

## ⚙️ Network Services

- **DHCP** – Configured on Floor 5 to assign dynamic IP addresses.
- **DNS** – Hosted on Floor 6 to resolve domain names within the local network.
- **HTTP Server** – Set up on Floor 7 for web-based services.
- **Email Server** – Installed on Floor 8 for internal communications.

## 🌐 IP Addressing

The network design uses segmented class C IP addresses in the 193.168.11.0/24 range, allocating unique subnets per floor to manage broadcast domains effectively.

## 📁 File Contents

This repository may include:
- `.pkt` simulation files (if done in Cisco Packet Tracer)
- Configuration scripts for routers and services
- Documentation and diagrams (optional)

## 🧑‍💻 Author

Victor Paul

---

