# Project Team Meeting

## Agenda
1. Opening
2. Project team meetings - Planning & Content
3. Collaboration POC teams
4. Backlog Items project team
5. AOB

## 1. Opening
- Additional agenda points
   - No additional agenda points
- Remarks
   - No remarks

## 2.Project team meetings - Planning & Content

### Proposal
- Planning: **Approved by project team**
   - Every two weeks on friday from 14:00 till 15:00
   - Next meetings:
      - 18 December
      - 15 January
      - 29 january
      - 12 February
      - 26 February
- Content: **Approved by project team**
    - Report progress API development
    - Discuss development issues within the participating companies
    - Discuss progress on backlog items

## 3. Collaboration POC teams

### Approach development phase - Proposal
- **Goal: Develop API's based on the design in [spotlight](https://stichtingsem.stoplight.io/) and be ready (end of January) to link them to the other roles based on the POC scenarios**
   - TLN
     - MP almost ready
     - LMS development in January > expect to be ready by end of January
   - Noordhoff
     - LA: No problem to have API's ready by the end of January, but will check with developers
   - Iddink
     - MP, LMS, LA: Development will start second half of January. End of January is to ambitious
   - SomToday
     - Started with SIS. Development Authorization and LMS will start in January
     - Luke expects that LMS/ELO will be integrated in February
   - Progress will be monitored in project team meetings
- Every Project team member is responsible for the development of API's in their own company
    - Edwin: Iddink (MP), Magister (SIS/LMS)
    - Erik or Luke: SomToday (SIS/LMS)
    - Elias: Noordhoff (LA)
    - Danny: TLN (MP/LMS)
    - There is no definitive GO from Thieme (LA). 
      - **Question to Luke/Erik**: If Thieme participates could you follow/report progress?
      - Luke: If Thieme joins we (Luke/Erik) will monitor and report progress
- POC team leads/Development teams are responsible for the use cases needed to develop the API's
- Scope:
   - Prove that the API's work in the determined POC scenarios
   - It has to be clear for non technical people (just a command line with 200 (OK) is not enough)
      - Share outcome with mock up front end
   - We have demo the procesess based on testscenarios to prove the processes work within the ecosystem
      - Order an product
      - Deliver product
      - Access product
      - Use product
   - Action: Marcel will make a first version of the functional test scenarios and will share this with Edwin (Jerry), Danny (Hessel) and Elias

## 4. Backlog Items project team

### Actions & Principles:
1. Refine scopes SIS API
  - Action holders: Edwin (Kees), Clifton
  - Planning: Update 18 December
2. Design setup service
  - Action holders: Erik/Luke, Clifton
  - Planning: Update 18 December
3. Applicability OSR
  - Action holders: Marcel, Erik, Edwin
  - Planning: Folluw up meeting during POC
4. Applicability RIO
  - Action holders: Marcel, Erik, Edwin
  - Planning: Folluw up meeting during POC
5. Design Usage API (MP)
  - Action Holders: Danny, Clifton
  - Planning: Update 18 December
6. Design Results & Progress API (LMS)
  - Action Holders: Danny, Edwim, Clifton
  - Planning: Update 18 December
7. Adjust design Entitlement API (and or either)
  - Action holder: Clifton **ELias will share this with Clifton**
  - Planning: Update 18 December
8. Adjust design Entitlment API (Add operation: Get all entitlements for a specific individual)
  - Action holder: Danny, Clifton **ELias will share this with Clifton**
  - Planning: Update 18 December
9. Match Catalogue API on ECK 2.3/2.4 (mandatory fields)
  - Action holder: Danny, Edwin, Clifton **ELias will share this with Clifton**
  - Planning: Update 18 December
10. Adjust design Catalogue (add stream codes)
  - Action holder: Edwin (Kees), Danny
  - Planning: Update 18 December
11. FUNCTIONAL: Determine non happy flows/test scenario's (including returns & cancelations)
  - Action holders: Marcel, Edwin (Jerry), Danny (Hessel), Elias
  - Planning: During development phase
12. Check Data Covenant & Attribute Policy
  - Action holder: Marcel, Danny (Marten Bakker)
  - Planning: After POC phase

### Basic Principles & starting points
- Exchange as little data as possible
- API provider is accountable to deliver correct and actual data
- Identifiers
  - User: ECK iD
  - Organization: DigiDeliveryID
  - Product: EAN
  - Market Place: URL

## 5. Any Other Business
- Danny: Technical Alignment during development is key to align parties. Danny will discuss this with Clifton and Edwin
- Elias: Teams that are ready can start developing a common frontend for demo purposes
