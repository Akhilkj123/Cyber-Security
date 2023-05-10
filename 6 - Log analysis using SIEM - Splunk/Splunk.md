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
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9c7db8c2-0732-4a5e-bb35-289bef547ae6)

- Now go to Splunk Enterprise and under apps click manage apps
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3380ad6b-f4b2-4039-88a9-211679220813)

- If the status of Splunk Forwarder is disabled, make it enabled. Then go to Edit Properties and make visible to be 'yes'
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/83c771d2-cf4c-4134-97a6-de40290ecf10)


