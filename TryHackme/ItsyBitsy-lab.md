## Task - 2  Scenario - Investigate a potential C2 communication alert 

- First of all, we go to the site using the machine_ip provided. 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/607bc96b-dd80-4244-ba8d-0ca46b8ebda7)

- Now we login to the site using the given credentials and we start answering the questions

a) How many events were returned for the month of March 2022?
- Here, we filter date from March 1,2022 to March 31,2022 to get the number of hits
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e7ccd7bd-c0a8-4bf7-a1b1-a05ed2783062)

b) What is the IP associated with the suspected user in the logs?
- Here ,first we go to the filtertype useragent, and we select the bitsadmin filter which is a suspicious useragent. When we select the agent we get the IP associated to it as 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ddaa87f8-dac5-46f6-983d-6f7e5ce7d3aa)

c) The user’s machine used a legit windows binary to download a file from the C2 server. What is the name of the binary?
- The answer to this question is the user agent which we acquired in question 2

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/321e81df-8c2f-4b43-9634-7af182aeb11b)

d) The infected machine connected with a famous filesharing site in this period, which also acts as a C2 server used by the malware authors to communicate. What is the name of the filesharing site?
- When we check the bitsadmin hits, we get the website to be

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f9453a8b-c0d7-46aa-bd04-74408098bd87)

e) What is the full URL of the C2 to which the infected host is connected?
- The full URL of the site to which the infected host is connected is as given pastebin.com/yTg0Ah6a

f) A file was accessed on the filesharing site. What is the name of the file accessed?
- Now we go the URL given and we get the file which was accessed by the infected host

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/cd9de660-e492-4268-bf9c-788480ebffff)

g) The file contains a secret code with the format THM{_____}.
- The page also contains the secret code in it.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/791f9f13-36d7-4bcb-b2f3-18eff76d5333)










