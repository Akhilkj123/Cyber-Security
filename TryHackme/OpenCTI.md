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
- 
