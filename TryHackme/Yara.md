## Task 2: What is Yara?
- Yara rules are frequently written to determine if a file is malicious or not, based upon the features - or patterns - it presents.

a) What is the name of the base-16 numbering system that Yara can detect?
- hexadecimal

b) Would the text "Enter your Name" be a string in an application?
- Yay

## Task 3: Deploy
- Logging in to the machine using provided credentials

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e902049d-729b-4404-96f6-49138cd310af)

## Task 4: Introduction to Yara Rules
- First we create two files

  i) some text file
  ii) file with yara rules

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6944f40e-69e6-4868-8554-0e06ae6aa69e)

## Task 5: Expanding on Yara Rules
### Yara has a few conditions as given below:
- **Meta** - This section of a Yara rule is reserved for descriptive information by the author of the rule.
- **Strings** - Strings can be used to search for specific text or hexadecimal in files or programs.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6eb533bf-5365-496e-9129-4b95d84be959)

- **Conditions** - Multiple strings can be searched by giving the condition

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/28401998-1b30-4347-bb38-6eac28bafb40)

 Much like regular programming, you can use operators such as:

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b06541ee-bdec-4455-a48f-e66c1606bc19)

## Task 6: Yara Modules
### Cuckoo
- Cuckoo Sandbox is an automated malware analysis environment.
- This module allows you to generate Yara rules based upon the behaviours discovered from Cuckoo Sandbox.

### Python PE
- Python's PE module allows you to create Yara rules from the various sections and elements of the Windows Portable Executable (PE) structure.

## Task 7: Other tools and Yara
### LOKI
- It is a free open-source IOC (Indicator of Compromise) scanner.

Detection is based on 4 methods:
- File Name IOC Check
- Yara Rule Check (we are here)
- Hash Check
- C2 Back Connect Check

### THOR
- THOR Lite is Florian's newest multi-platform IOC AND YARA scanner.

### FENRIR
- Fenrir is a bash script; it will run on any system capable of running bash

### YAYA
- YAYA is a new open-source tool to help researchers manage multiple YARA rule repositories.
- YAYA starts by importing a set of high-quality YARA rules and then lets researchers add their own rules, disable specific rulesets, and run scans of files.

## Task 8: Using LOKI and its Yara rule set

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/a8210830-6190-4da7-be86-38e5e4ffdbb7)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/63ea38c6-3aee-4d75-a4bd-185e6e22a6e5)

a) Does Loki detect this file as suspicious/malicious or benign?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fce66bd9-d09a-4068-8a5b-62472d285909)

b) What Yara rule did it match on?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b1e07312-4f5d-469a-ac93-2f65f02aedbf)

c) What does Loki classify this file as?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fc8d09ac-3896-489d-b6dd-f0008b186927)

d) Based on the output, what string within the Yara rule did it match on?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9ce4a9a6-239e-4b04-8cbf-a0eb5cb30f4e)

e) What is the name and version of this hack tool?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/29844c0c-84f3-4bda-8b2c-7ea1aae5f136)

f) Inspect the actual Yara file that flagged file 1. Within this rule, how many strings are there to flag this file?


g) Does Loki detect this file as suspicious/malicious or benign?
- benign

h) What is the name and version of this web shell?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/5743764a-67ea-4447-bca3-15d7f0ba576f)


## Task 9: Creating Yara rules with yarGen

- We are going to update yarGen, you'll see the following message at the end of the output.
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8dd7bc51-6881-467a-bf38-b47af69d30cb)

a) From within the root of the suspicious files directory, what command would you run to test Yara and your Yara rule against file 2?
- yara 1ndex.php file2/file2.yar

b) Did Yara rule flag file 2? (Yay/Nay)
- yay
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ccd2833b-abdd-4fc7-869b-f8155e8d490c)

c) Test the Yara rule with Loki, does it flag file 2?
- yay

d) What is the name of the variable for the string that it matched on?
- zepto


## Task 10: Valhalla
- Valhalla is an online Yara feed created and hosted by Nextron-Systems.
- Now take the sha256 of the file and enter it in Valhalla

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/5258c050-654c-473e-ac2d-70649d6a298a)

a)  What is the name of the first Yara rule to detect file 2?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ecf5a6f9-58e4-460f-a836-21c17c2aba7f)

b) Examine the information for file 2 from Virus Total (VT). The Yara Signature Match is from what scanner?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f7c00239-bdfb-419e-871e-38272bdb5414)

c) Enter the SHA256 hash of file 2 into Virus Total. Did every AV detect this as malicious?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/178dff32-bd08-4569-b633-e9fda78ee03a)

d) Enter the SHA256 hash of file 2 into Virus Total. Did every AV detect this as malicious?
- nay

e) Besides .PHP, what other extension is recorded for this file?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d802c872-130d-4f8d-8fcf-911ccb3c41f8)

f) What JavaScript library is used by file 2?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/47754c76-96b4-4db5-aa7e-8aea6e9ab306)

g) Is this Yara rule in the default Yara file Loki uses to detect these type of hack tools? 
- nay


