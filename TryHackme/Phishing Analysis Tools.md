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





