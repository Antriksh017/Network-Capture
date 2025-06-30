# 📡 Capture and Analyze Network Traffic Using Wireshark (Windows)

## 🧾 Objective

The goal of this project is to use **Wireshark**, a free and open-source packet analyzer, to capture live network packets on a Windows machine and identify basic protocols and traffic types such as DNS, HTTP, HTTPS, TCP, and UDP.

---

## 🛠️ Tools Used

- **Wireshark** (https://www.wireshark.org/) – for capturing and analyzing network traffic  
- **Windows 10/11** – operating system  
- **Web Browser / Command Prompt** – to generate test traffic during the capture

---

## 📸 Task Performed

1. **Installed Wireshark** on Windows with Npcap for packet capturing.
2. **Launched Wireshark as Administrator** to access all network interfaces.
3. **Selected the active network interface** (Wi-Fi/Ethernet).
4. **Started packet capture** and generated traffic by:
   - Visiting websites in a browser
   - Using `ping` and `nslookup` in Command Prompt
5. **Stopped the capture** after collecting enough traffic data.
6. **Saved the capture file** as `.pcap` format.
7. **Analyzed the captured traffic** using:
   - Protocol Hierarchy
   - Packet List and Details pane

---

## 📊 Protocols Identified

| Protocol | Port | Description                          |
|----------|------|--------------------------------------|
| DNS      | 53   | Domain name resolution               |
| HTTP     | 80   | Web traffic (unencrypted)            |
| HTTPS    | 443  | Secure web traffic (SSL/TLS)         |
| TCP      | —    | Reliable connection protocol         |
| UDP      | —    | Fast, connectionless communication   |
| ICMP     | —    | Used in tools like `ping`            |

---

## 📂 Deliverables

- `network_capture.pcap` – Wireshark capture file containing raw network data  
- `report.md` – Brief analysis of identified protocols and their purposes

---

## 📎 Sample Commands Used to Generate Traffic

```bash
ping google.com
nslookup openai.com
