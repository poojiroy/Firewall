# Firewall
Enterprise-grade Linux firewall using nftables with DNAT, SNAT, rate limiting, and packet inspection for DDoS protection.


## 🧠 What This Firewall Does (Core Features):

- ✅ **DNAT + SNAT (NAT)** – Acts like a load balancer / gateway
- ✅ **Rate Limiting** – Prevents DDoS and flooding attacks
- ✅ **Port Whitelisting** – Only allows selected ports
- ✅ **Deep Packet Inspection (DPI)** – Drops malicious payloads like `UNION`, `SELECT`, or `python scripts`
- ✅ **Ping Protection** – Limits ICMP echo requests (ping floods)
- ✅ **Logging** – Suspicious packets are logged for audit
- ✅ **Masquerading** – Ensures proper return routing for outgoing traffic

---

## 🛠 Technologies Used

- `nftables`
- `Linux` networking (iptables successor)
- NAT (DNAT & SNAT)
- Rate limiting and DPI
- Terminal/CLI scripting

---

## 🚀 How to Use

1. Copy the firewall rules from `firewall.nft`  
2. Load them into your system:

   ```bash
   sudo nft -f firewall.nft
