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

The meeting started with an update on the most important issues because of the limited time Clifton had available. The update on the issues is processed in the backlog items.

## 1. Opening
 - Additional agenda points
   - No Aditional Agenda Points
 - Remarks
   - No Opening (half way ;-)) Remarks

## 2. Notes 29 janaury
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-29-January.md)
    - There were no remarks on the notes and are thereby approved

## 3.Progress Development & Planning
   - TLN
     - MP: The Entitlement API is ready and is up and running in the acceptance environment
     - LMS: Development not started
        - **Action**: Danny will update Marcel on planning (16 February)
     - Test: Hessel is in contact with Jorim (Topicus/SomToday) on testing the SIS API
   - Noordhoff
     - LA: More dedicated development capacity (3 developers). No clarity on progress and planning. After sprint and demo clarity on remaning work and planning. Focus is on catalogue API
       - **Action**: Elias will update Marcel on planning (17 February)
   - Iddink:
     -  General set-up for the 3 extern service ready. Authentication is under construction. Some internal discussions what is the best way to deal with User Authentication and extern System authentication.
     - Catalogue api and first version of UX ready, we like to connect with de LA-Catalogue service to work with better example data. (we also have a small LA component build for this, just for testing and validation)
     - SIS api: Implementing this, UX design almost ready. Now Topicus is ready I will contact them to see what we can do with it. 
     - Entitlement to LMS technical ready, Some issue that we maybe want to share later
     - Test SIS API SomToday: Iddink wants to connect to the SIS API of SomToday. Erik mentions that Iddink has to contact Jorim to get information for connecting to the SIS API.
   - SomToday
     - SIS: First version of the SIS API is released to the test environment as planned. SomToday is in contact with TLN to arrange a test setup. This will take place next week
     - LMS: Next sprint focus on feedback on SIS API. After that start with connections to LMS
   - Thieme
     - LA: Marcel and Marchien had a meeting with Thieme (Pieter, Janneke). They want to join, but they weren't aware of the status, progress and planning of the pilot. Based on the expectation to start testing second half February/first half of March it's not feasible that the API's of the LA will be ready in time. Thieme will be part of the review group and would like to join in the next phase

Remark:
- Marchien mentions that it should be clear when and how (progress & demonstration) we will inform the reviewing partners. Expectations have to be managed.

## 4. Backlog Items project team

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - **Action**: Edwin will plan session on this subject in week 7
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - Update:
    - [Issue](https://github.com/stichtingsem/pilot-phase/issues/1)
    - [Setups](https://github.com/stichtingsem/pilot-phase/blob/main/documents/Setups.xlsx)
    -   Update: Edwin will discuss the issue/subject with Luke. The subject will also be on the agenda for the meeting (Tuesday 16 February)
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update: Pull request/branch is available in Github/Stoplight
     - Edwin has to check the design
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
    - Update: 
       - Danny: No decision on the content (not in sync on the details)
       - Clifton: Make a proposal and discuss about it
       - Results need to be shared on real-time basis > All the results from a certain student
       - Results will be disclosed once a task is completed > Every company (LA) has his own opinion
       - There needs to be a group discussion (Edwin, Danny, Clifton, Luke) on this subject
          - Initial proposal from this group
          - ECK iD is the identifier for enrolled (SIS) students. Determine identifier for webshop delivery
     - **Action**: Danny will plan a meeting with Edwin, Clifton, Luke on this subject (16 February 12:00 - 13:00)
7. Adjust design Entitlement API (and or either regarding school and individual)
  - Action holder: Danny, Clifton
  - Update: Pull request/branch is available in Github/Stoplight > DONE
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update: Will be part of the meeting on 16 February
11. Determine non happy flows/test scenario's (including returns & cancelations)
  - Action holders: Marcel, Edwin (Jerry), Danny (Hessel), Elias
  - Update:
    - [Usecases](https://github.com/stichtingsem/pilot-phase/blob/main/documents/20210128%20Use%20Cases%20SEM%20Pilot.xlsx)
    - **Action**: Project team members check the use cases on correctness and integrality
    - Update: No comments on the latest version of the use cases/test scenarios. This version will be the starting point of the test phase.
13. Frontend for demonstration
  - Update:
    - TLN: No Update
    - Noordhoff: No Update
    - Topicus: Use own interface
    - Iddink: Use own interface
3. Applicability OSR
  - Action holders: Marcel, Erik, (Edwin)
  - Planning: Meeting on 18 February
4. Applicability RIO
  - Action holders: Marcel, Erik, Edwin
  - Planning: Meeting on 22 February
 
Remarks:
- Events & Webhooks
    - Possible approaches on sharing data within event:
        - Always
        - Never
        - Sometimes > Most practical: Determine approach (always or never) per interface
    - Edwin will share proposal based on their point of view
    - Clifton: Implementation of events/webhooks is optional and can be done in a later phase
        - First focus on data exchanges
    - Marcel: Events and webhooks are part of the working hypothesis of the PoC and should be part of the demo
        - Clifton: Noordhoff will implement them on the catalogue API so we can show that in the review/demo
        - Danny: Each webhook/event should have it's counterpart
        - Edwin: We have to look at it from a market place point of view   

## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 5. Issues/Questions for Technical Advisory Board
  - No Issues and/or questions
  - Edwin/Danny: There has been unnecessay discussions within the companies. First discuss issues in project team before sharing them with the Technical Advisory Board
  - Marcel: We have to update Technical Advisory Board on (technical) progress 

## 6. Any Other Business
  - Marchien: Which decisions do we have to take in the steering committee
    - Erik: Discuss progress and next steps within steering committee and SEM board
    - Edwin: There is no relation between PoC and PSS because we are still in a technical PoC. There are still a lot of questions that need to be answered before implementing is in a live environment
    - Elias: Is everyone on the same page?
  - Edwin: Data duplication & Data fit for purpose > ACtions take place witin Iddink. Outcome will be shared later
  - Edwin: Is there a lastest version of the document "Moving from a chain to an ecosystem"? The version on Github contains remarks
    - Marcel: Version 3 (contains remarks) is the lastest version in posesion.
    - **Action**: Elias (Clifton) determine if there is a later version without remarks

# Actions:
 - Edwin will arrange SIS API session (Backlog Item 1)
    - Edwin will plan session on this subject in week 7 (19 February)
    - Jorim (Topicus) will be invited for the session
 - Danny will plan a meeting with Edwin, Clifton, Luke on this subject
    - 16 February (12:00 - 13:00)
 - Danny will update Marcel on planning
    - 16 February
 - Elias will update Marcel on planning
    - 17 February
 - Elias (Clifton) determine if there is a version of the document ("Moving from a chain to an ecosystem") without remarks
    - 26 February

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
 - Project team members check the use cases on correctness and integrality
 - Luke informs project team on the release of the SIS API
