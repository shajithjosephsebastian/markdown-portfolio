# 🖥️ TryHackMe — *Machine Name* Walkthrough

## 📌 Overview

| Field              | Info                            |
| ------------------ | ------------------------------- |
| **Room Name**      | MACHINE_NAME                    |
| **Difficulty**     | Easy/Medium/Hard                |
| **Category**       | Linux / Windows / Web / PrivEsc |
| **Author**         | TryHackMe                       |
| **Walkthrough By** | Shajith Joseph Sebastian        |

---

## 🔍 1. Enumeration

### **Nmap Scan**

```bash
nmap -sC -sV -oN nmap.txt <TARGET-IP>
```

**Findings:**

* Port 22 — SSH
* Port 80 — Apache
* Port XXXX — Service info...

---

## 🌐 2. Web Enumeration

### Gobuster

```bash
gobuster dir -u http://<TARGET-IP> -w /usr/share/wordlists/dirb/common.txt
```

Findings:

* `/admin`
* `/uploads`
* etc.

Screenshots can be added like:

```
![Screenshot](../assets/images/machine-name/web1.png)
```

---

## 🎯 3. Initial Foothold

Explain exploit, code, vulnerability etc.

---

## ⚡ 4. Privilege Escalation

Detail:

* SUID
* Cron
* PATH hijack
* Kernel exploit
* Capabilities
* Weak permissions
* etc.

Add commands:

```bash
find / -type f -perm -4000 2>/dev/null
```

---

## 🏁 5. Root Flag

```
cat /root/root.txt
```

---

## 📜 Conclusion

Short summary, attack path, lessons learned.

---

# DONE.
