# Project Team Meeting

## Agenda
1. Opening
2. Notes 29 January
3. Progress Development & Planning
4. Backlog Items project team
    - [Setup](https://github.com/stichtingsem/pilot-phase/blob/main/documents/Setups.xlsx)
    - [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
    - [Usecases](https://github.com/stichtingsem/pilot-phase/blob/main/documents/20210128%20Use%20Cases%20SEM%20Pilot.xlsx)
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

## 2. Notes 29 janaury
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-29-January.md)
    - 

## 3.Progress Development & Planning
   - TLN
     - MP: 
     - LMS: 
   - Noordhoff
     - LA: 
   - Iddink:
     -  general set-up for the 3 extern service ready. Authentication is under construction. Some internal discussions what is the best way to deal with User Authentication and extern System authentication. 
     - catalogue api and first version of UX ready, we like to connect with de LA-Catalogue service to work with better example data. (we also have a small LA component build for this, just for testing and validation)
     - SIS api: implementing this, UX design almost ready. Now Topicus is ready I will contact them to see what we can do with it. 
     - Entitlement to LMS technical ready, Some issue that we maybe want to share later.
   - SomToday
     - SIS: First version of the SIS API is released to the test environment as planned. SomToday is in contact with TLN to arrange a test setup. This will take place next week
     - LMS:
   - Thieme
     - LA: Marcel and Marchien had a meeting with Thieme (Pieter, Janneke). They want to join, but they weren't aware of the status, progress and planning of the pilot. Based on the expectation to start testing second half February it is not feasible that the API's of the LA will be ready in time. Thieme will be part of the review group and would like to join in the next phase

## 4. Backlog Items project team

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - **Action**: Edwin will plan session on this subject in week 7
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - Update:
    - [Setups](https://github.com/stichtingsem/pilot-phase/blob/main/documents/Setups.xlsx)
    - [Issue](https://github.com/stichtingsem/pilot-phase/issues/1)
    - Do the project team members support the starting point?
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update: Pull request/branch is available in Github/Stoplight
     - Reaction Project Team:
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - Update: [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
  - Reaction:
7. Adjust design Entitlement API (and or either regarding school and individual)
  - Action holder: Danny, Clifton
  - Update: Pull request/branch is available in Github/Stoplight
     - Reactions Project Team:
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update: See Issue at backlog item 6
11. Determine non happy flows/test scenario's (including returns & cancelations)
  - Action holders: Marcel, Edwin (Jerry), Danny (Hessel), Elias
  - Update:
    - [Usecases](https://github.com/stichtingsem/pilot-phase/blob/main/documents/20210128%20Use%20Cases%20SEM%20Pilot.xlsx)
    - **Action**: Project team members check the use cases on correctness and integrality
13. Frontend for demonstration
  - Update:
    - TLN: No Update
    - Noordhoff: No Update
    - Topicus: No Update 
    - Iddink: No Update
3. Applicability OSR
  - Action holders: Marcel, Erik, (Edwin)
  - Planning: Meeting on 18 February
4. Applicability RIO
  - Action holders: Marcel, Erik, Edwin
  - Planning: Meeting on 22 February


## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 5. Issues/Questions for Technical Advisory Board
  - 

## 6. Any Other Business
  - Edwin: Definition of an event
  - Edwin: Data duplication & Data fit for purpose

# Actions:
  
 - Edwin will arrange SIS API session (Backlog Item 1)
    - Edwin will plan session on this subject in week 7
    - Jorim (Topicus) will be invited for the session
 - Project team members check the use cases on correctness and integrality
 
# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality
 - Setups:
    - Client ID can be used for multiple services
    - During PoC no central registration like OSR
    - Setup will be done at DigiDelivery Id level. Multiple DigiDeliveryID for one school = multiple setups

# Completed Backlog Items:
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)
10. Adjust design Catalogue (add stream codes)
  - Conclusion: Stream codes will stay part of the design

# Completed Actions:
 - Marcel will arange a session on the subject 'setup flows' with the project team in week 3 (22 January from 10:00 - 11:00)
 - Marcel will plan meeting regarding test scenarios and use cases (26 January from 14:30 - 16:00)
 - Danny and Edwin will plan meeting to discuss the adjustment of the catalogue API (add stream codes)
 - Danny informs project team when the pull request is available and gives a summary (release notes) by mail
 - Elias gives update to project team on progress
 - Marchien contacts Thieme (Pieter Ruempol) on their participation
 - Luke informs project team on the release of the SIS API
