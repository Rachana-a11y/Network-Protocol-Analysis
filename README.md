# Network-Protocol-Analysis 
# Capture and Analyze Network Traffic Using Wireshark (Task 5)

## 📌 Objective

To capture live network traffic using Wireshark, identify different protocols, and analyze the packet-level details to understand basic communication over the network.

---

## 🧰 Tools & Environment

- **Tool**: [Wireshark](https://www.wireshark.org/)
- **Operating System**: Windows 7 (in VirtualBox)
- **Traffic Sources**: Web browsing, pinging servers
- **Output File**: `.pcap` file

---

## ⚙️ Task Implementation

### 1. Installed Wireshark

- Downloaded and installed Wireshark on the virtual machine.
- Launched the application and selected the **active network interface**.

### 2. Captured Live Network Traffic

- Started packet capture on the selected interface.
- Opened a browser and visited multiple websites.
- Performed a ping to `8.8.8.8` using Command Prompt to generate ICMP traffic.

### 3. Stopped the Capture

- Let the capture run for approximately 1 minute.
- Stopped and saved the capture as `task5_capture.pcap`.

### 4. Applied Filters in Wireshark

Used the following filters to identify different protocols:
- `http` → Captured HTTP packets
- `dns` → Captured DNS queries and responses
- `tcp` and `icmp` → Captured TCP communication and ping responses

### 5. Protocols Identified

- **DNS** – Domain name resolution when browsing.
- **HTTP** – Website requests and responses.
- **ICMP** – Ping packets (used for connectivity testing).
- **TCP** – Underlying reliable transport protocol for browsing.
- **ARP** – Address Resolution Protocol seen in local traffic.

---

## 📁 Repository Contents

- `README.md` – This file
- `task5_capture.pcap` – Exported packet capture file
- `screenshots/` – Screenshots of Wireshark filters and captured packets

---

## 📌 Key Concepts Learned

- Packet capture using Wireshark
- Filtering packets by protocol
- Analyzing headers and payloads of various protocol types
- Observing live DNS, HTTP, ICMP, TCP, and ARP traffic

