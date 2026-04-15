<<<<<<< HEAD
# 📡 Network Traffic Capture and Analysis using Wireshark (Kali Linux)

---

## 🎯 Objective

The objective of this task is to capture live network traffic and analyze HTTP packets using Wireshark in a Kali Linux environment. This demonstrates how unencrypted data can be monitored and inspected.

---

## 🛠️ Tools Used

* **Wireshark** (Packet Analyzer)
* **Kali Linux** (Operating System)

---

## ⚙️ Methodology / Steps Performed

### 1. Launch Wireshark

Wireshark was opened using terminal and the available network interfaces were displayed.

### 2. Select Network Interface

The active interface (`wlan0` for Wi-Fi) was selected to begin capturing live packets.

### 3. Start Packet Capture

Once the interface was selected, Wireshark started capturing all incoming and outgoing network traffic in real-time.

### 4. Generate Network Traffic

To generate HTTP traffic, the following websites were accessed:

* http://example.com
* http://testphp.vulnweb.com
* http://neverssl.com

These sites were chosen because they use **HTTP protocol**, which is not encrypted.

### 5. Apply Filter

To isolate relevant packets, the following display filter was applied:

```
http
```

This filtered out all non-HTTP packets and displayed only HTTP requests and responses.

### 6. Packet Analysis

Individual packets were analyzed to observe key details such as:

* Source IP Address
* Destination IP Address
* Request Method (GET / POST)
* Host Name (Website)
* User-Agent Information

### 7. Save Capture File

The captured traffic was saved as:

```
wireshark_capture.pcap
```

---

## 🔍 Observations / Analysis

* Multiple **HTTP GET requests** were captured successfully.
* The **source IP address** corresponds to the local machine.
* The **destination IP address** belongs to the web server.
* HTTP headers such as **Host** and **User-Agent** were visible.
* Since HTTP is **unencrypted**, all data can be easily read.

---

## ⚠️ Security Insight

This experiment clearly shows that:

* HTTP traffic is **not secure**
* Sensitive data transmitted over HTTP can be intercepted
* Attackers can use tools like Wireshark for **packet sniffing**

👉 This highlights the importance of using **HTTPS**, which encrypts data and prevents unauthorized access.

---

## 📁 Files Included

* `wireshark_capture.pcap` → Captured network traffic file
* `README.md` → Documentation of the task

---

## 🎥 Demo (Optional)

A demonstration video can include:

* Launching Wireshark
* Starting packet capture
* Visiting HTTP websites
* Applying filter (`http`)
* Analyzing packets

---

## ✅ Conclusion

Wireshark is a powerful network analysis tool that allows real-time monitoring of network traffic. This task demonstrates how unencrypted HTTP traffic can be captured and analyzed, emphasizing the importance of secure communication protocols like HTTPS.

---

## 🚀 Learning Outcome

* Understanding of packet sniffing
* Hands-on experience with Wireshark
* Ability to analyze network protocols
* Awareness of network security risks

---

## 👨‍💻 Author

Jayant Patil
