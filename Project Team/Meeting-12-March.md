# Project Team Meeting

## Agenda
1. Opening
2. Notes 26 February
3. Actions
4. Progress Development & Planning
5. Planning Test Phase
6. Backlog Items project team
7. Issues/Questions for Technical Advisory Board
8. AOB

## Summary:
- Actions
- Project Team Decisions
- Completed Backlog Items
- Completed Actions

## 1. Opening
 - Additional agenda points
   - No agenda points added
 - Remarks
   - Meeting of last Monday (8 March) was succesfull (see Github). A lot of the outstanding were discussed and closed
   - Design of the Progress & Results API is still open and will be dicussed in separate sesions - Design will be finished before the 1st of April
     - Clifton will arrange meeting to finish designs
     - Progress & Results API will not be part of the PoC (only design)
   - There is a recurring meeting planned on monday (11:00 - 15:00) where developers and engineers can align with each other

## 2. Notes 26 February
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-26-February.md)
   - There were no remarks on the notes and are thereby approved

## 3. Actions
 -  Discuss contents of the entitlement API (MP > LMS)
      - Closed during meeting 8 March
 - Questions Topicus (Jorn) will be discussed by the technical group
      - Closed during meeting 8 March
 - Finish designs (API's, setup, events)
      - Closed during meeting 8 March
 - Share remarks on picture of connections with Edwin
      - Closed
 - Determine use cases to share with Kennisnet (OSR)
      - Marcel > Share use cases with project team
        - 19 March

## 4.Progress Development & Planning
        
   - TLN
     - Entitlement API: Finalise API on Monday 14 March
     - LMS: Work in Progress > Will be finished before the 1st of April
   
   - Noordhoff
     - Catalogue API: Authentication will be added to the catalogue API. Release at the start of next week
     - Usage API: API is created and will be avaliable at the start of next week
     - Connected to SIS endpoint Topicus
   
   - Iddink:
     - Finish development & deployment of API's and then make connections to external API's
   
   - SomToday
     - Noordhoff/Infinitas Learning is connected to SIS API
     - Iddink has credentials to SIS API > One bug in the SIS API has to be resolved
     - Start with development of connection to entitlement API (TLN) next week
       -  TLN (Hessel) can get credentials. If they are not shared yet, then they will be shared next monday
     
     **Next week is important for the delivery of API's and sharing of credentials so partners can start linking API's and start data exchange**   

## 5. Planning Test Phase
  - The coming two weeks will be needed to connect. After these weeks we can start testing

**After this a discussion started (free format)**

To summarize it:
Looking ahead the SEM board meeting of the March 16Th we had a discussion on the opinion of the project team members regarding the status of the PoC. The conclusion is that the project team is not completely aligned.
You could look at it from different angels, the glass is half full or half empty. What has been done technically is not very difficult, but we have moved further down the road. If we as private partners want to be in the lead of the development of a new system, there is only one way and that is forward
We deliberately decided after the first phase that although we still had open ends and issues to develop the technical base to go back to functional and administrative thereafter.
There is agreement on the fact that we established a common ground with each other to connect and communicate technically, although most members think we still need to have more discussion with members of financial and administrivia track to establish a broader understanding of what has to be done.
The project team is aware of the fact that there is still a gap to close before we have reached the phase that we can involve school in a Pilot. On the other hand we have to convince schools as well as other Public partners that we are on the right track. If and how we go forward depends on the opinion of the Board members.

## 6. Backlog Items project team

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - Update: Closed during meeting 8 March

2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - [Issue](https://github.com/stichtingsem/pilot-phase/issues/1)
  - [Setups](https://github.com/stichtingsem/pilot-phase/blob/main/documents/Setups.xlsx)
    - Update: Closed during meeting 8 March
   
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update: Closed during meeting 8 March


6. Design Results & Progress API (LMS)
  - Action Holders: Clifton, Danny, Edwin
  - [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
  - Update:
   	- **Action:** Will be discussed in seperate meetings which Clifton will arrange
    - Design will be finished before 1st of April

8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update: Closed during meeting 8 March

3. Applicability OSR
  - Action holders: Marcel, Erik, (Edwin)
   - Update:
    - **Action**: Determine use cases to share with Kennisnet (OSR)
      - Marcel > 19 March

## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 7. Issues/Questions for Technical Advisory Board
  - No queations/issues to share

## 8. Any Other Business
  - Slack channel available for credentials etc (CC to invite those without slack)


# Action

 - Arrange seperate meeting to finalize progress & results API
      - Clifton
      - 19 March
 - Determine use cases to share with Kennisnet (OSR) > First share with Project group for validation
      - Marcel
      - 19 March 

# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality
 - Setups:
    - Client ID can be used for multiple services
    - During PoC no central registration like OSR
    - Setup will be done at DigiDelivery Id level. Multiple DigiDeliveryID for one school = multiple setups

# Completed Backlog Items:
4. Applicability RIO
7. Adjust design Entitlement API (and or either regarding school and individual)
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
