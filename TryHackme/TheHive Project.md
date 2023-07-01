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
