# Decisions document Preparation Team meeting 13-11-2020

## Purpose meeting:
- Remove issues so we can start developing API's 
- If necessary determine short term actions to get things clear

## Do the API's make it possible to have a valid transactions & balanced administration
Related documents:
[Data flows](https://github.com/stichtingsem/pilot-phase/blob/main/documents/work-stream-finance-administration/20200817%20SEM%20POC%20FIN%20ADMIN%20Dataflow%20EV.pdf) |
[Final Report Finance & Admin Track](https://github.com/stichtingsem/pilot-phase/blob/main/documents/work-stream-finance-administration/20200924%20FINAL%20Work-%20Discussion%20document%20Stream%20Finance%20Admin%20(CONCEPT).pptx)

### Outcome Track Finance & Admin:
Technical solution contains **all** required fields for a valid transaction, but:
- Entitlement contains (to) many required (and optional) fields
  - Discuss purpose and target binding with technical stream (next phase)
    - Examples:
     - Business model
     - Duplication of data:
     - Title (name), URL of EAN in interface
     - School name
     - Group (structure)
  - Does the source always contain all the correct and actual data?
  - Status entitlement from LA to MP and LMS in separate service/call
     - Example: entitlement quantity vs. quantity in use 
  - Determine owner of data parts

## Architecture & Data

[Architecture](https://stichtingsem.stoplight.io/docs/sem-technology-prototype/docs/introduction.md)

### 1. Do we implement webhooks and events in every interface or are there exceptions?

Can we reach a valid transaction and balanced administration with the defined architecture? Do we need to specify certain business rules (best practice) to ensure that API's and technical interfaces are implemented correct?
  - Ecxample: 
    - Order of events

### 2. Use of data from various contexts (need for profiles)

Related Issue: [SIS API](https://github.com/stichtingsem/pilot-phase/issues/4)

Do we need profiles on API's regarding use of data(parts) for the pilot or afterwards?

Example: Is group structure available for all roles?

### 3. Purpose/use of (double) data components
Related Issues 
[Data usage](https://github.com/stichtingsem/pilot-phase/issues/6) |
[Entitlement API](https://github.com/stichtingsem/pilot-phase/issues/3)

Data components like product name, content URL are shared in the catalogue API (source data) and entitlement API (transaction data - not updated)

Edwin: **Data is only exchanged upon first use and only within the context of use**.

Do we remove those kind of double components or make a clear document on how to use the data in the API's?

Document that describes the target binding based on the role that is fulfilled?

### 4. How to ensure that data at the source is correct and actual?

## Setups (Subscribing service)

### 1. What is needed to create a setup or subsribe to a API? What is an acceptable MVP for the pilot? We have to prove it is easy to setup!

### 2. Is OSR sufficient to be the "central phonebook" for the ecosystem? Or do we need something more?
Related Issue[OSR](https://github.com/stichtingsem/pilot-phase/issues/11)

Luke: although I think this would require a quite significant addition to the functionality of OSR as its main components (mandates and endpoints) currently only exist within the context of a specific school. But that's a discussion / research probably best held within the context

## SIS API
Related Issue: [SIS](https://github.com/stichtingsem/pilot-phase/issues/4)

### 1. How to exchange personal data?

#### Proposal Edwin: We use the Edukoppeling standard for the exchange of personal data.

## Entitlement API

Related Issues: [Entitlement API](https://github.com/stichtingsem/pilot-phase/issues/3) | 
Design: [API](https://stichtingsem.stoplight.io/docs/sem-technology-prototype/reference/entitlement.v1.yaml)

### 1. Business model included in the API?
Elias: Yes. For data minimization an open question remains if we can reduce this to only the id, since name and description are already exchanged in catalogue API.

### 2. Define status entitlement in API or separate service?
Marcel: Based on the design it is not possible to determine quantity activated, quantity shared and quantity available. This are important aspects to know for processes like cancelation and returns > Do we adjust the API or design additional status API?

### 3. Which identifiers do we allow to be used (in the pilot)?

#### Proposal:
Users: ECK iD
Organizations: Digi Delivery Id
Product: EAN
Market Place: URL (created in ecosystem)

OSR and RIO are researched/evaluated during pilot foor applicability in roll-out, but not implemented during pilot phase

### 4. For the use case in which a student receives a license on behalf of a school (the school pays), I now miss the option to include information from the school in addition to the student's data.

### 5. Get all entitlements for a specific individual is not designed. Add this call?

## Catalogue API

### 1. Match API on ECK 2.3
Related Issue: [ECK 2.3](https://github.com/stichtingsem/pilot-phase/issues/15)

Do this match in front or start with current design?

### 2. Add stream codes to products 
Related Issue: [Stream codes]{https://github.com/stichtingsem/pilot-phase/issues/5)

Blocking?

## Remaining Work - Non Blocking
[Progress & Results Service](https://github.com/stichtingsem/pilot-phase/issues/14)

Proposal: Design during development

[Non Happy Flows/Test SCenarios]](https://github.com/stichtingsem/pilot-phase/issues/9)

Proposal: Determine during pilot

[Attributes Policy/Data Covenant](https://github.com/stichtingsem/pilot-phase/issues/10)

Proposal: Check later

[OSR](https://github.com/stichtingsem/pilot-phase/issues/11)

Prposal: Continue research for roll-out

[RIO](https://github.com/stichtingsem/pilot-phase/issues/12)












