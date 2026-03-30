# ServiceNow MID Server Installation & Configuration (Windows x86‑64)

This project demonstrates the complete installation, configuration, and validation of a **ServiceNow MID Server** on a Windows environment. It highlights my ability to work with enterprise integration components, troubleshoot system issues, and document technical processes clearly.

---

## 🚀 Project Overview
The ServiceNow MID Server enables secure communication between the ServiceNow platform and on‑premises systems. 
In this project, I installed and configured a MID Server, resolved Windows command‑line issues, and validated successful connectivity to my ServiceNow instance.

---

## 🛠️ Skills Demonstrated
- ServiceNow Administration  
- Windows Command Line & Services  
- XML Configuration  
- Integration & Automation  
- Troubleshooting & Debugging  
- Secure Credential Handling  
- Technical Documentation  

---

## 📂 Project Steps

### **1. Downloaded and extracted the MID Server package**
- Selected the correct Windows x86‑64 build  
- Ensured folder structure remained intact  

---

### **2. Configured `config.xml`**
Key parameters included:

```xml
<parameter name="url" value="https://YOUR_INSTANCE.service-now.com"/>
<parameter name="mid.instance.username" value="mid.server"/>
<parameter secure="true" name="mid.instance.password" value="********"/>
<parameter name="name" value="demo_mid_server"/>

3. Created a dedicated MID Server user
Assigned the mid_server role
Ensured the account was active and not locked

4. Resolved Windows path and execution errors
Used quotes to handle long folder names:
cd "C:\Users\shaki\Downloads\mid.zurich...\agent"
start.bat

5. Started the MID Server service
Observed successful startup messages:
“ServiceNow MID Server service installed”
“ServiceNow MID Server service started”

6. Validated in ServiceNow
MID Server appeared under MID Server → Servers
Status: Up
Logged‑in user: mid.server

📸 Screenshots
Command Prompt showing successful startup

<img width="1310" height="627" alt="Screenshot 2026-03-30 160632" src="https://github.com/user-attachments/assets/f2a2228e-c01a-49b0-8687-a67532d2ecfc" />

MID Server record with “Up” status

<img width="1276" height="267" alt="Screenshot 2026-03-30 161131" src="https://github.com/user-attachments/assets/fd83dba1-481b-4470-90d1-34d60be6cb52" />

Edited config.xml

<img width="830" height="480" alt="image" src="https://github.com/user-attachments/assets/3bae8e69-2bcb-4819-b70c-a0a00cd64baf" />

MID Server user record

<img width="1600" height="857" alt="Screenshot 2026-03-30 114225" src="https://github.com/user-attachments/assets/92dd83fa-bd76-464f-a742-2611edb0cef1" />

What This Project Demonstrates

Ability to configure enterprise‑grade integration components
Strong troubleshooting and debugging skills
Understanding of ServiceNow architecture and ECC Queue
Clear, structured documentation
Hands‑on technical execution

✨ Author
Shakirāt Odin
Richmond, Texas
Focused on ServiceNow, ITSM, automation, and real‑world technical problem‑solving.



