<a href="http://www.spkaa.com"> 
<img src="http://i.imgur.com/EanML13.gif" height="110" width="220" align="right" title="www.spkaa.com"/> 

# RFI # CDT–ADPQ–0117 

> Prototype Submission for Agile Pre-Qualified Vendor Pool - California Department of Technology 

Prototype B Selected: California Emergency Notification Web Portal 

###URL:  [[SPK Submission Prototype]](https://github.com/calmeida81/CarlosADPQ) 


## About SPK and Associates
 Founded in 1997 with corporate office in Los Gatos, CA, SPK is Technology Services Company completely focused on fulfilling the specialized needs of R&D or Engineering groups.  Rather than providing generic IT services like many other IT Services companies, we decided that we would become absolutely great at understanding the business of R&D.  Then, we translate that into tech services designed to speed up product design and release while improving your product quality.    We operate in highly regulated verticals such as Medical Device, Financial and Automotive.  We specialized in Agile development techniques while maintaining rigorous discipline required for auditors and regulators.

 We are a Certified Woman-Owned Business Enterprize (WBENC)
<img src="http://i.imgur.com/W9rZqZX.jpg" height="100" width="200" align="right" />

### Attachment [B-PQVP-DS-AD-Vendor Profile](https://github.com/calmeida81/CarlosADPQ/blob/master/Attachment-B_PQVP-DS-AD-Vendor_Profile-SPK.pdf )

 
## Technical Approach

 
This project contains 4 Sprints timeboxed within 3-5 days each.  Each sprint contains defined content deliverables/features, and testcases.  

Usecases drive overall requirements. Peer review and external non developer review are done per sprint.  This application will run on Android Mobile Devices and Chrome Browsers other devices.

**Tools Used** 

- [Usecase Development (ADPQ-Use_Case_Specifications-SPK.pdf) ](https://github.com/calmeida81/CarlosADPQ/blob/master/ADPQ-Use_Case_Specifications-SPK.pdf) - Done via  Usecase Visual Studio.  
- [Website Mockups  (ADPQ_Mockups-SPK.pdf) ](https://github.com/calmeida81/CarlosADPQ/blob/master/ADPQ_Mockups-SPK.pdf) - Done via  Balsamiq.  
- [Requirements Management/Traceability (ADPQ_RequirementsToTestTraceabilityMatrix-SPK.pdf) ](https://github.com/calmeida81/CarlosADPQ/blob/master/ADPQ_RequirementsToTestTraceabilityMatrix-SPK.pdf) - Done via PTC Integrity Requirements Manager.   
- [Configuration Management](https://github.com/calmeida81/CarlosADPQ) - Done Via Git
- [Continuous Integration (ADPQ_ContinuousIntegrationModelDescription-SPK.pdf) ](https://github.com/calmeida81/CarlosADPQ/blob/master/ADPQ-ContinuousIntegrationModelDescription-SPK.pdf) - Done via Electric Cloud's ElectricFlow
- [Interactive Testing (ADPQ_SampleTestSession-SPK.pdf) ](https://github.com/calmeida81/CarlosADPQ/blob/master/ADPQ_SampleTestSession-SPK.pdf) - Done via PTC Integrity Test Manager.
- Unit Testing - Done with Junit
- Webapp Testing - Done with Mocha
- [Restful API Documentation (URL Link to Swagger API) ](https://github.com/calmeida81/CarlosADPQ/blob/master/api-docs.json) - Done via Swagger
- Project Management and Collaboration - Done Via Confluence
- Bug Tracking - Done Via Jira
- Deployment - Done Via Docker
- Android Development - Done Via Android Studio SDK environment
  
**Project Architectural Elements Used**

- Node JS: Server control
- Angular JS: Client control
- MongoDB: Database
- Android SDK: Android app

**Project Architectural Libraries Used**

- Bootstrap: Responsive UI and styling
- Twilio: Messaging
- Mocha: Unit testing in web
- Nodemailer: Emailing
- Google Maps: Geolocation
- D3: Web visualization


**Core Architectural Flow**

This system consists of two parts. The first is a Node.js webapp written with Express. The second is an Android app written primarily in Java. When a user opens the webapp, they are presented with a splash screen and asked to either login or sign up. When they do, their data is pulled or pushed from a locally running MongoDB database, using Mongoose. The user is then presented with a dashboard screen, which differs depending on whether they are an admin or a user. As an admin, visualization data is presented to them using the d3 javascript library. They are also able to select which data will be sent and to the users via socket connections. Users are able to select their preferences and alter their profiles, both of which are saved in the local database.

When a user opens the Android app, they are similarly presented with a login splash screen. This portion of the app pulls from the webapp database. At the main dashboard screen, the user is able to view data sent by the webapp and alter their profiles. This data is also sent via socket connections. When users receive notifications, they will see them via sockets and push for the app, email with Nodemailer, and sms with twilio.



## Sprint Content

**Sprint 1**

- Define Usecases and Requirements
- Define Mockups/Wireframes
- Define Tools
- Define Architecture
- Define CI Methodology
- Define Release Methodology
- Produce Requirements -> Design Specifications -> Testcases Traceabiliy Matrix
- Dev Code and Tests for **User Login/Profile Usecases****/Requirements**
- Release Sprint 1 for Internal Review
- Release Sprint 1 External Review
- Sprint 1 Retrospective

**Sprint 2**

- Dev Code and Tests for **Alert/Messaging Usecases/Requirements**
- Release Sprint 2 for Internal Review
- Release Sprint 2 External Review
- Sprint 2 Retrospective

**Sprint 3**

- Dev Code and Tests for **Administrative Usecases/Requirements**
- Release Sprint 3 for Internal Review
- Release Sprint 3 External Review
- Sprint 3 Retrospective

**Sprint 4**

- Dev Code and Tests for **Visualization Usecases/Requirements**
- Release Sprint 4 for Internal Review
- Release Sprint 4 External Review
- Sprint 4 Retrospective

## Installation

**Android Mobile Devices**

[Describe How User installs application on Android Devices]

**Other Devices Utilize Chrome Browser**

[Describe How User installs application on Other Devices Utilize Chrome Browser]

## SPK Project Team

- Team Leader:	Carlos Almeida
- Developer:	Joshua Kling
- Developer:	David Hubbell
- QA:	Steve Lundy
- External Non Team Reviewer:	Colin Doyle


## License


This prototype is intended to a be *sample* of an Agile Development project.  Requirements/Features/Usecases and Test Coverage are not comprehensive.  This prototype not intended for production.
