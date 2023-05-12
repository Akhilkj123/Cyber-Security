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

- Now as a third person, if we search any scans in splunk we get
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/588dfe61-4bed-416b-acc2-6efc66dbc538)

- Another method of search query if the third person knows the host name he/she can use 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ad811d16-5d2c-4313-bd46-346fb486918d)

- or If the index value is known to the person
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/07021f1d-fcc2-4823-b502-f244de93dc1e)

### 3. Run Splunk >> Forwarder can be in the same system or another system(user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise.
### • Perform any communication using unencrypted traffic.
### • Use the Splunk search section to check the firewall logs to analyzewhich application usesunencrypted data.
### • Analyze the log file and create an alert for any further similar activities.







