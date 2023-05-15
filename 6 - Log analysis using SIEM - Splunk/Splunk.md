### 1. Understand the architecture of Splunk and the installation process. Setup collector and forwarder,then ensure the logs are accumulated in Splunk. Familiarize yourself with the dashboard fields.

Splunk Architecture

- **Data collection**: Splunk can collect data from a variety of sources such as servers, network devices, applications, sensors, and more. It uses agents and connectors to collect data and send it to the Splunk server.
- **Data indexing**: The collected data is indexed and stored in Splunk's proprietary format, which is optimized for searching and querying. The indexing process involves breaking the data into events, extracting fields from the events, and creating an index for each field.
- **Search and analysis**: Splunk provides a powerful search and analysis engine that allows users to query the indexed data using a search language called SPL (Splunk Processing Language). Users can create ad-hoc searches or save them as dashboards and alerts for later use.
- **Visualization**: Splunk provides a range of visualization options such as charts, graphs, and tables to help users understand and analyze their data. Users can customize the visualization options to suit their needs.
- **Deployment options**: Splunk can be deployed on-premises, in the cloud, or as a hybrid deployment. Splunk Enterprise can be deployed as a single instance or as a distributed environment with multiple indexers, search heads, and forwarders.

#### Installing Splunk Forwarder in Kali
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/95ef383c-9a35-49c8-a2cf-91ab58c4817a)
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d59657ca-4064-4f3a-8aef-853b8d886d63)
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e4d79590-3701-4f90-98f5-0242f2c34f3b)



#### Splunk Forwarding Configuration
- First we get the Splunk Enterprise IP and port
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e79ad500-d5c7-49e7-9c0a-f7f3213f849e)

- Then give configure the splunk forwarder with the splunk enterprise
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/11add3e6-db41-49de-a650-2dc3d79a5040)
- Now go to Splunk Enterprise and under apps click manage apps
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3380ad6b-f4b2-4039-88a9-211679220813)

- If the status of Splunk Forwarder is disabled, make it enabled. Then go to Edit Properties and make visible to be 'yes'
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/83c771d2-cf4c-4134-97a6-de40290ecf10)

- Now we send a log to splunk-enterprise 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/4882d981-f5bf-4bae-8dbc-9b8fbe422778)

### 2. Run Splunk >> Forwarder can be in the same system or another system (user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise.
### • Run any network and port scanning commands from the host to the target machine. Run at least 5 to 8 commands. (If required, any tools can also be used).
### • Use the search section in Splunk to analyze the firewall logs to find the log of the above process and the exact IP from where the scan was performed. HINT: Use the “stats” command.
### • Analyze the log file and create an alert for any further similar activities.
- Now we perform a nmap-scan and save it as a log file
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8181b83e-9aa6-4085-8508-0dbd71ca461e)

- Now we send the nmap logs to the splunk-enterprise 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/0d481bc0-203e-4bbf-ae55-952cda5f9f0e)

- Now as a third person who only knows that a vulnerable scan has took place in it, we perform the command 'scan' in splunk 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/588dfe61-4bed-416b-acc2-6efc66dbc538)

- Another method of search query, if the third person knows the host name he/she can use 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ad811d16-5d2c-4313-bd46-346fb486918d)

- or If the index value is known to the person
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/07021f1d-fcc2-4823-b502-f244de93dc1e)

### 3. Run Splunk >> Forwarder can be in the same system or another system(user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise.
### • Perform any communication using unencrypted traffic.
### • Use the Splunk search section to check the firewall logs to analyzewhich application usesunencrypted data.
### • Analyze the log file and create an alert for any further similar activities.
- First we visit a http site
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fccdb215-afba-447b-94d8-e37165142deb)

- Now we add the location of the default logs of kali i.e /var/log into splunk
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1ebb39d7-02df-4b17-8ac0-e598138622c5)

- Now as a third person who only knowst that an unencrypted web traffic is being performed, we give a search of a http request in splunk 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e147093c-4e70-403e-abf3-0a270eceb71f)

- The result gives the browsed site
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6183e7ad-a7d4-4665-a45b-3b5a791fb20d)

- As we know, we perform a get request to access a website we can also give the following command
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/eaac059a-55b0-4935-a1a8-7f332a6a70fa)

- It also gives the result
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ad587ea6-25ad-4bd9-9494-f5ca82e19422)

### 4. Run Splunk >> Forwarder can be in the same system or another system (user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise. Download malware from this site https://dasmalwerk.eu/ . CAUTION: THEY ARE REAL MALWARE. USE IN AN ISOLATED ENVIRONMENT. >> Run the malware in your target system.
### • After running your malware file, either it is stopped by your antivirus or not using the search section, find the antivirus log for the past 1 hour.
### • Run different malware files again in the same target system and use the search section  to find the time range between the previous and current malware file execution. HINT: Use the “stats” command.
### • Then save that search as an alert to show a notification when the same type happens again.

### 5. Run Splunk >> Forwarder can be in the same system or another system (user’s convenience)  >>Make sure the logs are indexing in the Splunk enterprise.
### • Logout of the target system and perform multiple failed attempts. Then use the search section to filter out the failed attempt logs. Hint: Use the “stats” command.
### • Analyze the log file and create an alert for any further similar activities.

- We logout of the system and conduct multiple failed attempts.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/eaf99c8c-7fce-4502-ae43-7916a24a0469)

- Now if we go to our Splunk Enterprise and enter the host name

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/65bd9923-1ef8-447c-b77d-4bddd7501ec8)

- Now as a third person if we know only an authentication failure has happened, so the command can be
 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/be8edce5-58d4-4e4b-974b-5dc172e05221)

- or it can also be

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/c1e41184-30cb-48b1-ae06-f62b1d0fa58c)








