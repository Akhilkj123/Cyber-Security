## Task 1: Introduction
- Zeek is the world's leading platform for network security monitoring.
- It is a passive, open-source network traffic analyser.

## Task 2: Network Security Monitoring and Zeek
- **Network Monitoring** - It  is highly focused on IT assets like uptime (availability), device health and connection quality (performance), and network traffic balance and management (configuration).
- **Network Security Monitoring** - It is focused on network anomalies like rogue hosts, encrypted traffic, suspicious service and port usage, and malicious/suspicious traffic patterns in an intrusion/anomaly detection and response approach.

### Zeek Architecture
  - It has two primary layers
  - **The Event Engine layer:** It is where the packets are processed; it is called the event core and is responsible for describing the event without focusing on event details.
  - **The Policy Script Interpreter:** This layer is where the semantic analysis is conducted. It is responsible for describing the event correlations by using Zeek scripts.

### Zeek Frameworks
- It has several frameworks to provide extended functionality in the scripting layer.
- These frameworks enhance Zeek's flexibility and compatibility with other network components.

### Zeek Outputs
- It provides 50+ log files under seven different categories, which are helpful in various areas such as traffic monitoring, intrusion detection, threat hunting and web analytics.

a) Each exercise has a folder. Ensure you are in the right directory to find the pcap file and accompanying files. Desktop/Exercise-Files/TASK-2
- We need to process the pcap files with Zeek. Logs are saved in the working directory. We can view the generated logs using the ls -l command.  

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e07a88e4-9a14-4b8c-9c32-41e665c8749d)

b) What is the installed Zeek instance version number?
 
 ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/07324b05-53c6-4674-83da-b1ad59988e3b)

c) What is the version of the ZeekControl module?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9f848b6a-7de1-42a9-9482-f39bea806e9e)

d) Investigate the "sample.pcap" file. What is the number of generated alert files?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1e5ceb44-06f2-4fd8-b333-0b14514362c1)

### Task 2: Zeek Logs
- Zeek generates log files according to the traffic data.
- Zeek is capable of identifying 50+ logs and categorising them into seven categories.

- **Overall Info:** The aim is to review the overall connections, shared files, loaded scripts and indicators at once. This is the first step of the investigation.
- **Protocol Based:** Once you review the overall traffic and find suspicious indicators or want to conduct a more in-depth investigation, you focus on a specific protocol.
- **Detection:** Use the prebuild or custom scripts and signature outcomes to support your findings by having additional indicators or linked actions. 
- **Observation:** The summary of the hosts, services, software, and unexpected activity statistics will help you discover possible missing points and conclude the investigation.

- First we run the process of sample file

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f61cb5ef-7b8a-489b-b0c5-d69cace1e5b1)

a) Investigate the sample.pcap file. Investigate the dhcp.log file. What is the available hostname?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/30722661-7a91-48e1-8712-9764fe912cf2)

b) Investigate the dns.log file. What is the number of unique DNS queries?
- 2

c) Investigate the conn.log file. What is the longest connection duration?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d203aa0e-948c-4605-86c6-6679dd67b998)
