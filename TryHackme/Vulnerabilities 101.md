## Task 2: Introduction to Vulnerabilities

- A vulnerability in cybersecurity is defined as a weakness or flaw in the design, implementation or behaviours of a system or application.

  ### Five main categories of vulnerabilities:
  - **Operating System** - These types of vulnerabilities are found within Operating Systems (OSs) and often result in privilege escalation.
  - **Configuration-based** - These types of vulnerability stem from an incorrectly configured application or service.
  - **Weak or Default Credentials** - Applications and services that have an element of authentication will come with default credentials when installed.
  - **Application Logic** - These vulnerabilities are a result of poorly designed applications.
  - **Human-Factor** - Human-Factor vulnerabilities are vulnerabilities that leverage human behaviour.
 
a) An attacker has been able to upgrade the permissions of their system account from "user" to "administrator". What type of vulnerability is this?
- operating system
 
b) You manage to bypass a login panel using cookies to authenticate. What type of vulnerability is this?
- application logic

  
## Task 3: Scoring Vulnerabilities (CVSS & VPR)
- Vulnerability management is the process of evaluating, categorising and ultimately remediating threats (vulnerabilities) faced by an organisation.

### Common Vulnerability Scoring System
- It awards points to a vulnerability based upon its features, availability, and reproducibility.
- A vulnerability is given a classification (out of five) depending on the score that is has been assigned. 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ba53fe70-4b24-44fc-88da-f330cbe0c0e1)

### Vulnerability Priority Rating (VPR)
- This framework is considered to be risk-driven; meaning that vulnerabilities are given a score with a heavy focus on the risk a vulnerability poses to the organisation itself, rather than factors such as impact (like with CVSS).
- VPR does not have a "None/Informational" category, and because VPR uses a different scoring method, the same vulnerability will have a different score using VPR than when using CVSS.

 ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e9656608-8402-4f74-8cc0-84b04cedd47c)

a) What year was the first iteration of CVSS published?
- 2005

b) If you wanted to assess vulnerability based on the risk it poses to an organisation, what framework would you use?
- VPR

c) If you wanted to use a framework that was free and open-source, what framework would that be?
- CVSS

## Task 4: Vulnerability Databases
### Fundamental key terms in vulnerability 
- **Vulnerability** - A vulnerability is defined as a weakness or flaw in the design, implementation or behaviours of a system or application.
- **Exploit** - An exploit is something such as an action or behaviour that utilises a vulnerability on a system or application.
- **Proof of Concept (PoC)** - A PoC is a technique or tool that often demonstrates the exploitation of a vulnerability.

### NVD – National Vulnerability Database
- The National Vulnerability Database is a website that lists all publically categorised vulnerabilities.
-  In cybersecurity, vulnerabilities are classified under “Common Vulnerabilities and Exposures” (Or CVE for short).
- These CVEs have the formatting of CVE-YEAR-IDNUMBER. For example, the vulnerability that the famous malware WannaCry used was CVE-2017-0144.

- ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/61354529-2e0a-4ffe-bc6b-d825688ecdf2)

### Exploit-DB
- Exploit-DB retains exploits for software and applications stored under the name, author and version of the software or application.
- We can use Exploit-DB to look for snippets of code (known as Proof of Concepts) that are used to exploit a specific vulnerability.

  
