## Task-2: What is Sigma?
- Sigma is an open-source generic signature language developed by Florian Roth & Thomas Patzke to describe log events in a structured format. This allows for quick sharing of detection methods by security analysts.

### Sigma Use Cases
- To make detection methods and signatures shareable alongside IOCs and Yara rules.
- To write SIEM searches that avoid vendor lock-in.
- To share signatures with threat intelligence communities.
- To write custom detection rules for malicious behaviour based on specific conditions.

### Sigma Development Process
- Sigma Rule Format: Generic structured log descriptions written in YAML.
- Sigma Converter: A set of python scripts that will process the rules on the backend and perform custom field matching based on specified SIEM query language.
- Machine Query: Resulting search query to filter out alerts during investigations. The query will be based on the specified SIEM.

## Task-3: Sigma Rule Syntax

### Sigma Syntax

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/79297df8-5a59-46f4-9f0d-82d8a53a884e)
- **Title** - Names the rule based on what it is supposed to detect. This should be short and clear.


- **ID** - A globally unique identifier mainly used by the developers of Sigma to maintain the order of identification for the rules submitted to the public repository, found in UUID format. 
- **Status** - Describes the stage in which the rule maturity is at while in use. There are five declared statuses that you can use:

- Stable: The rule may be used in production environments and dashboards.
- Test: Trials are being done to the rule and could require fine-tuning.
- Experimental: The rule is very generic and is being tested. It could lead to false results, be noisy, and identify interesting events.
- Deprecated: The rule has been replaced and would no longer yield accurate results. Therelated field is used to create associations between the current rule and one that has been deprecated.
- Unsupported: The rule is not usable in its current state (unique correlation log, homemade fields).

- **Description:** Provides more context about the rule and its intended purpose. With the rule, you can be as verbose as possible on the malicious activity you intend to detect.

a) Which status level could lead to false results or be noisy, but could also identify interesting events?
- experimental

b) The rule detection comprises two main elements: __ and condition expressions.
- search identifiers

c) What two data structures are used for the search identifiers?
- lists and maps

## Task-4: Rule Writing & Conversion
- First we deploy the machine and go to the elastic server and log into the server with the given credentials

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9d6e575e-a8da-4e00-85e9-309d15765a8b)

a) What command line tool is used to convert Sigma rules?
- sigmac

b) At what time was the AnyDesk installation event created? [MMM DD, YYYY @ HH:MM:SS] 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/523f322d-a2ce-4bdd-9517-dc3e7723adab)

c) What version of AnyDesk was installed? 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/482ca91e-a18a-481a-9627-a203a9dfb49f)



