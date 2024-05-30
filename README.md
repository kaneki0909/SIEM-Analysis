# Practical Insights into Azure Sentinel(SOC) and Honeypot/Honeynet Implementation 

This project is about mapping failed brute-force RDP logins worldwide, showing where cyber attackers are based and the intensity of their attacks. We set up a Windows 10 Virtual Machine on Microsoft Azure, opened its ports to attract attackers, and used Azure Sentinel SIEM to analyze logs. These logs include data like attacker and victim IPs, which we extracted and enriched with geolocation info using a custom Powershell script. 

Using a world map visualization in Azure, we displayed attempted RDP logins along with attackers' locations and attack intensities over several days. We then analyzed this data as a group to discuss and document defense strategies against such attacks.

- Setups/Walkthrough 
  - [Virtual Machine Setup](https://github.com/kaneki0909/SIEM-Analysis/blob/main/Virtual_Machine_Setup/Vm.md) 
  - [Log Analytics Workspace](https://github.com/kaneki0909/SIEM-Analysis/blob/main/Log_Analytics_Workspace_setup/LA.md)
  - [Sentinel Setup](https://github.com/kaneki0909/SIEM-Analysis/blob/main/Sentinel_Setup/Sen.md) 
  - [Remote Desktop and Custom Powershell Script]()
  - [Custom Log Table integration into Log Analytic Workspace]() 
- MindMap 
  - ![](img/MingMap.png)
- Key Insights 
  - 🔒 Importance of SIEM tools: SIEM tools like Azure Sentinel are crucial for cybersecurity jobs as they help monitor and analyze security events, enabling proactive threat detection and response.
  - 🖥️ Setting up a virtual machine: Creating a honeypot virtual machine allows capturing and analyzing attack data without risking the main system’s security.
  - 📊 Analyzing log data: Log analytics and Azure Sentinel provide powerful tools to extract and analyze log data, helping to identify patterns and potential threats.
  - 🌐 Understanding internet security: Monitoring failed login attempts from different countries highlights the importance of strong passwords and multi-factor authentication to protect against unauthorized access.
  - 🌍 Geographic data insights: Obtaining geographic data from IP addresses provides valuable insights into the origin and distribution of attacks, aiding in threat analysis and response.
  - 🗺️ Visualizing attacks: Visualizing attacks on a map using Azure Sentinel enhances situational awareness and helps identify regions with high threat activity.


