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

## 1. Opening
- Additional agenda points
   - 
 - Remarks
   - 

## 2. Notes 18 December
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-15-January.md)

## 3.Progress Development & Planning
   - TLN
     - MP:
     - LMS:
   - Noordhoff
     - LA: 
   - Iddink
     - MP:
     - SIS:
     - LMS:
   - SomToday
     - SIS:
     - LMS:
   - Thieme
     - LA: Still no confirmation on participation

## 4. Backlog Items project team

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - **Action**: Edwin will contact Clifton to determine who will arrange the SIS API session and make sure that the session will be held in the coming weeks
  - Update:
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
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update:
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - Update:
7. Adjust design Entitlement API (and or either regarding school and individual)
  - Action holder: Danny, Clifton
  - Update:
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update:
10. Adjust design Catalogue (add stream codes)
  - Action holder: Edwin (Kees), Danny
  - **Action**: Danny and Edwin will plan meeting to discuss this backlog item
  - Update:
11. Determine non happy flows/test scenario's (including returns & cancelations)
  - Action holders: Marcel, Edwin (Jerry), Danny (Hessel), Elias
  - Update:
    - [Usecases](https://github.com/stichtingsem/pilot-phase/blob/main/documents/20210124%20Use%20Cases%20SEM%20Pilot.xlsx)
13. Frontend for demonstration
  - Update:
    - TLN:
    - Noordhoff:
    - Topicus:
    - Iddink:


## Other Backlog Items:
3. Applicability OSR
  - Action holders: Marcel, Erik, Edwin
  - Planning: Folluw up meeting during POC
4. Applicability RIO
  - Action holders: Marcel, Erik, Edwin
  - Planning: Folluw up meeting during POC
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 5. Issues/Questions for Technical Advisory Board
  - Setup Scenarios
  - 

## 6. Any Other Business
  - 

# Actions:
 - Edwin will contact Clifton to determine who will arrange the SIS API session and make sure that the session will be held in the coming weeks
    - Before end of January
 - Danny will update Spotlight with the latest API designs before 25 January
 - Danny and Edwin will plan meeting to discuss the adjustment of the catalogue API (add stream codes)
    - Week 3

# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality

# Completed Backlog Items:
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)

# Completed Actions:
 - Marcel will arange a session on the subject 'setup flows' with the project team in week 3 (22 January from 10:00 - 11:00)
 - Marcel will plan meeting regarding test scenarios and use cases (26 January from 14:30 - 16:00)
