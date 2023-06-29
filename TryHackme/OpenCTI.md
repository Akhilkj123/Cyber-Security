## Task 2: Introduction to OpenCTI
### OpenCTI
- OpenCTI is another open-sourced platform designed to provide organisations with the means to manage CTI through the storage, analysis, visualisation and presentation of threat campaigns, malware and IOCs.

## Task 3: OpenCTI Data Model
- OpenCTI uses a variety of knowledge schemas in structuring data, the main one being the Structured Threat Information Expression (STIX2) standards. STIX is a serialised and standardised language format used in threat intelligence exchange.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/cef84cc0-e544-4049-9f3b-7fec969eb756)

The highlight services include:

- **GraphQL API:** The API connects clients to the database and the messaging system.
- **Write workers:** Python processes utilised to write queries asynchronously from the RabbitMQ messaging system.
- **Connectors:** Another set of Python processes used to ingest, enrich or export data on the platform. These connectors provide the application with a robust network of integrated systems and frameworks to create threat intelligence relations and allow users to improve their defence tactics.

## Task 4: OpenCTI Dashboard 1
- First we login to the opencti platform with the given credentials

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1c1e77b8-fc72-40ab-99ad-0942195637ab)

### OpenCTI Dashboard
- Once connected to the platform, the opening dashboard showcases various visual widgets summarising the threat data ingested into OpenCTI.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/e13dbf26-d891-4559-8bc5-6d4f991824a5)

### Analysis
- The Analysis tab contains the input entities in reports analysed and associated external references. Reports are central to OpenCTI as knowledge on threats and events are extracted and processed.


 ### Events
 - Security analysts investigate and hunt for events involving suspicious and malicious activities across their organisational network.


### Observations
- Technical elements, detection rules and artefacts identified during a cyber attack are listed under this tab: one or several identifiable makeup indicators.

### Threats
All information classified as threatening to an organisation or information would be classified under threats.
- **Threat Actors:** An individual or group of attackers seeking to propagate malicious actions against a target.
- **Intrusion Sets:** An array of TTPs, tools, malware and infrastructure used by a threat actor against targets who share some attributes.
- **Campaigns:** Series of attacks taking place within a given period and against specific victims initiated by advanced persistent threat actors who employ various TTPs.

### Arsenal
- **Malware:** Known and active malware and trojan are listed with details of their identification and mapping based on the knowledge ingested into the platform.
- **Attack Patterns:** Adversaries implement and use different TTPs to target, compromise, and achieve their objectives.
- **Courses of Action:** MITRE maps out concepts and technologies that can be used to prevent an attack technique from being employed successfully

a) What is the name of the group that uses the 4H RAT malware?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/d3cc159a-817b-4e23-a0a6-70a10bc816e3)

b) What kill-chain phase is linked with the Command-Line Interface Attack Pattern? 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/c899644a-2a42-4b1b-b1a0-62c49d6b2c58)

c) Within the Activities category, which tab would house the Indicators?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/2b40e8b4-1edf-4409-984d-1b6265e98c86)

## Task 5: OpenCTI Dashboard 2
- **Overview Tab:** Provides the general information about an entity being analysed and investigated.
- **Knowledge Tab:** Presents linked information associated with the entity selected.
- **Analysis Tab:** Provides the reports where the identified entry has been seen.
- **Indicators Tab:** Provides inf)mation on IOC identified for all the threats and entities.
- **Data Tab:** Contains the files uploaded or generated for export that are related to the entity

a) What Intrusion sets are associated with the Cobalt Strike malware with a Good confidence level? (Intrusion1, Intrusion2)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3afe0692-606d-45c2-aea3-1f93c0a520f3)

b) Who is the author of the entity?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/bf906db6-c813-4f8f-bc2a-6bd59ef9b60b)

## Task 6: Investigative Scenario

a) What is the earliest date recorded related to CaddyWiper?  Format: YYYY/MM/DD

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9849ee93-fa7f-493d-8e00-944521d74d43)

b) Which Attack technique is used by the malware for execution?
- Under Arsenal tab Attack Patterns gives the result

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/dacefe8b-0aff-448a-a519-b218649c6f48)

c) How many malware relations are linked to this Attack technique?
- now filter the Native API and under the knowledge tab

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/bd0207d5-2277-4f48-b5c0-5b8010e1b2cb)

d) Which 3 tools were used by the Attack Technique in 2016? (Ans: Tool1, Tool2, Tool3)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/37fdb61f-c256-4dc6-8077-7bd52fc6364a)

e) What country is APT37 associated with?
- Search APT37 and go to the intrsuion sets, under the overview result is present.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6febd896-83f3-4e22-9094-73365feaff0d)

f) Which Attack techniques are used by the group for initial access? (Ans: Technique1, Technique2)
 - Under the Global Kill chain in the Knowledge tab the result shows.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/505fda88-ebdd-467d-9541-58e12dc94d72)



