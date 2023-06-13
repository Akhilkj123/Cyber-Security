## Task-2:  What information should we collect?

#### Below is a checklist of the pertinent information an analyst (you) is to collect from the email header:

- Sender email address
- Sender IP address
- Reverse lookup of the sender IP address
- Email subject line
- Recipient email address (this information might be in the CC/BCC field)
- Reply-to email address (if any)
- Date/time

#### Below is a checklist of the artifacts an analyst (you) needs to collect from the email body:

- Any URL links (if an URL shortener service was used, then we'll need to obtain the real URL link)
- The name of the attachment
- The hash value of the attachment (hash type MD5 or SHA256, preferably the latter)

## Task-3:Email header Analysis
- Meassage Header: https://toolbox.googleapps.com/apps/messageheader/analyzeheader
- Message Header Analyzer: https://mha.azurewebsites.net/
- Mail Header Analysis:  mailheader.org
- IPinfo.io: https://ipinfo.io/
- URLScan.io: https://urlscan.io/

urlscan.io is a free service to scan and analyse websites. When a URL is submitted to urlscan.io, an automated process will browse to the URL like a regular user and record the activity that this page navigation creates. This includes the domains and IPs contacted, the resources (JavaScript, CSS, etc) requested from those domains, as well as additional information about the page itself. urlscan.io will take a screenshot of the page, record the DOM content, JavaScript global variables, cookies created by the page, and a myriad of other observations. If the site is targeting the users one of the more than 400 brands tracked by urlscan.io, it will be highlighted as potentially malicious in the scan results".

- Talos Reputation Center: https://talosintelligence.com/reputation

## Task-4: Email Body Analysis

- URL Extractor: https://www.convertcsv.com/url-extractor.html
- Talos File Reputation: https://talosintelligence.com/talos_file_reputation

The Cisco Talos Intelligence Group maintains a reputation disposition on billions of files. This reputation system is fed into the AMP, FirePower, ClamAV, and Open-Source Snort product lines. The tool below allows you to do casual lookups against the Talos File Reputation system. This system limits you to one lookup at a time, and is limited to only hash matching. This lookup does not reflect the full capabilities of the Advanced Malware Protection (AMP) system".

- VirusTotal: https://www.virustotal.com/gui/

"Analyze suspicious files and URLs to detect types of malware, automatically share them with the security community."

## Task-5: Malware Sandbox
- Any.Run: https://app.any.run/
- Hybrid Analysis: https://www.hybrid-analysis.com/
- https://www.joesecurity.org/

Joe Sandbox empowers analysts with a large spectrum of product features. Among them: Live Interaction, URL Analysis & AI based Phishing Detection, Yara and Sigma rules support, MITRE ATT&CK matrix, AI based malware detection, Mail Monitor, Threat Hunting & Intelligence, Automated User Behavior, Dynamic VBA/JS/JAR 
instrumentation, Execution Graphs, Localized Internet Anonymization and many more".

## Task-7: Phishing Case 1

a) What brand was this email tailored to impersonate?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/2448f456-13c7-49c8-b31a-1a68b16bdb81)

b) What is the From email address?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6b31ee0d-1169-4f2d-aeb1-146ad7e0b4de)

c) What is the originating IP? Defang the IP address.  

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9a4a62f2-79b4-4cc3-bf65-528efb790307)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/03de04ce-2c6e-4072-9ffa-5b347db96fed)

d) From what you can gather, what do you think will be a domain of interest? Defang the domain.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/2217c8a0-7930-46c8-aca1-a27bed6e70bc)

e) What is the shortened URL? Defang the URL.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f9baa48c-92ba-42d0-9074-3e57d1912a4d)

## Task-8: Phishing Case 2

a) What does AnyRun classify this email as?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b586c49c-4719-45a2-874f-d63c65e86845)

b) What is the name of the PDF file?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/dfb6badc-8e67-44cc-8e40-05aa52396934)

c) What is the SHA 256 hash for the PDF file?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d011fec7-7011-4dbb-961e-ab674b5c20fd)

d) What two IP addresses are classified as malicious? Defang the IP addresses. (answer: IP_ADDR,IP_ADDR)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ff4fa4f7-f856-466a-9b0a-b8d132fe15b6)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ff21c849-f5ba-4f8c-a990-048089858036)

e) What Windows process was flagged as Potentially Bad Traffic?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1f002ee0-0245-49f3-9a95-01b7c2d3bdbc)


## Task-9: Phishing Case 3

a) What is this analysis classified as?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/5f03d1a7-72b6-4a36-a659-dc487b506178)

b) What is the name of the Excel file?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/43123b60-5b0a-4e80-ae48-013fa5e349c3)

c) What is the SHA 256 hash for the file?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f80749c0-1a14-4dcf-8c50-30c4e2265108)

d) What domains are listed as malicious? Defang the URLs & submit answers in alphabetical order.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/fa416831-e50b-4e01-86ce-e2bc785ac5b4)

e) What IP addresses are listed as malicious? Defang the IP addresses & submit answers from lowest to highest.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/51ce79a5-866c-4461-908f-267589bd0f31)

f) What vulnerability does this malicious attachment attempt to exploit?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8c1ff619-17fd-4c8b-bf52-e70e865066ea)


