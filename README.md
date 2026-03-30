
# ServiceNow MID Server Installation & Configuration (Windows x86-64)

## 🚀 Project Overview
This project demonstrates the end-to-end installation, configuration, and validation of a **ServiceNow MID Server** in a Windows environment.

The MID Server plays a critical role in enabling **secure communication between ServiceNow and on-premises infrastructure**, which is essential for use cases such as:
- Discovery
- Orchestration
- Integration with internal systems

---

## 🎯 Business Use Case
Organizations often need to connect ServiceNow with internal systems behind firewalls.  
In this project, I simulated that real-world scenario by deploying and configuring a MID Server to establish secure communication with my ServiceNow instance.

---

## 🛠️ Skills Demonstrated
- ServiceNow Administration  
- MID Server Deployment & Configuration  
- Windows Server & Command Line  
- Integration Architecture (ServiceNow ↔ On-Prem Systems)  
- Troubleshooting & Root Cause Analysis  
- Secure Credential Management  
- Technical Documentation  

---

## ⚙️ Architecture Overview
ServiceNow Instance ↔ MID Server ↔ Local Machine (Simulated On-Prem Environment)

- Communication handled via **ECC Queue**
- Secure outbound connection (no inbound firewall exposure required)

---

## 📂 Implementation Steps

### 1. Installed MID Server
- Downloaded correct Windows x86-64 package  
- Extracted while preserving directory structure  

---

### 2. Configured MID Server (`config.xml`)
Updated key parameters:

```xml
<parameter name="url" value="https://YOUR_INSTANCE.service-now.com"/>
<parameter name="mid.instance.username" value="mid.server"/>
<parameter secure="true" name="mid.instance.password" value="********"/>
<parameter name="name" value="demo_mid_server"/>
````

---

### 3. Created ServiceNow MID Server User

* Assigned **mid_server role**
* Ensured account was active and secure

---

### 4. Troubleshooting & Issue Resolution

Encountered Windows path execution errors due to long directory names.

✅ Solution:

```cmd
cd "C:\Users\shaki\Downloads\mid.zurich...\agent"
start.bat
```

Also validated:

* Java availability
* Correct credentials
* Network connectivity

---

### 5. Started MID Server Service

Successfully initialized the MID Server:

* Service installed and running
* Agent connected to instance

---

### 6. Validation in ServiceNow

* MID Server visible under **MID Server → Servers**
* Status: ✅ **Up**
* Verified communication via ECC Queue

---

## 📸 Proof of Work

Command Prompt showing successful startup

<img width="1310" height="627" alt="Screenshot 2026-03-30 160632" src="https://github.com/user-attachments/assets/f2a2228e-c01a-49b0-8687-a67532d2ecfc" />

MID Server record with “Up” status

<img width="1276" height="267" alt="Screenshot 2026-03-30 161131" src="https://github.com/user-attachments/assets/fd83dba1-481b-4470-90d1-34d60be6cb52" />

Edited config.xml

<img width="830" height="480" alt="image" src="https://github.com/user-attachments/assets/3bae8e69-2bcb-4819-b70c-a0a00cd64baf" />

MID Server user record

<img width="1600" height="857" alt="Screenshot 2026-03-30 114225" src="https://github.com/user-attachments/assets/92dd83fa-bd76-464f-a742-2611edb0cef1" />

---

## 📘 Key Learnings

* How MID Servers enable **secure enterprise integrations**
* Importance of **ECC Queue in ServiceNow communication**
* Real-world troubleshooting of environment setup issues
* Hands-on experience with **infrastructure-level components**

---

## 🚀 Future Enhancements

* Configure **ServiceNow Discovery using MID Server**
* Integrate with external systems (e.g., database or API)
* Automate tasks using Orchestration workflows

---

## ✨ Author

**Shakirāt Odin**
ServiceNow Engineer | ITSM | Automation | Integration

```

---

# 💡 Why This Version Is Better
- Adds **business context** (huge for recruiters)
- Shows **architecture understanding**
- Highlights **problem-solving (critical skill)**
- Includes **future roadmap** (shows growth mindset)

---

# 🔥 Next Power Move (VERY IMPORTANT)
Now that you’ve done this:

👉 Your next GitHub project should be:
- **ServiceNow Discovery using MID Server**  
or  
- **Integration (REST API or Orchestration)**  

That combination = 🔥 *job-ready profile*

---

# 💬 Want Me to Go Further?
I can help you:
- Turn this into a **LinkedIn post that attracts recruiters**
- Suggest **GitHub repo naming + tags for visibility**
- Build your **next project (Discovery step-by-step on your PDI)**

Just tell me 👍
```
