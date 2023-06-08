
## Task - 2: Main Components of Metasploit 

### Auxiliary
- Any supporting module, such as scanners, crawlers and fuzzers, can be found in auxiliary.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/076d5729-09f6-492d-8114-3d6ce406d393)

### Encoders
- Encoders will allow you to encode the exploit and payload in the hope that a signature-based antivirus solution may miss them.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8b112e59-9fc3-40f8-bbe8-8b92c0bfb1f6)

### Evasion
- While encoders will encode the payload, they should not be considered a direct attempt to evade antivirus software. 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/383cfa65-c4f9-4e09-8d19-68bd859aa973)

### Exploits
- Exploits, neatly organized by target system.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ba6455f2-1e32-4d36-bfb0-582a805acc78)

### NOPs(No Operation)
- They are represented in the Intel x86 CPU family they are represented with 0x90, following which the CPU will do nothing for one cycle.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fd56e460-5791-4e92-bf20-4664725d5bd4)

### Payloads
- Exploits will leverage a vulnerability on the target system, but to achieve the desired result, we will need a payload. 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f8aa3e28-6f2e-4f53-84d1-76affa1c5bec)

- **Adapters:** An adapter wraps single payloads to convert them into different formats. For example, a normal single payload can be wrapped inside a Powershell adapter, which will make a single powershell command that will execute the payload.
- **Singles:** Self-contained payloads (add user, launch notepad.exe, etc.) that do not need to download an additional component to run.
- **Stagers:** Responsible for setting up a connection channel between Metasploit and the target system. Useful when working with staged payloads. “Staged payloads” will first upload a stager on the target system then download the rest of the payload (stage). 
- **Stages:** Downloaded by the stager. This will allow you to use larger sized payloads.

### Post
- Post modules will be useful on the final stage of the penetration testing process listed above, post-exploitation.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/eae96a70-aa9d-40e7-88d7-9c4887b0fa6c)


a) What is the name of the code taking advantage of a flaw on the target system?
- exploit

b) What is the name of the code that runs on the target system to achieve the attacker's goal?
 - Payload

c) What are self-contained payloads called?
- singles

d) Is "windows/x64/pingback_reverse_tcp" among singles or staged payload?
- singles

## Task - 3: Msfconsole

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/0071b6ef-63ae-422d-b35c-60e83174f2c9)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/151a9ccd-15a4-4390-97a3-8f9cdc2861c9)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/bc078d5b-0143-4ac2-9950-e66cacbbbe56)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8dd77d41-e492-4a4e-8ec6-a4b5d2e2edeb)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/92879e7b-be98-4793-bb51-19918fb683e2)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f07a2961-e486-45d7-beb3-e16ab2134db9)

a) How would you search for a module related to Apache? 
- search apache

b) Who provided the auxiliary/scanner/ssh/ssh_login module?
- ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9e2a039b-1b37-4ea8-b7f1-4ef2d96b00ad)

## Task - 4: Working with modules
- We can set a host and exploit by using

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/596b2bc5-17b8-444c-8b8b-a9fff574f17c)


a) How would you set the LPORT value to 6666?

 ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/725caf3c-cb3f-4166-8dcb-18dad4a27ccc)

b) How would you set the global value for RHOSTS  to 10.10.19.23 ?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3715491b-acef-4af8-bc16-c48d8a6b09a6)

c) What command would you use to clear a set payload?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6c9f1b98-66af-4499-886b-f546372ab495)

d) What command do you use to proceed with the exploitation phase?
- exploit

