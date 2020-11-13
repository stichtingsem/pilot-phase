# Decisions Preparation Team 13-11-2020

## Do the API's make it possible to have a closed administration
Related document: [Data flows](https://github.com/stichtingsem/pilot-phase/blob/main/documents/work-stream-finance-administration/20200817%20SEM%20POC%20FIN%20ADMIN%20Dataflow%20EV.pdf)

## Use of data from various contexts (need for profiles)
Related Issue: [SIS API](https://github.com/stichtingsem/pilot-phase/issues/4)

Do we need profiles on API's regarding use of data(parts) for the pilot or afterwards?

Example: Is group structure available for all roles?

## Purpose/use of (double) data components
Related Issues 
[Data usage](https://github.com/stichtingsem/pilot-phase/issues/6) |
[Entitlement API](https://github.com/stichtingsem/pilot-phase/issues/3)

Data components like product name, content URL are shared in the catalogue API (source data) and entitlement API (transaction data - not updated)

Principle EvW: Data is only exchanged upon first use and only within the context of use.

Do we remove those kind of double components or make a clear document on how to use the data in the API's?

Document that describes the target binding based on the role that is fulfilled?

## Entitlement API

Related Issues: [Entitlement API](https://github.com/stichtingsem/pilot-phase/issues/3)

1. Business model included in the API?

2. Define status entitlement in API or separate service?
Based on the design it is not possible to determine quantity activated, quantity shared and quantity available. This are important aspects to know for processes like cancelation and returns

3. Which identifiers do we allow to be used (in the pilot)?

### Proposal:
Users: ECK iD
Organizations: Digi Delivery Id
Product: EAN
Market Place: URL (created in ecosystem)

OSR and RIO are researched/evaluated during pilot foor applicability in roll-out, but not implemented during pilot phase


