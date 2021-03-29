# Project Team Meeting

## Agenda
1. Opening
2. Notes 12 March
3. Actions
4. Progress Development, Linking & Testing
5. Progress & Results API
6. OSR use cases
7. AOB

## Summary:
- Actions
- Project Team Decisions
- Completed Backlog Items
- Completed Actions

## 1. Opening
 - Additional agenda points
   - No agenda points added
 - Remarks
   - No opening remarks

## 2. Notes 26 February
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-12-March.md)
   - There were no remarks on the notes and are thereby approved

## 3. Actions
 - Arrange seperate meeting to finalize progress & results API
      - See agenda point Progress & Results API
 - Determine use cases to share with Kennisnet (OSR) > First share with Project group for validation
      - See agenda point OSR use cases - Closed

## 4. Progress Development, Linking & Testing
        
   - TLN
     - Received feedback on entitlement API from Topcus and Noordhoff. Main focus will be to fix the Entitlement API
     - Hessel is contact for credentials
     - Noordhoff informs that they have issues with DNS. Danny will take action on this
     - Connections will be made > LMS and MP roles
     - TLN is working on Admin tool (dashboard)
   
   - Noordhoff
     - Usage API depends on availability entitlement data
     - Noordhoff is connected to SIS API of Topicus
     - Need to look at what we need to do in the ADMIN part to show the flow

   - Iddink
     - Created 4 applications to show how API's and connections work
     - There is an admin environment (not nice, but works)
     - Started connecting to Noordhoff and Topicus > Issues will be recorded in Github
     - Hope to finish entitlment connection (incoming)

     - What is the technical mechanism of Iddink?
       - Iddink is working with webhooks -> data are not on the webhook part
       - Issues/questions will be shared next week
     - Iddink will be ready for demo on the 5th of April

   - SomToday
     - All partners are connecting to SIS API
     - Work around for group data besides working on the real fix
     - Working on entitlement API of TLN > Focus for next week
   
   
       
## 5. Progress & Results API
  - Action Holders: Clifton, Danny, Edwin
  - [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
  - Update:
    - Clifton:
      - There is a rough skeleton version of the service. Next week there will be a follow-up session with Kees to further formailze the design
      - The progress & results API will be XML based to support CMI5 (not REST like the other services)
  - **Action**: Arrange follow-up meeting in week 13 - Clifton

## 6. OSR Use Cases
  - [Related Issue](https://github.com/stichtingsem/pilot-phase/issues/11)
  - Update:
     - Only the use case "Als ketenpartij wil ik de mogelijkheid hebben om mijn services (endpoints) te publiceren via OSR, zodat scholen en andere ketenpartijen weten welke services beschikbaar zijn" wil be shared with Kennisnet (OSR). This is the use case for the central phone book
     - The other use cases (mandates) will not be shared with Kennisnet 


## 7. Any Other Business
  - Monday is critical for end to end testing
    - Danny, Henk, Jorim will be in the sync meeting for testing and alignment
  - Next meeting on 9 April (evaluation)

## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

# Action

- Arrange follow-up meeting progress & results API
  - Clifton 

# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality
 - Setups:
    - Client ID can be used for multiple services
    - During PoC no central registration like OSR
    - Setup will be done at DigiDelivery Id level. Multiple DigiDeliveryID for one school = multiple setups

# Completed Backlog Items:
1. Refine scopes SIS API
2. Design setup service
4. Applicability RIO
5. Design Usage API (MP)
7. Adjust design Entitlement API (and or either regarding school and individual)
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)
10. Adjust design Catalogue (add stream codes)
  - Conclusion: Stream codes will stay part of the design
11. Determine non happy flows/test scenario's (including returns & cancelations)
13. Frontend for demonstration

# Completed Actions:
 - Marcel will arange a session on the subject 'setup flows' with the project team in week 3 (22 January from 10:00 - 11:00)
 - Marcel will plan meeting regarding test scenarios and use cases (26 January from 14:30 - 16:00)
 - Danny and Edwin will plan meeting to discuss the adjustment of the catalogue API (add stream codes)
 - Danny informs project team when the pull request is available and gives a summary (release notes) by mail
 - Elias gives update to project team on progress
 - Marchien contacts Thieme (Pieter Ruempol) on their participation
 - Project team members check the use cases on correctness and integrality
 - Luke informs project team on the release of the SIS API
 - Danny will plan a meeting with Edwin, Clifton, Luke on this subjects (multiple back log items)
 - Danny will update Marcel on planning
 - Elias will update Marcel on planning
 - Edwin will plan session on SIS API in week 7
 - Elias (Clifton) determine if there is a version of the document ("Moving from a chain to an ecosystem") without remarks
 - Inform members of the Steering Committee on the progress of the SEM PoC. Determine position/opinion for the next Steering Committee
 - Update sheet for Steering Committee
 - Discuss contents of the entitlement API (MP > LMS)
 - Questions Topicus (Jorn) will be discussed by the technical group
 - Finish designs (API's, setup, events)
 - Share remarks on picture of connections with Edwin
 - Determine use cases to share with Kennisnet (OSR) > First share with Project group for validation
