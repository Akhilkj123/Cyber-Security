## Task -3
## Elastic stack
- collection of different open source components linked together to help users take the data from any source and in any format and perform a search, analyze and visualize the data at real-time.

### Elasticsearch 
- full-text search and analytics engine used to store JSON-formated documents. 
- important component used to store, analyze, perform correlation on the data, etc.

### Logstash
- data processing engine used to take the data from different sources, apply the filter on it or normalize it, and then send it to the destination.
- **input part** is where the user defines the source from which the data is being ingested. 
- **filter part** is where the user specifies the filter options to normalize the log ingested above.
- **output part** is where the user wants the filtered data to send.

### Kibana
- web-based data visualization that works with elasticsearch to analyze, investigate and visualize the data stream in real-time.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/8f990adc-170a-4a5d-8a37-8dfe29d681b3)

## Task - 6
## KQL(Kibana Query Language)
- search query language used to search the ingested logs/documents in the elasticsearch.


With KQL, we can search for the logs in two different ways.

### a) Free text Search
- allows users to search for the logs based on the text-only.

####  i)Wild Card
- KQL allows the wild card * to match parts of the term/word.

#### ii) Logical Operators (AND | OR | NOT)
 - 1- OR Operator
- 2- AND Operator
- 3- NOT Operator

### b) Field-based search

- we will provide the field name and the value we are looking for in the logs. 



