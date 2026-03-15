## 📂 Project Structure

To make this repository easy to navigate, I have organized the files as follows:

* **[Documentation/](Documentation/)**: Contains the full technical report (PDF) covering the step-by-step implementation of Week 2 tasks.
* **[Configuration/](Configuration/)**: Includes the `local_rules.xml` snippets and `ossec.conf` settings used for FIM and Active Response.
* **[Screenshots/](Screenshots/)**: Visual evidence of the Wazuh dashboard alerts, log analysis, and automated firewall blocks.

---

### 🛠️ Technical Deep-Dive

#### 1. Configuration Highlights (`/Configuration`)
In this folder, you will find the custom XML rules I wrote to detect:
- **SSH Brute Force:** Rule ID `100001` (Level 10).
- **User Creation:** Rule ID `100002` (Level 7) for Windows Event ID 4720.

#### 2. Evidence & Results (`/Screenshots`)
Key alerts captured during the simulation:
- **FIM Alert:** Real-time notification when `/etc/test_file` was modified.
- **Active Response:** Evidence of `iptables` dropping the attacker's IP automatically after 5 failed attempts.

---

### 🛡️ How to Use This Repo
1.  Review the **Full Report** in the `Documentation` folder for a detailed walkthrough.
2.  Use the XML snippets in `Configuration` to implement similar detection logic in your own Wazuh environment.
