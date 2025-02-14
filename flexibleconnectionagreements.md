# Reference model for *Collective Self-Consumption*

change..

## Context/ Whereas

(1)     It was identified that it is advantageous for data sharing and the eligible party working with that data, that metering and consumption data series refer to the metering point identifier and be independent from the underlying physical metering equipment. That means, that if the underlying physical metering equipment is changed, the metering point identifier doesn’t change.

(2)     For the purpose of this act, 'accounting point master data' shall refer to [TODO].

## Definitions

In this section, each term is defined:

* 'term1', in the context of this act, means ...

## Responsibilities of Market Roles

In this section the responsibilities of each market role should be described.

### Responsibilities of energy community operators

1. Metering point administrators shall make metering point master data available online to final customers and eligible parties, without undue delay and whenever the final customer needs to access or share the data.
2. Metering point administrators shall ensure that final customers can access and make available to eligible parties their validated metered data and receive it in a structured, commonly used, machine-readable and interoperable format.

### Responsibitilies of metering point administrators

1. Metered data administrators shall ensure the equal treatment of all eligible parties.

## Annex

Table I contains information needed by eligible parties to set up for utilising connection point master data access in a Member State. It is primarily describing information that needs to be accessible for them to register, onboard or establish prerequisite infrastructure to take part in the procedures listed in Table III.

### General Information

| ID  | Name                         | Description                                                                                                                                                                                                           |
|-----|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| I1  | National competent authority | *Name* - Name of appointed national competent authority.<br/>*Website* - Website of appointed national competent authority.<br/>*Official contact* - Contact details for managing the mappings of national practices. |
| I2  | National co-ordination instance | *Name* - Name of the national body intended to help ECs.<br/>*Website*<br/>*Email*<br/>*Phone*<br/>*Operational since*<br/>*no. as of now*<br/>*Comments*                                                                                                                                                                                                                   |
| I3  | National regulatory basis for Jointly Acting Self-Consumers  | *Implemented?* Yes/No<br/>*Reference* - to national law<br/>*URL* - weblink to national law<br/>*Operational since*<br/>*no. as of now*<br/>*Comments*                                                                                                                                                                                                                   |
| I4  | National regulatory basis for Local Renewable Energy Communities  | *Implemented?* Yes/No<br/>*Reference* - to national law<br/>*URL* - weblink to national law<br/>*Expression of locational vicinity* how is locational vicinity expressed in your regime (e.g. radios of 500m, need to be behind the same secondary substation etc.)<br/>*Operational since*<br/>*no. as of now*<br/>*Comments*                                                                                                                                                                                                                   |
| I5  | National regulatory basis for Regional Renewable Energy Communities  | *Implemented?* Yes/No<br/>*Reference* - to national law<br/>*URL* - weblink to national law<br/>*Expression of locational vicinity* how is locational vicinity expressed in your regime (e.g. radios of 500m, need to be behind the same secondary substation etc.)<br/>*Operational since*<br/>*no. as of now*<br/>*Comments*                                                                                                                                                                                                                   |
| I6  | National regulatory basis for Citizen Energy Communities  | *Implemented?* Yes/No<br/>*Reference* - to national law<br/>*URL* - weblink to national law<br/>*Comments*                                                                                                                                                                                                                   |
| I7  | Settlement process for ECs | Please describe the settlement process for collective self-consumption schema. Who gathers and processes, which data? |
| I8  | Testing possibilities | Please describe a) the testing possibilities that digital platforms for Energy Communities have and b) how they can onboard to these testing facilities. |
| I9  | Onboarding for CU Operators | Description of what needs to be done by Energy Community operators to found an EC and to connect to the relevant energy market communication. |
| I10 | Multi-participation | Indication about how many ECs an accounting point can be part of at the same time. |
| I11 | Self-consumption calculation responsible | List all parties responsible for calculating self-consumption values.<br/><br/>*Name*<br/>*URL*<br/>*Email*<br/>*Contact information*<br/>*Grid area responsibility* |
| I12 | Self-consumption participation administrator | List all self-consumption participation administrators.<br/><br/>*Name*<br/>*URL*<br/>*Email*<br/>*Contact information*<br/>*Grid area responsibility* |


### Relevant Roles

| Role name                                | Role type | Role description                                                                                                                            |
|------------------------------------------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------|
| Final customer                           | Business  | A party connected to the grid that purchases electricity for its own use. Please note, that this also includes the case of active customer. |
| Connecting system operator                | Business  | A party ... |                     

### Procedures

| No. | Procedure Name                              | Primary Actor  | Preconditions                                         |
|-----|---------------------------------------------|----------------|-------------------------------------------------------|
| 1   | Onboarding to a flexible connection agreeent | Final customer | Final customer is identified by the CSO. |
| 2   | Offboarding from a flexible connection agreement | Final customer | The final customer is the holder of a flexible connection agreement. |
| 3   | Issuing a flexible connection limit | Connecting system operator | The final customer and the CSO have an active flexible connection agreement. |

In the following, each procedure is described in steps, whilst each step represents an information exchange between two roles. Each procedure is visualised using a BPMN diagram.

#### Procedure 1 - Onboarding to a flexible connection agreeent

| Step No. | Step                                   | Step description                                                                                                     | Info producer        | Info consumer  | Information exchanged             |
|----------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------|----------------------|----------------|-----------------------------------|
| 1.1      | Identify connecting system operator (CSO) | Final customers identify the data access provider that is responsible for their metering points under consideration. | Competent authority  | Final customer | [not relevant] |
| 1.2      | CSO asks final customer for close-to-realtime data | CSO provides means for final customer to provide connectivity with connection agreement point data. | Connecting system operator | Final customer | A - Consent request |
| 1.3      | Final customer accepts or rejects consent request | The final customer accepts or rejects the request from the CSO and sends back the respective information. | Final Customer | Connecting system operator | B - Consent information |
| 1.4      | Send close-to-realtime consumption data | The final customer sends close-to-realtime consumption data to the CSO. | Final customer | Connecting system operator | C - Close-to-realtime consumption data |

#### Procedure 2 - Offboarding from a flexible connection agreement

| Step No. | Step                                   | Step description                                                                                                     | Info producer        | Info consumer  | Information exchanged             |
|----------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------|----------------------|----------------|-----------------------------------|
| 2.1      | Identify connecting system operator (CSO) | Final customers identify the data access provider that is responsible for their metering points under consideration. | Competent authority  | Final customer | [not relevant] |
| 2.2      | CSO asks final customer for close-to-realtime data | CSO provides means for final customer to provide connectivity with connection agreement point data. | Connecting system operator | Final customer | A - Consent request |
| 2.3      | Final customer accepts or rejects consent request | The final customer accepts or rejects the request from the CSO and sends back the respective information. | Final Customer | Connecting system operator | B - Consent information |
| 2.4      | Send close-to-realtime consumption data | The final customer sends close-to-realtime consumption data to the CSO. | Final customer | Connecting system operator | C - Close-to-realtime consumption data 

### Data Exchanged

| ID  | Name of information object   | Definition of attributes of exchanged information object                                                                                                      |
|-----|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A   | Metering point identificator | Unique identifier for the metering point within the metered data administrator’s meter identification space.                                                  |
| B   | Metered data specification   | *Reading start timestamp* - Start of the interval covered by the data package.<br/>*Reading end timestamp* - End of the interval covered by the data package. |
|     |                              |                                                                                                                                                               |
