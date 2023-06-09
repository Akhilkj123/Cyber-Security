Snort Version check

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/633690d5-2b05-4b29-bd4c-2d56acc93a98)

- Checking configuration file is valid or not

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fb5824ac-3e28-42ca-844e-35e07c43f141)

### Task 4
- Run the Snort instance and check the build number.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1187c26c-3685-49f3-b254-22fcb3ffcfa4)

- Test the current instance with "/etc/snort/snort.conf" file and check how many rules are loaded with the current build.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/aca557c0-4ce3-4be2-8bc8-5382319361c1)

- Test the current instance with "/etc/snort/snortv2.conf" file and check how many rules are loaded with the current build.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3331867f-e3d2-4d79-86a2-6d5b0fd1dcb4)

### Task-6:Operation Mode 2: Packet Logger Mode


Investigate the traffic with the default configuration file with ASCII mode.

sudo snort -dev -K ASCII -l .

Execute the traffic generator script and choose "TASK-6 Exercise". Wait until the traffic ends, then stop the Snort instance. Now analyse the output summary and answer the question.

sudo ./traffic-generator.sh

a) Now, you should have the logs in the current directory. Navigate to folder "145.254.160.237". What is the source port used to connect port 53?
- First we perform the traffic-generator and get the folders

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1083e1af-2aaa-463d-bfaf-f59fbae8c183)

- Now we get into the file and read the port

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/4e686900-6913-4fac-a847-9d1e932e3644)

b) Read the snort.log file with Snort; what is the IP ID of the 10th packet?
- Now we navigate into the 'Exercise-files' and select the 'TASK-6' file to get the snort.log.1640048004 to get the id of the 10th packet

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/03d26d17-f25c-4eef-bc26-2c43477ad084)

c) Read the "snort.log.1640048004" file with Snort; what is the referer of the 4th packet?
- When we give the command 'snort -r snort.log.1640048004 -n 4 -K' 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ea3d94b5-9a5d-49e1-a11e-cd670d624e75)

d) Read the "snort.log.1640048004" file with Snort; what is the Ack number of the 8th packet?
- Now we give the command 'snort -r snort.log.1640048004 -n 8 -K'

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/7e3ec245-3a04-4406-b3e4-2788e71b4e05)






