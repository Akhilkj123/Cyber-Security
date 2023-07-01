## Task 2: Introduction
- It is a scalable, open-source and freely available Security Incident Response Platform, designed to assist security analysts and practitioners working in SOCs, CSIRTs and CERTs to track, investigate and act upon identified security incidents in a swift and collaborative manner.
 ### TheHive Project operates under the guide of three core functions:

- **Collaborate:** Multiple analysts from one organisation can work together on the same case simultaneously. Through its live stream capabilities, everyone can keep an eye on the cases in real time.
- **Elaborate:** Investigations correspond to cases. The details of each case can be broken down into associated tasks, which can be created from scratch or through a template engine. Additionally, analysts can record their progress, attach artifacts of evidence and assign tasks effortlessly.
- **Act:** A quick triaging process can be supported by allowing analysts to add observables to their cases, leveraging tags, flagging IOCs and identifying previously seen observables to feed their threat intelligence.

## Task 3: TheHive Features & Integrations
### The features include:

- **Case/Task Management:** Every investigation is meant to correspond to a case that has been created. Each case can be broken down into one or more tasks for added granularity and even be turned into templates for easier management. 

- **Alert Triage:** This feature allows an analyst to go through the imported alerts and decide whether or not they are to be escalated into investigations or incident response.

- **Observable Enrichment with Cortex:** One of the main feature integrations TheHive supports is Cortex, an observable analysis and active response engine. Cortex allows analysts to collect more information from threat indicators by performing correlation analysis and developing patterns from the cases. More information on Cortex.

- **Active Response:** TheHive allows analysts to use Responders and run active actions to communicate, share information about incidents and prevent or contain a threat.

- **Custom Dashboards:** Statistics on cases, tasks, observables, metrics and more can be compiled and distributed on dashboards that can be used to generate useful KPIs within an organisation.

- **Built-in MISP Integration:** Another useful integration is with MISP, a threat intelligence platform for sharing, storing and correlating Indicators of Compromise of targeted attacks and other threats. This integration allows analysts to create cases from MISP events, import IOCs or export their own identified indicators to their MISP communities.

a) Which open-source platform supports the analysis of observables within TheHive?
- Cortex

## Task 4: User Profiles & Permissions
### The pre-configured user profiles are:

- **admin:** full administrative permissions on the platform; can't manage any Cases or other data related to investigations;
- **org-admin:** manage users and all organisation-level configuration, can create and edit Cases, Tasks, Observables and run Analysers and Responders;
- **analyst:** can create and edit Cases, Tasks, Observables and run Analysers & Responders;
- **read-only:** Can only read, Cases, Tasks and Observables details;

a) Which pre-configured account cannot manage any cases?
- admin

b) Which permission allows a user to create, update or delete observables?
- manageObservables

c) Which permission allows a user to execute actions?
- manageActions

- Logged into Thehive using the given credentials

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/038bb61c-0dfb-472f-97a4-b5f6560f0d2d)

## Task 5: Analyst Interface Navigation
### The following options must be indicated on the case to set different categories and filter options:

- **Severity:** This showcases the level of impact the incident being investigated has on the environment from low to critical levels.
- **TLP:** The Traffic Light Protocol is a set of designations to ensure that sensitive information is shared with the appropriate audience. The range of colours represents a scale between full disclosure of information (White) and No disclosure/ Restricted (Red). You can find more information about the definitions on the CISA website.
- **PAP:**  The Permissible Actions Protocol is used to indicate what an analyst can do with the information, whether an attacker can detect the current analysis state or defensive actions in place. It uses a colour scheme similar to TLP and is part of the MISP taxonomies.

- Now we create a new task

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/01c6b4fb-14f8-4e30-8d69-05355cf86f88)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b66905c3-8ac4-4fe5-873f-f7b3a027fd45)

- Now we add new observables in it

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/5bc77cd6-728c-4f2e-b5ad-1e647af3632b)

a) Where are the TTPs imported from?
- MITRE ATT&CK Framework

b) According to the Framework, what type of Detection "Data source" would our investigation be classified under?
- Network Traffic

c) Upload the pcap file as an observable. What is the flag obtained from https://10.10.117.56//files/flag.html

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/83f507b5-1949-4447-97f0-c0c0bfb4eadd)

