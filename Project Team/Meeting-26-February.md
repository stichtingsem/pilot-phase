# Project Team Meeting

## Agenda
1. Opening
2. Notes 12 February
3. Actions
4. Progress Development & Planning
   - Scope
   - Progress
5. Planning Test Phase
6. Backlog Items project team
   - Questions
   - Updates
7. Issues/Questions for Technical Advisory Board
8. AOB

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
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-12-February.md)

## 3. Actions
 - Edwin will arrange SIS API session (Backlog Item 1)
     - Edwin will plan session on this subject in week 7 (19 February)
     - Jorim (Topicus) will be invited for the session
     - Pull request > Check by LAS parties if it is OK (master)
 - Elias (Clifton) determine if there is a version of the document ("Moving from a chain to an ecosystem") without remarks
     - 26 February


## 4.Progress Development & Planning
   - Scope
     - Marcel: In the Steering Committee we discussed the minimal scope of the proof of concept. If we want to demonstrate the ecosystem to reviewers and the SEM board we have to implement and test the API’s and connections. To make this possible we should at least:
        - Implement SIS, catalogue and entitlement API’s and the connections between these service for demonstration to reviewers and SEM Board
        - Finish API designs for usage, progress and results so we have all the designs in place to inform reviewers and the SEM Board
     - Edwin:
       - I miss the set-up and basic rules around events and bootstrap and usage is necessary for the first happy flow
       - And I have a question about de scope of entitlements do we want to support the two flows of only the flow to the LA?
       - Luke: I agree with Edwin on the need to determine what flows will have to be supported regarding the Entitlements API (i.e. are events mandatory or optional?)
  
   - TLN
     - MP: The Entitlement API is ready and is up and running in the acceptance environment.
     - LMS: Development will start in the first week of March. First expectation is that the LMS connections will be available around the 20th of March
     - Test: 
   
   - Noordhoff
     - LA: Working on the catalogue API, but there is no clarity on the release of this API
   
   - Iddink:
     - We started later but are still on schedule as previously stated. It will be exciting because unfortunately we do not yet have catalog data and that we are still determining the content of the dataset. But that is also part of the game. Our goal is to be ready April 1st. An integral happy flow test is planned for us after April 1. But let's see what we can do in parts in the meantime. 
     - Test SIS API SomToday:
   
   - SomToday
     - SIS: As Somtoday we are able to commit to the April 1st deadline for providing the SIS API. A first version of this API is already available in our testing environment and credentials have been provided to at least one MP.
     - LMS:As for the other parts (Entitlements API), where Somtoday (in the role of LMS) is acting as the client, it will depend on the (spec-finalization and) delivery of these API's by the servers (MP and LA). If this doesn't happen in the next couple of weeks we won't be able to deliver the client side of things on April 1st. 
   
   - Thieme
     - LA: Thieme will not join in this phase op the proof of concept

## 5. Planning Test Phase
  - 

## 6. Backlog Items project team

### Questions
- Luke: Also with regards to the finalization of the spec it's currently unclear to us if the API to support step 3.6 in [Use Case](https://github.com/stichtingsem/functionaloverview/blob/master/use-cases/oa.3.0-sales-agent-delivers-products.md is defined). The current entitlements API seems to concern the exchange of entitlements between MP and LA/LMS, but not between LA and LMS. Are we not looking in the right place or is this indeed an omission in the current specs?
  - Edwin: Proposal (mail)
- Jorn (Topicus) on 
   - Catalogue API Get/Products
     1. There is a start query parameter with default value, but that does not indicate the total amount of products. Can there be a total products added tot the response?
     2. The start parameter is 0 by default. This can be seen as a skip parameter. It could be that 0 and 1 have the same outcome. If the count starts with 0 this should be documented or is it better to change the description of the parameter?
     3. The product entity has no publisher information. This is a problem because we have products of multiple publishers in our catalog. Do we miss something or should this information be added to the response
  - Entitlement API
     1. The defaultaccessURL is part of the product information. This seems feasible for communication to the LMS, but not for the communication from MP to LA. Maybe we should ad documentation on conditional elements (required and not required)

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - **Action**: Edwin will plan session on this subject in week 7
  - Update:
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - Update:
    - [Issue](https://github.com/stichtingsem/pilot-phase/issues/1)
    - [Setups](https://github.com/stichtingsem/pilot-phase/blob/main/documents/Setups.xlsx)
    -   Update: 
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update: Pull request/branch is available in Github/Stoplight
     - Edwin has to check the design
     - Update: 
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
    - Update:
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update: 
13. Frontend for demonstration
  - Update:
3. Applicability OSR
  - Action holders: Marcel, Erik, (Edwin)
  - Update: [Report OSR 18 February](https://github.com/stichtingsem/pilot-phase/blob/main/documents/osr/20210218%20Gespreksverslag%20vervolgsessie%20OSR.pptx)
    - Development of connections between two partners is on the roadmap
    - They want use cases from the SEM Proof of Concept to determine if they can provide the right functionality in OSR for a central register
    - Next meeting: June 2021
4. Applicability RIO
  - Action holders: Marcel, Erik, (Edwin)
  - Update: [Report RIO 22 February](https://github.com/stichtingsem/pilot-phase/blob/main/documents/rio/20210222%20Gespreksverslag%20vervolgsessie%20RIO.pptx)
    - Applicable: [Onderwijsdata](https://onderwijsdata.duo.nl)
      - Data secondary Education will be added in 2021
      - Applicability can be possible in the next phase of the SEM environment
    - Not applicable: [Linked Open Data](https://lod.onderwijsregistratie.nl/restful-api)
    - Next meeting: June 2021

## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 7. Issues/Questions for Technical Advisory Board
  - 

## 8. Any Other Business
  - 


# Project Team Decisions:
 - The Usage API will **not** be renamed to consumption API
 - Partners in the ecosystem are responsible (based on role(s)) for their own front-end/interface to demonstrate functionality
 - Setups:
    - Client ID can be used for multiple services
    - During PoC no central registration like OSR
    - Setup will be done at DigiDelivery Id level. Multiple DigiDeliveryID for one school = multiple setups

# Completed Backlog Items:
7. Adjust design Entitlement API (and or either regarding school and individual)
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)
10. Adjust design Catalogue (add stream codes)
  - Conclusion: Stream codes will stay part of the design
11. Determine non happy flows/test scenario's (including returns & cancelations)

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
