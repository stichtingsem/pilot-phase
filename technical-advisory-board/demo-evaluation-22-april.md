## Technical Advisory Board - 22 April (17:00 - 18:00)

### Demo
- TLN:
  - Build the API’s and connections based on the SEM architecture in Github/Stoplight.
  - Tested the API’s and connections in their own internal environment with success
  - Started connecting to the SIS API’s of Topicus and Iddink
  - Topicus: Issue in receiving and processing the data
  - Iddink: There is a connection, but after the first message there is no data in the message
  - Danny will contact Jorim and Kees to solve the issues to bring the connections a step further (creating entitlements for the Learning Application and Learning Management System)
  - TLN will not demo (based on internal environment) because they’ve been working on fixing the connection with Iddink
- Topicus:
  - There is not much progress to show because there are no connections with the API’s of the other companies
    - Topicus wants to move further but depends on availability of the other companies
  - Jorim demos the parts that he can show
    - SIS API that shares groups, subjects and students
    - Connection to the market places for entitlement, but receives errors because there are no working connections
- Iddink:
  - Iddink is working with Noordhoff, Topicus and TLN to bring connections further so the demo will contain a full circle and participation of all the companies
    - Connecting to Topicus to deliver entitlement
    - Connecting to TLN for sharing SIS data and receiving entitlement data
    - Receives catalogue data from and working on the processing of usage data (Noordhoff)
  - Kees demos the API’s and connections between the roles that Iddink fulfils. In the receiving of catalogue and usage data he also shows the Noordhoff environment. Henk talks through these parts of the demo.
- Noordhoff
  - Noordhoff delivered a new version of the events and webhooks which other companies can connect to
  - Catalogue API is linked to Iddink and waiting for others to connect
  - Connection to usage API is tested by Iddink
- Conclusion/Next step
  - Some progress is made in comparison with the demo in the project team two weeks ago, but not as much as expected/hoped
  - There would be a demo in the steering committee tomorrow (23 April), but participants commit to make progress in the coming week so there is more to demo in the steering committee on the 30th of April
  - Participants will make time available to help other companies to make progress. This is supported by the CTO’s
  - Henk (Noordhoff) will not be available next week (holiday)
    - Clifton and Henk will discuss what is possible during the absence of Henk
  - Marcel will inform Marchien that demo will be rescheduled to the next meeting of the steering committee

Marcel thanks Kees, Edwin, Jorim, Danny and Henk for the demo and information. They leave the meeting.

The demo is recorded

### Evaluation

In the last meeting the CTO’s started to look back on the progress made during the PoC and possible next steps. The CTO’s give their (new) insights based on the demo and input from their company.

- Marcel (introduction):
  - Last time there was a positive view on the progress made
  - Steps after the PoC:
    - Have a meeting (4 hours) with the technical group to formalize designs and architecture (clean up and clear loose ends)
      - Finish progress & results API
    - Bring documentation to a next level so it can be shared with new partcipants
      - Hire (SME) somebody to help with the technical and functional documentation
    - Prepare for the next phase by organizing sessions
      - CTO’s
      - Tracks (Functional, Technical and Administrative)
- Edwin:
  - Good to see that we what we have achieved during this technical PoC phase
    - Maybe not were we wanted to be, but there is a technical base for further steps
  - Next Steps:
    - Round up the technical designs
      - Events and webhooks (bootstrap)
      - Setups/Consent flow
      - Progress & Results API
    - Involve schools (as soon as possible)
    - Finish documentation
      - Make it smart so it can be shared with new participants
    - Get involvement of more (SEM) partners > explain what we are doing
    - Involve Edu-K (public)
      - Marcel: Is integration of the API’s a (possible) next step?
        - The presented demo will be shown to the management of Iddink to discuss if they will start to integrate the API’s
        - Edwin will inform SEM about the outcome of this discussion
- Clifton:
  - Possitive about the progress made and confirms the introduction at the start of the evaluation
  - Instead of ‘talking a lot’ we ‘did a lot’
- Erik:
  - Suggests to make a split in the next phase > Working on the integration of the API’s in the backend, but also involve schools to validate what is build
    - Examples: consent and setups
  - Has convidence that the connections will work even if the demo doesn’t show this at the moment
- Jannes
  - Agrees with the other CTO’s
    - Focus on finishing technical designs and documentation as preparation for the next phase
  - He would like (as mentioned in the last meeting) to discuss the scope and goals for the next phase within this group (physical meeting)
- Albert
  - Underlines the comments that are made
  - There should be focus on documentation, but not only on the technical part of it. It should be clear for smaller companies what our goals are with the ecosystem. They have less technical knowhow then the participating companies.
    - There was an example after the broader update session that confirms this aspect
