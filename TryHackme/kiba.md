## Task 1
- First we login to the kibana siote using the giiven machine_ip and the kibana assigned port 5601

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f8bfa1bb-3b8c-410d-af5c-2eb3f08a370f)


a) What is the vulnerability that is specific to programming languages with prototype-based inheritance?

- Prototype pollution

b) What is the version of visualization dashboard installed in the server?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d752d8a2-3c6d-4111-8629-bd2e395679e5)

c) What is the CVE number for this vulnerability? This will be in the format: CVE-0000-0000

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/dd0604d5-b3ee-4d0f-845d-0e1e9347904b)

- First we perform the nmap scan to check the details of the open port 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e51fc717-2c26-4a6c-844b-42d1544db5cd)

- Now we are about to compromise the machine. So, we download a python file from a github page to compromise the machine.
- We give the command to run the python file along with URL of the kibana page, a port( which we set as reverse shell port)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/212a8959-4bbe-4727-b877-c378b41c9a99)

- Now we will listen to the port which obtains us the kiba user page.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/20ceac78-efe8-4f3a-9b49-a4abd712d2a5)

d) Compromise the machine and locate user.txt

- Now we cat the filename to get the result

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/269de452-691b-4158-9ede-6996d8acf238)

e) How would you recursively list all of these capabilities?

- The getcap command is used to display the capabilities of files on a Linux system by checking the file's capability bit-mask

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/53a4cbfc-6426-4a4a-b61d-d09b70d7fe00)

- Now we transfer all the errors '2' to /dev/null folder, where the output shows only correct outputs

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/c44e9d9a-85f6-4192-8511-d26d87192523)

- Now using the given command below which first imports the os libraries, and we set the setuid as 0, and run the shell file

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d5c30238-0019-442a-a78c-7ec33943615b)

- Now we get into the kiba as root user.

e) Escalate privileges and obtain root.txt

- Now if we list in the root user we cat the root.txt file, we get the result.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d2138044-1972-4529-8516-c99c4cc5595b)



