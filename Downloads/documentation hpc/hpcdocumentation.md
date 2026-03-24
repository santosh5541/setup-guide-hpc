# 🚀 SDSU HPC SSH Setup Guide (For Undergraduate Students)

---

## 📘 1. Introduction

This guide helps you connect to SDSU High Performance Computing (HPC) systems:

- 🖥️ Innovator Cluster  
- 🖥️ Discovery Cluster  

You will learn:
- How to connect using SSH  
- Common mistakes (real examples)  
- How to fix login issues  

---

## 🧰 2. Requirements

Before starting, make sure you have:

- ✅ USD account  
- ✅ HPC access approved  
- ✅ Internet connection  
- ✅ SSH client installed  

### SSH Clients:
| OS | Tool |
|----|------|
| Windows | PowerShell / Git Bash / PuTTY |
| Mac | Terminal |
| Linux | Terminal |

---

## ⚠️ 3. MOST IMPORTANT: Username Format

This is where most students make mistakes.

### ✅ Correct Format:

yourusername@usd.local@cluster-address


### Example:
santosh.luitel@usd.local@innovator.sdstate.edu


---

## 💻 4. SSH Login Commands

### 🔹 Innovator
```bash
ssh yourusername@usd.local@innovator.sdstate.edu
then enter your usd password

### 🔹 Discovery

ssh yourusername@usd.local@discovery.sdstate.edu
then enter your usd password

### 5. first time login
you may see
Are you sure you want to continue connecting (yes/no)?
type
yes


## 6. REAL ERRORS (From Students) + FIXES
ssh santosh.luitel@usd.local
Error1: Could not resolve hostname usd.local

fix: ssh santosh.luitel@usd.local@innovator.sdstate.edu

Error2: Connection Refused
ssh santosh.luitel@usd.local@discovery.sdstate.edu
❌ Error: connection to host discovery.sdstate.edu port 22: Connection refused

🔍 Possible Causes:
Cluster temporarily down
Network restriction
Firewall issue
✅ Fix:
Try again later
Check with HPC support

🔴 Error 3: Permission Denied
Permission denied, please try again.

🧠 7. Why "Permission Denied" Happens

Based on real case:

Causes:
❌ Wrong password
❌ Wrong username format
🚫 IP address blocked (MOST COMMON)
🚫 8. IP Address Blocking (VERY IMPORTANT)

If you enter the wrong password 3 times, your IP gets blocked.

🔍 Symptoms:
SSH login fails
Browser login works
🌐 9. Verify Using Browser

Try logging in here:

Innovator → https://ondemand.sdstate.edu
Discovery → https://mydiscovery.sdstate.edu
If browser works:

👉 Your credentials are correct
👉 Your IP is likely blocked

🛠️ 10. How to Fix IP Blocking
Step 1: Find Your IP

Go to:
👉 https://www.whatismyipaddress.com

Example:

IPv4: 96.3.185.178
Step 2: Email HPC Support

📧 SDSU.HPC@sdstate.edu


📩 Example Email
Subject: SSH Login Issue (IP Blocked)

Dear HPC Team,

I am unable to login via SSH.

I may have entered incorrect password multiple times.

Details:
- Username: yourusername@usd.local
- Cluster: Innovator / Discovery
- IP Address: xxx.xxx.xxx.xxx

Please unblock my IP.

Thank you.

💡 11. Real Case Summary

A student experienced:

SSH login failed
Browser login worked
Issue → IP blocked
Solution → HPC team unblocked IP

✅ SSH worked again

✅ 12. Best Practices

✔️ Always use correct username format
✔️ Avoid multiple wrong password attempts
✔️ Test login via browser first
✔️ Contact support early

📞 13. Support

📧 SDSU HPC Support
Email: SDSU.HPC@sdstate.edu


📌 14. Quick Summary
Step	Action
1	Use correct SSH format
2	Enter correct password
3	Try browser login
4	If SSH fails → check IP block
5	Contact support
🎯 Final Tip

💬 90% of SSH issues = wrong format OR IP block

Be patient, and you’ll get connected quickly!

