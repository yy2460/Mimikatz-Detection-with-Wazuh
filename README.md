# 🔐 Mimikatz Detection with Wazuh 🛡️

## 🚀 Overview
This project demonstrates the creation of a custom rule in Wazuh to detect **Mimikatz**, a popular credential dumping tool used in cyber attacks. By leveraging **Sysmon logs**, this custom rule is tailored to spot Mimikatz activity even when the executable is renamed, ensuring your systems are protected against stealthy attacks.
![image](https://github.com/user-attachments/assets/23aaf254-f297-48a7-8fe4-bef29a951000)

## 🔧 Features
- **Custom Rule Creation**: Learn how to create and configure custom detection rules in Wazuh.
- **Sysmon Integration**: Utilizes **Sysmon Event ID 1** to capture detailed file information and activity.
- **Mimikatz Detection**: Specifically designed to detect the execution of Mimikatz by monitoring file names.
- **Robust Alerting**: Ensures that alerts are triggered even when the Mimikatz executable is renamed or obfuscated.
- **MITRE ATT&CK Mapping**: Maps Mimikatz activity to the **MITRE ATT&CK framework** for credential dumping (**T1071.001**).

## 📝 What You’ll Learn
- How to manage and customize Wazuh rules.
- How **Sysmon** and **Wazuh** can work together for advanced threat detection.
- Best practices for creating effective security alerts.
- How to handle **rule IDs**, **severity levels**, and **field values**.
- Understanding **case sensitivity** in rule creation.

## 💡 Why This Matters
Mimikatz is often used in post-exploitation attacks to dump credentials from a compromised system. This project will help you build a reliable detection mechanism to identify Mimikatz activity, even in advanced scenarios where attackers try to rename or alter the tool to bypass traditional detection systems.

## 🔍 How It Works
1. **Search and Modify Sysmon Rule**:  
   We start by searching for existing Sysmon rules related to Event ID 1 in Wazuh.
   
2. **Customization of Rule**:  
   We edit the rule ID, severity, and field name to specifically look for Mimikatz-related activity.

3. **Testing the Rule**:  
   Run a test by renaming the Mimikatz executable and check if the alert triggers correctly.

## 📸 Screenshots
(Here, add a screenshot of the Wazuh dashboard showing the alert triggered by the renamed Mimikatz executable.)

## 📁 Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/yy2460/mimikatz-detection-wazuh.git
2. Follow the instructions in the README.md file for configuring Sysmon and Wazuh.
3. Customize your Wazuh rules according to the provided example.
4. Restart Wazuh manager and validate the rule with a test run.

## 🛠️ Technologies Used
1. **Wazuh**: For security information and event management (SIEM).
2. **Sysmon**: For monitoring system activity and collecting logs.
3. **MITRE ATT&CK**: To map activities for better threat intelligence.

## 📫 Contact
For more information or questions, feel free to reach out to me at:

✉️ shankarchowdary1610@gmail.com
