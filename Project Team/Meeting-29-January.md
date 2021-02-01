# Project Team Meeting

## Agenda
1. Opening
2. Notes 15 January
3. Progress Development & Planning
4. Backlog Items project team
    - Update Backlog Items
    - Other Backlog Items
5. Issues/Questions for Technical Advisory Board
6. AOB

## Summary:
- Actions
- Project Team Decisions
- Completed Backlog Items
- Completed Actions

The meeting started with an update from Danny because of his limited time. His update is processed in the backlog items.

## 1. Opening
- Additional agenda points
  - No Aditional Agenda Points
- Remarks
  - No Opening Remarks

## 2. Notes 15 janaury
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-15-January.md)
    - There were no remarks on the notes and are thereby approved

## 3.Progress Development & Planning
   - TLN
     - MP: The Entitlement API is ready and is up and running in the acceptance environment. Partners in the ecosystem can ask for an access token to get access and link to the API. TLN wants to move the API to production because of security guidelines.
     - LMS: Development of the connections to the LMS will start next week (1st of February)
   - Noordhoff
     - LA: The catalogue API is on the current sprint. Because of an issue and the lockdown development has been delayed.
        - **Action**: Elias gives update to project team on progress - 3 February
   - Iddink: Setup in place pipielines
     - Iddink started development last monday (25th of January). The base setup (pipelines) is in place
     - MP:  Development of the entitlement API (including stub data) is sterted
     - Other: The order of development of the API's and connections is flexible. Depends on progress within Iddink and the available API's at partners within the ecosystem
   - SomToday
     - SIS: SomToday will finish the SIS API in the next week and will be available in test environment for partners from the 8th of February
         - **Action**: Luke informs project team on the release of the SIS API - 8 February
     - LMS: Start when adjusted designs are approved
   - Thieme
     - LA: Still no confirmation on participation
         - **Action**: Marchien contacts Pieter Ruempol on their participation

## 4. Backlog Items project team

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - **Action**: Edwin will arrange SIS API session in the coming weeks and wil invite Jorim from Topicus
  - Update: 12 February
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - Update:
    - [Proposal](https://github.com/stichtingsem/pilot-phase/issues/1)
    - Meeting Notes 22-1-2021:
       - Regarding the setup between two parties
         - When party A wants to use the API provided by party B, B will create a client for A. This client consists of a client_id, a client_secret and the set of scopes that can be used by this client. This set may contain scopes that span across multiple API's. If for instance B provides a Usage API and a Results API a single client may be defined that's allowed to use both API's.
         - The endpoints/urls for the different API's (for now) will not be maintained in a central registry. Each party should maintain their own list of the urls of the other parties API's.
      - On authorization by the school:
         - The school-specific authorization flow as described above always happens within the context of one specific digideliveryid. Meaning if a school uses multiple digideliveryid's the authorization flow will have to be started for each digideliveryid separately. If it turns out in practice this is too much of a burden on the school's administrator we can consider allowing for an array of digideliveryid's, but this greatly introduces complexity, especially in the various non-happy flows.
         - Which data exchanges involve authorization by the school is not fully clear at this point. The Catalogue API clearly is one that does not involve the school's authorization. The same seems to apply to the Entitlements sent to the Learning Application by the Marketplace. As for the other exchanges some discussion was had and probably needs to continue.
    - The project team agrees on the following points:
      - Client ID can be used for multiple services
      - During PoC no central registration like OSR
      - Setup will be done at DigiDelivery Id level. Multiple DigiDeliveryID for one school = multiple setups
    - The project team discusses the ways of setup (school level or partner level). There is no consensus on this point
      - Catalogue API: setup on partner level
      - SIS API: setup on school level
      - Usage API: setup on school level
      - Progress & Results API: setup on school level
      - Entitlement API: discussion
         - Technical Advisory Board will be consulted on this matter
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update: Adjusted designs will be available as pull request from the 1st of February after Clifton helps Danny with release on Stoplight/Github
    - **Action**: Danny informs project team when the pull request is available and gives a summary (release notes) by mail
       - This actions contains all the changes for items 5, 6, 7, 8
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - Update: Adjusted designs will be available as pull request from the 1st of February after Clifton helps Danny with release on Stoplight/Github
7. Adjust design Entitlement API (and or either regarding school and individual)
  - Action holder: Danny, Clifton
  - Update: Adjusted designs will be available as pull request from the 1st of February after Clifton helps Danny with release on Stoplight/Github
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update:Adjusted designs will be available as pull request from the 1st of February after Clifton helps Danny with release on Stoplight/Github
10. Adjust design Catalogue (add stream codes)
  - Action holder: Edwin (Kees), Danny
  - Update: Edwin had contact with Danny on the streamcodes. They concluded that stream codes would stay part of the design and will be part of the adjusted designs (pull request)
11. Determine non happy flows/test scenario's (including returns & cancelations)
  - Action holders: Marcel, Edwin (Jerry), Danny (Hessel), Elias
  - Update:
    - [Usecases](https://github.com/stichtingsem/pilot-phase/blob/main/documents/20210128%20Use%20Cases%20SEM%20Pilot.xlsx)
    - This is the last version (90% version) of the use cases and will be the base for testing
    - **Action**: Project team members check the use cases on correctness and integrality
13. Frontend for demonstration
  - Update:
    - TLN: No Update
    - Noordhoff: No Update
    - Topicus: No Update 
    - Iddink: No Update
3. Applicability OSR
  - Action holders: Marcel, Erik, Edwin
  - Planning: Marcel will plan meeting in February to get informed and determine progress
4. Applicability RIO
  - Action holders: Marcel, Erik, Edwin
  - Planning: Marcel will plan meeting in February to get informed and determine progress


## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 5. Issues/Questions for Technical Advisory Board
  - The Technical Advisory Board will be informed/consulted (no formal decisions) on the following: 
    - Setup Scenarios
    - Use Cases/Test scenarios
    - Push functionality in ENtitlemenmt API
        - Market Place can push entitlements to the Learning Application and Learning Material System. This is necessary because of the validity of the transactions
          - Market Place will be updated (confirmation) by the Learning Application in three phases
            1. Receive message
            2. Process message
            3. Progress message
        - This push mechanism is available within the architecture but works different from the other connections
        - This will be part of the set of appointments

## 6. Any Other Business
  - 

# Actions:
  - Danny informs project team when the pull request is available and gives a summary (release notes) by mail
    - 1 February
 - Elias gives update to project team on progress
    - 3 February
 - Luke informs project team on the release of the SIS API
    - 8 February
 - Marchien contacts Thieme (Pieter Ruempol) on their participation
    - 5 February
 - Edwin will arrange SIS API session (Backlog Item 1)
    - 11 February
    - Jorim (Topicus) will be invited for the session
 - Project team members check the use cases on correctness and integrality
    - 11 February
 
# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality
 - Setups:
    - Client ID can be used for multiple services
    - During PoC no central registration like OSR
    - Setup will be done at DigiDelivery Id level. Multiple DigiDeliveryID for one school = multiple setups

# Completed Backlog Items:
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)

# Completed Actions:
 - Marcel will arange a session on the subject 'setup flows' with the project team in week 3 (22 January from 10:00 - 11:00)
 - Marcel will plan meeting regarding test scenarios and use cases (26 January from 14:30 - 16:00)
 - Danny and Edwin will plan meeting to discuss the adjustment of the catalogue API (add stream codes)
