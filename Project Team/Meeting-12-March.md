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
   - Design of the Progress & Results API is still open and will be dicussed in separate sesions - Design will be finished before the 1st of APril
     - Clifton will arrange meeting to finish designs
     - Progress & Results API will not be part of the PoC (only design)

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
     
     **Next week is important for the delivery of API's and sharing of credentials. So partners can start linking API's and start data exchange**   

## 5. Planning Test Phase
  - The coming two weeks will be needed to connect. After these weeks we can start testing

**After this a discussion started (free format):**
    - Edwin: For Iddink (Edwin) this is too much. "We have seen nothing yet"
      - There will be misfits (loose ends)
      - After PoC we only established a common ground to connect and communicatie. There is no integration with the backend > It is not a technical platform yet.
      - Integration in the application landscape is more difficult then the
  - Clifton: Been able to collaborate and and build the same things in the same way. Technical it's not very difficult, but it's a step
  - Danny: Could have done this (connection to Noordhoff and other partners) without this project
  - Marchien: It's not just these partners. It should be the base to connect with other prtners in the private sector
  - Edwin: Services were not needed at this point. We should have had more discussion first with members from the technical, functional and financial track first to establish a common ground/base
  - Erik: Our SIS API is nearly ready and we are going to use it
  - Elias: Not so worried about the technical side. It's more about getting schools on board based on the things we show and explain to them
  - Marcel: We have now have a technical design (base) to discuss with members of the functional and financial track
  
  - Danny: The board has to decide if we proceed with this or not
  - Marchien: The opinion of board members depend on the opinion of project team members. If you're positive it's more likely that that there will be a next phase
  - Danny: I think this is the right way to develop a new standard, but TLN has many projects. Others have to decide on the priority of this PoC within TLN
  
  - Marchien: Who do we need to convince in the next stage
  - Elias: Convincing schools will help the Board to decide to go on
  - Marcel: It's not only about the schools, but also to get more public and partners on board. We are not going to create a new standard that will be adopted if only TLN, Noordhoff, Topicus and Iddink join.
  
  - Clifton: It's not perfect, but is there an other altenarnative for private partners to be in charge of the change (the glass is half full)
  - Edwin: We are not at the point to involve schools

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
