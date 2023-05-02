#### 1. Understand the architecture of Splunk and the installation process. Setup collector and forwarder,then ensure the logs are accumulated in Splunk. Familiarize yourself with the dashboard fields.

Splunk Architecture

- **Data collection**: Splunk can collect data from a variety of sources such as servers, network devices, applications, sensors, and more. It uses agents and connectors to collect data and send it to the Splunk server.
- **Data indexing**: The collected data is indexed and stored in Splunk's proprietary format, which is optimized for searching and querying. The indexing process involves breaking the data into events, extracting fields from the events, and creating an index for each field.
- **Search and analysis**: Splunk provides a powerful search and analysis engine that allows users to query the indexed data using a search language called SPL (Splunk Processing Language). Users can create ad-hoc searches or save them as dashboards and alerts for later use.
- **Visualization**: Splunk provides a range of visualization options such as charts, graphs, and tables to help users understand and analyze their data. Users can customize the visualization options to suit their needs.
- **Deployment options**: Splunk can be deployed on-premises, in the cloud, or as a hybrid deployment. Splunk Enterprise can be deployed as a single instance or as a distributed environment with multiple indexers, search heads, and forwarders.
