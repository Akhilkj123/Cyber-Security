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

### Task 5


Investigate the traffic with the default configuration file with ASCII mode.

sudo snort -dev -K ASCII -l .

Execute the traffic generator script and choose "TASK-6 Exercise". Wait until the traffic ends, then stop the Snort instance. Now analyse the output summary and answer the question.

sudo ./traffic-generator.sh
