# Project Team Meeting

## Agenda
1. Opening
2. Notes 18 December
3. Progress Development & Planning
4. Backlog Items project team
    - Update Backlog Items
    - Other Backlog Items
5. Issues/Questions for Technical Advisory Board
6. AOB

## 1. Opening
- Additional agenda points
   - Status Technical Advisory Board (Edwin)
     - Last meeting: 17 December
     - Next meeting: 21 January
     - Introduction new board member (Thijs WIllems)
     - Walkthrough/Introduction Architecture on Spotlight
     - Status update from Clifton/Marcel
     - Advice: Use ECK standard as base for the test scenario
   - Remarks
     - No opening remarks

## 2. Notes 18 December
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-18-December.md)

## 3.Progress Development & Planning
   - TLN
     - MP:
        - The Entitlement API is developed, webhooks will be added at a later moment. At the moment stubs are being developed for test and validation purposes
        - Danny and Edwin discussed/determined that there has to be a confirmation message of a transaction in the process flow. Danny will add this in the design of the       entitlement API
     - LMS:
        - The development of the connections to the LMS has started, but depends on the availability of the various API's (entitlement, SIS, catalogue)
   - Noordhoff
     - LA: 
        - Development of the catalogue API is on the current development sprint which will end in the last week of January
     - Other: 
        - There have been some grooming sessions on the consumption of services
        - There is a React project for the developmnent of the LA interface
   - Iddink
     - Resources (developers) are assigned to the project
     - Design sessions are completed
     - Development will start in week 3
        1. Develop entitlement API
        2. Link with catalogue API
        3. Develop SIS API
        4. Develop LMS connections
   - SomToday
     - SIS:
       - The SIS API is being developed at the moment. Expectation is that the SIS API will be available in the test environment in two weeks from now. The webhooks will not be available in this release  
     - LMS:
       - The development of the connections to the LMS will be started when the various API's are available (start of February)
   - Thieme
     - LA:
       - Still no confirmation on participation
       - Thieme can still join, but they have to conform to the designs and agreements that are in place. This also goes for reviewers of the pilot 

## 4. Backlog Items project team

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - Update:
     - There would be a session on this topic, but this session has not taken place
     - **Action**: Edwin will contact Clifton to determine who will arrange the SIS API session and make sure that the session will be held in the coming weeks
        - The quenstions from Topicus will be on the agenda of this session
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - Update:
    - Are there remarks on the proposal (shared 4 January) that Luke made?
        - [Proposal](https://github.com/stichtingsem/pilot-phase/issues/1)
    - **Action**: Marcel will arange a session on this subject with the project team in week 3 > 22 January from 10:00 - 11:00 
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update:
    - Proposal: Rename it to **Consumption API**
      - Decision project team: The Usage API will **not** be renamed to consumption API
    - Danny: Designs are adjusted and compared to other standards. Spotlight has to be updated with the last version of the API designs
      - Deadline: 25 January
    Specificaties doorgewerkt en vergeleken met andere standaarden > Moet nog naar Spotlight (medio week 2)
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - Update:
    - Danny: Designs are adjusted and compared to other standards. Spotlight has to be updated with the last version of the API designs
      - Deadline: 25 January
7. Adjust design Entitlement API (and or either regarding school and individual)
  - Action holder: Clifton
    - Update Danny: Designs are adjusted and compared to other standards. Spotlight has to be updated with the last version of the API designs
      - Deadline: 25 January
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update:
    - Danny: Designs are adjusted and compared to other standards. Spotlight has to be updated with the last version of the API designs
      - Deadline: 25 January
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)
  - Action holder: Danny, Edwin, Clifton
  - Update:
    - Danny: Done
10. Adjust design Catalogue (add stream codes)
  - Action holder: Edwin (Kees), Danny
  - Update:
    - Danny: This action is still open.
      - **Action**: Danny and Edwin will plan meeting to discuss this backlog item
11. Determine non happy flows/test scenario's (including returns & cancelations)
  - Action holders: Marcel, Edwin (Jerry), Danny (Hessel), Elias
  - Update:
    - **Action**: Marcel is planning a meeting (before end of January) and makes a first version
13. Frontend for demonstration
  - **Project Team Decision**: Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality


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
  - No questions or issues to share with Technical Advisory Board

## 6. Any Other Business
  - **Action**: Edwin will arrange that Jorim (Topicus) is invited for the SIS API session

# Actions:
 - Edwin will contact Clifton to determine who will arrange the SIS API session and make sure that the session will be held in the coming weeks
    - Before end of January
 - Marcel will arange a session on the subject 'setup flows' with the project team in week 3
    - 22 January from 10:00 - 11:00
 - Danny will update Spotlight with the latest API designs before 25 January
 - Danny and Edwin will plan meeting to discuss the adjustment of the catalogue API (add stream codes)
    - Week 3
 - Marcel will plan meeting regarding test scenarios and use cases
    - Before end of January

# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality
