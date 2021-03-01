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
   - No agenda points added
 - Remarks
   - No opening remarks

## 2. Notes 29 janaury
- [Notes](https://github.com/stichtingsem/pilot-phase/blob/main/Project%20Team/Meeting-12-February.md)
   - There were no remarks on the notes and are thereby approved

## 3. Actions
 - Edwin will arrange SIS API session (Backlog Item 1)
     - Meeting took place and there will be a follow up meeting
     - Kees (Iddink Group) created a pull request for the SIS API which should be checked and approved by the LAS partners in the ecosystem
         - Luke mentioned that Jorim was attending the meeting and the changes will be developed in their SIS API
 - Elias (Clifton) determine if there is a version of the document ("Moving from a chain to an ecosystem") without remarks
     - Clifton searched during the meeting and found version 2. Marcel found version 3 on Github. Both versions contain remarks of partners in the ecosystem.
         - Version 3 will be the base version for further purpose [Document](https://github.com/stichtingsem/pilot-phase/blob/main/sBDL%20-%20Moving%20from%20a%20Chain%20to%20an%20Ecosystem%20-%20v3.docx)

## 4.Progress Development & Planning
   
### Proposed Scope Steering Committee (1 April)
   - Implement SIS, catalogue and entitlement API’s and the connections between these service for demonstration to reviewers and SEM Board
   - Finish API designs for usage, progress & results so we have all the designs in place to inform reviewers and the SEM Board
      - Edwin:
         - I miss the set-up and basic rules around events and bootstrap and usage is necessary for the first happy flow
           - Usage is crucial for the processes of the Market Place
      - Clifton:
         - Not sure about bootstrap (events) and usage being part of the minimal scope of demonstration of the proof of concept
           - Designs should be completed in this phase
      - Elias:
           - We have difficulties getting things done as planned. Is usage really necessary to show the (basic) functionality of the ecosystem. I think that's not the case
      - Marcel:
         - Is it possible to have a working environment on the 1st of April?
            - Deliver and link API's during the second half of March
      - Edwin:
         - What do we need to "show" in April?
            - Marcel: Basic functionality of the ecosystem (SIS, Catalogue, Entitle, Access to content)
         - We are waiting on the Catalogue API for further testing
         - I'm going to escalate this internally, because developers could also do other things (new school year)
         - Maybe we could work with a smaller group on finishing technical designs and validate progress by functional/financial experts
      - Luke:
         - Topicus can commit to the Proof of Comcept till the 1st of April. After that we have to work on changes to facilitate the third exam time frame
         - Agree with Clifton on usage API not being part of the minimal scope (but we are not an MP)
         - Entitlement is crucial and should be part of the scope for the 1st of April
      - Hessel:
         - Agrees with Edwin on availibitlity of the catalogue API and the fact that usage API should be in scope
         - Explanation of Clifton might change opinion
      - Clifton:
         - We will discuss (Clifton, Elias, Henk) progress internally and look at ways to speed up the development of:
            - 1. catalogue API
            - 2. connection to entitlment API
            - 3. Usage API      
      
      **Actions**:
      - Luke, Elias/Clifton, Edwin, Hessel: Inform members of the Steering Committee on the progress of the SEM PoC. Determine position/opinion for the next Steering Committee (5 March)
      - Marcel: Update sheet for Steering Committee (5 March)
      
### Discussion Entitlement API   
   - Edwin:
       - I have a question about de scope of entitlements do we want to support the two flows of only the flow to the LA?
   - Luke:
       - I agree with Edwin on the need to determine what flows will have to be supported regarding the Entitlements API (i.e. are events mandatory or optional?)
   - There was a technical/functional discussion on the data that should be exchanged betwtween MP and LMS (entitlement API)
      - Should the Default Access URL and title of a product be shared within the Entitlement API?
      - This question will be discussed in the next technical meeting
    
   **Action**: Discuss contents of the entitlement API (MP > LMS)   
      
### Progress  
   - TLN
     - MP: The Entitlement API is ready and is up and running in the acceptance environment. Wotrking with a stub for catalgue data.
         - Partners can ask for credentials to setup connection
     - LMS: Development will start in the first week of March. First expectation is that the LMS connections will be available around the 20th of March
     - Test: Hessel could not yet test with SIS API of SomToday because of an issue
   
   - Noordhoff
     - LA: Working on the catalogue API, but there is no clarity on the release of this API yet
         - See earlier remarks on progress  
   
   - Iddink:
     - Consent and authorisation in place for all services
     - MP services working on SIS integration
     - Working on catalogue internally > Waiting catalogue API Noordhoff
     - Entitlement service partly ready (not deployed)
     - Next sprint -> acceptance environment
     - An integral happy flow test is planned for us after April 1. But let's see what we can do in parts in the meantime. 
   
   - SomToday
     - SIS API available but not aware of any issues
         - Luke will ask Jorim for more information on the issue
         - Wouter is talking with Kees (Iddink) about some flows 
     - Don’t need to implement Catalogue API
         - Edwin: Entitlement from Iddink will only contain EAN (No access location unknown) > Data at the source (Catalogue API)
            - To be discussed in technical meeting
            - Implementing Catalogue gives more option
      - Looking at Entitlement API (what should we do as an LMS to use it
   
   - Thieme
     - They will not participate in this phase op the proof of concept

## 5. Planning Test Phase
  - Agenda point will be moved to the next meeting when more is clear about progress

## 6. Backlog Items project team

### Questions
- Luke:
   - Question in email: Also with regards to the finalization of the spec it's currently unclear to us if the API to support step 3.6 in [Use Case](https://github.com/stichtingsem/functionaloverview/blob/master/use-cases/oa.3.0-sales-agent-delivers-products.md is defined). The current entitlements API seems to concern the exchange of entitlements between MP and LA/LMS, but not between LA and LMS. Are we not looking in the right place or is this indeed an omission in the current specs?
  - Tbd with the team: looks as if we have to implement Catalogue API
- Jorn (Topicus) on 
   - Catalogue API Get/Products
     1. There is a start query parameter with default value, but that does not indicate the total amount of products. Can there be a total products added tot the response?
     2. The start parameter is 0 by default. This can be seen as a skip parameter. It could be that 0 and 1 have the same outcome. If the count starts with 0 this should be documented or is it better to change the description of the parameter?
     3. The product entity has no publisher information. This is a problem because we have products of multiple publishers in our catalog. Do we miss something or should this information be added to the response
     - See [Issue](https://github.com/stichtingsem/pilot-phase/issues/17) 
  - Entitlement API
     1. The defaultaccessURL is part of the product information. This seems feasible for communication to the LMS, but not for the communication from MP to LA. Maybe we should ad documentation on conditional elements (required and not required)
     - See [Issue](https://github.com/stichtingsem/pilot-phase/issues/3)

 **Action**: Questions Topicus (Jorn) will be discussed by the tchnical group

### Update Backlog Items:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - [Questions Topicus](https://github.com/stichtingsem/pilot-phase/issues/4#issuecomment-753905214)
  - Update:
      - Pull request Kees available in Github/Stoplight for approval
      - Follow-up meeting is planned by Edwin
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - [Issue](https://github.com/stichtingsem/pilot-phase/issues/1)
  - [Setups](https://github.com/stichtingsem/pilot-phase/blob/main/documents/Setups.xlsx)
    - Update:
     - Part of discussions in the technical group
     - Wouter and Kees will meet on this issue next wednesday 
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Update:
     - Part of discussions in the technical group next tuesday
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwin, Clifton
  - [Issue & Reaction](https://github.com/stichtingsem/pilot-phase/issues/14)
  - Update:
     - Part of discussions in the technical group next tuesday
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton
  - Update:
     - Part of discussions in the technical group next tuesday
13. Frontend for demonstration
  - No updates
3. Applicability OSR
  - Action holders: Marcel, Erik, (Edwin)
  - Update: [Report OSR 18 February](https://github.com/stichtingsem/pilot-phase/blob/main/documents/osr/20210218%20Gespreksverslag%20vervolgsessie%20OSR.pptx)
    - Development of connections between two partners is on the roadmap
    - They want use cases from the SEM Proof of Concept to determine if they can provide the right functionality in OSR for a central register
    - Next meeting: June 2021

**Action**: Marcel will determine use cases to share with Kennisnet > First share with Project group for validation

4. Applicability RIO
  - Action holders: Marcel, Erik, (Edwin)
  - Update: [Report RIO 22 February](https://github.com/stichtingsem/pilot-phase/blob/main/documents/rio/20210222%20Gespreksverslag%20vervolgsessie%20RIO.pptx)
    - Applicable: [Onderwijsdata](https://onderwijsdata.duo.nl)
      - Data secondary Education will be added in 2021
      - Applicability can be possible in the next phase of the SEM environment
    - Not applicable: [Linked Open Data](https://lod.onderwijsregistratie.nl/restful-api)
    - Next meeting: June 2021
  - Edwin: First use PSS data and later implement RIO 

## Other Backlog Items:
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker), Edwin
  - Planning: After POC phase

## 7. Issues/Questions for Technical Advisory Board
  - No questions/issues for the Technical Advisory Board

## 8. Any Other Business
  - Edwin: Picture of the connections within the ecosystem. Does everybody agree on this setup?
      - **Action**: All Send remarks to Edwin
  - Hessel: Can we add colours to the connections to determine what is ready or not?
      - Marcel will share this 


# Actions:
 - Inform members of the Steering Committee on the progress of the SEM PoC. Determine position/opinion for the next Steering Committee
      - Luke, Elias/Clifton, Edwin, Hessel
      - 5 March
 - Update sheet for Steering Committee
      - Marcel
      - 5 March
 - Discuss contents of the entitlement API (MP > LMS)
      - Edwin, Clifton, Luke, Danny
      - 2 March
 - Questions Topicus (Jorn) will be discussed by the technical group
      - Edwin, Clifton, Luke, Danny
      - 2 March
 - Finish designs (API's, setup, events)
      - Edwin, Clifton, Luke, Danny
      - TBD
 - Share remarks on picture of connections with Edwin
      - All
      - 5 March   
 - Determine use cases to share with Kennisnet (OSR) > First share with Project group for validation
      - Marcel
      - 11 March 

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
 - Edwin will plan session on SIS API in week 7
 - Elias (Clifton) determine if there is a version of the document ("Moving from a chain to an ecosystem") without remarks
