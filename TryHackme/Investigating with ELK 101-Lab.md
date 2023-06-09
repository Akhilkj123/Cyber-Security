## Task - 3 ElasticStack Overview

- collection of different open source components linked together to help users take the data from any source and in any format and perform a search, analyze and visualize the data at real-time.

### Elasticsearch 
- full-text search and analytics engine used to store JSON-formated documents. 
- important component used to store, analyze, perform correlation on the data, etc.

### Logstash
- data processing engine used to take the data from different sources, apply the filter on it or normalize it, and then send it to the destination.
- **input part** is where the user defines the source from which the data is being ingested. 
- **filter part** is where the user specifies the filter options to normalize the log ingested above.
- **output part** is where the user wants the filtered data to send.

### Kibana
- web-based data visualization that works with elasticsearch to analyze, investigate and visualize the data stream in real-time.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8f990adc-170a-4a5d-8a37-8dfe29d681b3)

a) Logstash is used to visualize the data. (yay / nay)
- nay

b) Elasticstash supports all data formats apart from JSON. (yay / nay)
- nay

## Task - 5 Discover tab

- First we get into the website of elastic search using the ip provided

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/11e66be9-3a16-4ea1-9bb0-5a02144aa23d)

- Now we login the wesbsite using the given credentials

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/0c6e365d-784d-4160-af08-fad23720b219)

- Now we are into the account which has the files for analysis and lets answer the questions

a) Select the index vpn_connections and filter from 31st December 2021 to 2nd Feb 2022. How many hits are returned? 
- We first selected the filter vpn_connections and then set the time range from 31st December 2021 to 2nd Feb 2022. So it returned a value of '2861 hits'
  ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f1e8e64e-9012-45af-9095-9e9d7b532ad1)

b) Which IP address has the max number of connections?
- When we get into the filters, we see a Source_ip filter present. When we open it we see an ip with maximum number of connection.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b48d3890-01a7-41b5-86c7-f42c1ac88fcb)

c) Which user is responsible for max traffic?
- Similarly if we select the filter 'Username' we get the user responsible for maximum traffic.
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/120fd16f-268d-464b-93f3-68ab94918ba8)

e) Apply Filter on UserName Emanda; which SourceIP has max hits?
- When we filter on UserName Emanda, we get the sourceIp used maximum is,
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8f68a2a4-10f8-437a-a58e-0ffd4e12d6ad)

f) On 11th Jan, which IP caused the spike observed in the time chart?
- Now we filter the date to be 11th Jan and select the filter type as Source_ip and observe who has used the maximum traffic.
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/39d0dad9-dc7f-4538-b7a2-3b9e491c5c0f)

g) How many connections were observed from IP 238.163.231.224, excluding the New York state?

- When we give a filter of 238.163.231.224 in Source_ip, we get

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6bfbd15d-cb27-4744-a26a-74b993bce4cd)

- Now we give with filter 'New York'

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9bc084ff-a6e5-4f13-a612-f0abca34e6a5)
- So we do the calculation of Total - Newyork(hits)

- 96 - 48 = 48

## Task - 6 KQL Overview

## KQL(Kibana Query Language)
- search query language used to search the ingested logs/documents in the elasticsearch.

With KQL, we can search for the logs in two different ways.

### a) Free text Search
- allows users to search for the logs based on the text-only.

####  i)Wild Card
- KQL allows the wild card * to match parts of the term/word.

#### ii) Logical Operators (AND | OR | NOT)
 - 1- OR Operator
- 2- AND Operator
- 3- NOT Operator

### b) Field-based search

- we will provide the field name and the value we are looking for in the logs. 


a) Create a search query to filter out the logs from Source_Country as the United States and show logs from User James or Albert. How many records were returned?
- The search query to filter the souce_country, username includes the following

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/113d1d6a-315b-44f0-9515-f87f097d6971)
- When we select these filters we get output as
- 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/354d7027-885e-41e2-98d5-d98fc1816677)

b) As User Johny Brown was terminated on 1st January 2022, create a search query to determine how many times a VPN connection was observed after his termination.
- In this we give the username filter as johny brown and the time to be from 1st January 2022

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/507ab27b-12c5-42ce-ad2b-3e02a9f1a223)
- This gives the result

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fc480bce-b6f5-45b0-b257-d4a29b91f046)

## Task - 7 Create Visualizations

a) Which user was observed with the greatest number of failed attempts? 
- In the filter search field, we give a filter action whose value is to be 'failed'

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/0fcf70ce-806e-47ed-acd9-4c83119b2e70)
- Now we go the filter by type and set it as Username to get the result 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/db89bb5c-1f8c-4bf3-bedc-d63a8e4fb8da)

b) How many wrong VPN connection attempts were observed in January?
- In this we proceed with the filter action with a value true and set the time from Jan 1st to Jan 31st which the number of hits.
 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b96526da-56e3-4475-b874-c82cf886bed2)

## Task - 8 Creating Dashboards
a) Create the dashboard containing the available visualizations.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1040aa66-b6ed-43e8-9d78-85cf85204bcc)











