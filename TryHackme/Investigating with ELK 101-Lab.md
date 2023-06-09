## Task - 3 ElasticStack Overview

a) Logstash is used to visualize the data. (yay / nay)
- nay

b) Elasticstash supports all data formats apart from JSON. (yay / nay)
- nay

## Task - 5 Discover tab

a) Select the index vpn_connections and filter from 31st December 2021 to 2nd Feb 2022. How many hits are returned? 

  ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f1e8e64e-9012-45af-9095-9e9d7b532ad1)

b) Which IP address has the max number of connections?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b48d3890-01a7-41b5-86c7-f42c1ac88fcb)

c) Which user is responsible for max traffic?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/120fd16f-268d-464b-93f3-68ab94918ba8)

d) Create a table with the fields IP, UserName, Source_Country and save.

e) Apply Filter on UserName Emanda; which SourceIP has max hits?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8f68a2a4-10f8-437a-a58e-0ffd4e12d6ad)

f) On 11th Jan, which IP caused the spike observed in the time chart?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/39d0dad9-dc7f-4538-b7a2-3b9e491c5c0f)

g) How many connections were observed from IP 238.163.231.224, excluding the New York state?

- Now trying with filter IP 238.163.231.224

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6bfbd15d-cb27-4744-a26a-74b993bce4cd)

- Now trying with filter 'New York'

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9bc084ff-a6e5-4f13-a612-f0abca34e6a5)

- Now excluding New York
- 96 - 48 = 48

## Task - 6 KQL Overview
a) Create a search query to filter out the logs from Source_Country as the United States and show logs from User James or Albert. How many records were returned?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/354d7027-885e-41e2-98d5-d98fc1816677)

b) As User Johny Brown was terminated on 1st January 2022, create a search query to determine how many times a VPN connection was observed after his termination.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fc480bce-b6f5-45b0-b257-d4a29b91f046)

## Task - 7 Create Visualizations

a) Which user was observed with the greatest number of failed attempts? 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/db89bb5c-1f8c-4bf3-bedc-d63a8e4fb8da)

b) How many wrong VPN connection attempts were observed in January?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3a5d793a-d661-4be9-9375-a21440c52f53)

## Task - 8 Creating Dashboards
a) Create the dashboard containing the available visualizations.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1040aa66-b6ed-43e8-9d78-85cf85204bcc)










