# 🦈 Wireshark Filters – Crash Cheat Sheet  

A **quick reference guide** for Wireshark filters 🎯.  
Use it while analyzing packets in your **lab or authorized networks** ✅.  

---

## 👨‍💻 Author Introduction  

Hello! I am **Muhammad Saqlain Shoukat** also known as **Dark Wolf** founder and developer of **Coding Chat Room**, a passionate learner and creator in the field of **Cybersecurity, Programming, and DevSecOps**.  

🔹 My mission is to make **complex technical concepts simple and easy** so that students and professionals can learn without confusion.  
🔹 On my platforms, I share tutorials, study notes, and practical tips about **Linux, Ethical Hacking, Development, Programming and Cybersecurity**.  
🔹 I believe in **learning by sharing** — the more we teach, the more we grow.  

---

## 🌐 Basic Protocol Filters  

| 🔍 **Filter** | 📌 **Use Case** |
|--------------|----------------|
| `icmp` | Show **Ping** requests & replies |
| `dns` | Show **Domain name lookups** |
| `http` | Show **Web traffic** (GET/POST) |
| `https` | Show **Encrypted web traffic** |
| `ftp` | Show **File transfers** (sometimes creds visible 😱) |
| `ssh` | Show **Encrypted remote shell traffic** |
| `arp` | Show **IP ↔ MAC mapping** |

---

## 🖧 IP & Port Filters  

| 🔍 **Filter** | 📌 **Use Case** |
|--------------|----------------|
| `ip.addr == 192.168.1.1` | Show **all traffic** of one IP |
| `ip.src == 192.168.1.10` | Show only **source IP** traffic |
| `ip.dst == 192.168.1.20` | Show only **destination IP** traffic |
| `tcp.port == 80` | Show **HTTP** packets |
| `udp.port == 53` | Show **DNS queries** |
| `tcp.port == 443` | Show **HTTPS** packets |

---

## 🔎 TCP Analysis  

| 🔍 **Filter** | 📌 **Use Case** |
|--------------|----------------|
| `tcp.flags.syn == 1` | Show **SYN** packets (handshake start 🤝) |
| `tcp.flags.fin == 1` | Show **FIN** packets (connection close 🔚) |
| `tcp.analysis.retransmission` | Detect **network issues** (retransmits) |

---

## 🛠 Combo & Security Filters  

| 🔍 **Filter** | 📌 **Use Case** |
|--------------|----------------|
| `http || dns` | Show both **HTTP & DNS** traffic |
| `ip.addr == 192.168.1.5 && http` | Show **HTTP traffic of one IP** |
| `http.contains "password"` | Find packets containing **passwords** 🔑 |
| `http.request.method == "POST"` | Show only **POST requests** (logins 👤) |

---

## ⚡ Quick Notes  

- ✅ Use **filters** to save time and focus on important packets.  
- 🚀 Great for **hackers & security analysts**.  
- ⚠️ Always capture traffic **ethically & legally**.  

---

✨ *Made for learners who want to master Wireshark fast!* 🚀 
> **Watch Demo**: You can also watch demo for its learning from here 👉: [wireshark in 1 Video](https://youtu.be/MgxZSFRlu-M?si=HmPIdj00dbqQZM1-)

---

## 📚 More Learning & Connect with Me

If you found this helpful and want to learn more about **search tricks, cybersecurity, and coding**, follow me here and **Star this Resporatory**:

- 🎥 **YouTube**: [Coding Chat Room](https://www.youtube.com/@CodingChatRoom)  
- 📸 **Instagram**: [@codingchatroom](https://www.instagram.com/codingchatroom/?igsh=czBrcjAyYmxma2du)
- 💻 GitHub: [Coding Chat Room](https://github.com/CodingChatRoom)

💡 I share tutorials, tips, and resources to make learning **cybersecurity and coding easier**.  
Don’t forget to **subscribe & follow** for more updates and **Star this Resporatory** 🚀  
