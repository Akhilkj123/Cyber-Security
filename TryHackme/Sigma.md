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
- **Title** - Names the rule based on what it is supposed to detect. This should be short and clear.
- **ID** - A globally unique identifier mainly used by the developers of Sigma to maintain the order of identification for the rules submitted to the public repository, found in UUID format. 
- **Status** - Describes the stage in which the rule maturity is at while in use. There are five declared statuses that you can use:

- Stable: The rule may be used in production environments and dashboards.
- Test: Trials are being done to the rule and could require fine-tuning.
- Experimental: The rule is very generic and is being tested. It could lead to false results, be noisy, and identify interesting events.
- Deprecated: The rule has been replaced and would no longer yield accurate results. Therelated field is used to create associations between the current rule and one that has been deprecated.
- Unsupported: The rule is not usable in its current state (unique correlation log, homemade fields).

