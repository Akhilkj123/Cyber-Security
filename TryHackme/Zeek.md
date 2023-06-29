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

## Task 4: CLI Kung-Fu Recall: Processing Zeek Logs
- Graphical User Interfaces (GUI) are handy and good for accomplishing tasks and processing information quickly.
- There are multiple advantages of GUIs, especially when processing the information visually.
### Use cases and their descriptions
- **sort | uniq** - Remove duplicate values.
- **sort | uniq -c** - Remove duplicates and count the number of occurrences for each value.
- **sort -nr**- Sort values numerically and recursively.
- **rev** - Reverse string characters.
- **cut -d '.' -f 1-2** - Split the string on every dot and print keep the first two fields.
- **grep -v -e 'test1' -e 'test2'** - Display lines that don't match one or both "test1" and "test2" strings.
- **file** - View file information.
- **grep -rin Testvalue1 * | column -t | less -S** - Search the "Testvalue1" string everywhere, organise column spaces and view the output with less.

## Task 5: Zeek Signatures
- Zeek supports signatures to have rules and event correlations to find noteworthy activities on the network.
- Zeek signatures use low-level pattern matching and cover conditions similar to Snort rules.

Zeek signatures use the ".sig" extension.
- -C: Ignore checksum errors.
- -r: Read pcap file.
- -s: Use signature file. 

a) Investigate the http.pcap file. Create the  HTTP signature shown in the task and investigate the pcap. What is the source IP of the first event?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9b1ff610-e0bf-4eab-9835-9bf9fcd39814)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/bf901047-78f3-4c86-af6d-589c0418750c)

b) What is the source port of the second event?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/38930742-8060-4f8f-b5bf-83f5a5cad2f5)

c) What is the total number of the sent and received packets from source port 38706?
- 20

Create the global rule shown in the task and investigate the ftp.pcap file.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/5004d076-b5a7-4fa2-a2ce-a814c20c5f00)

d) Investigate the notice.log. What is the number of unique events

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/151cab56-dadc-4a80-807f-a95d9e194441)

e) What is the number of ftp-brute signature matches?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6f808d32-a747-4f89-aefe-a643eb362c48)

## Task 6: Zeek Scripts | Fundamentals
- Zeek has its own event-driven scripting language, which is as powerful as high-level languages and allows us to investigate and correlate the detected events.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/4fc90b8e-cf9a-4977-b07c-603d1a05ec08)

a) Investigate the smallFlows.pcap file. Investigate the dhcp.log file. What is the domain value of the "vinlap01" host?
  
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/4a99d12c-d18c-4b9c-b011-ecdc1667c841)

b) Investigate the bigFlows.pcap file. Investigate the dhcp.log file. What is the number of identified unique hostnames?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e78bf5cc-8c8c-48e1-8723-85ae991ad1ac)

c) Investigate the bigFlows.pcap file. Investigate the dhcp.log file. What is the number of identified unique hostnames?
- 17

d) Investigate the dhcp.log file. What is the identified domain value?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d6894bf7-5a07-4451-b208-1ed95f5193a0)

e) Investigate the dns.log file. What is the number of unique queries?
- 1109

## 
