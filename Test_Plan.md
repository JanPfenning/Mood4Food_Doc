
- [1. Introduction](#1-introduction)
  * [1.1 Purpose](#11-purpose)
  * [1.2 Scope](#12-scope)
  * [1.3 Intended Audience](#13-intended-audience)
  * [1.4 Document Terminology and Acronyms](#14-document-terminology-and-acronyms)
  * [1.5  References](#15--references)
  * [1.6 Document Structure](#16-document-structure)
- [2. Evaluation Mission and Test Motivation](#2-evaluation-mission-and-test-motivation)
  * [2.1 Background](#21-background)
  * [2.2 Evaluation Mission](#22-evaluation-mission)
  * [2.3 Test Motivators](#23-test-motivators)
- [3. Target Test Items](#3-target-test-items)
- [4. Outline of Planned Tests](#4-outline-of-planned-tests)
  * [4.1 Outline of Test Inclusions](#41-outline-of-test-inclusions)
  * [4.2 Outline of Other Candidates for Potential Inclusion](#42-outline-of-other-candidates-for-potential-inclusion)
  * [4.3 Outline of Test Exclusions](#43-outline-of-test-exclusions)
- [5. Test Approach](#5-test-approach)
  * [5.1 Initial Test-Idea Catalogs and Other Reference Sources](#51-initial-test-idea-catalogs-and-other-reference-sources)
  * [5.2 Testing Techniques and Types](#52-testing-techniques-and-types)
    + [5.2.1 Data and Database Integrity Testing](#521-data-and-database-integrity-testing)
    + [5.2.2 Functional Testing](#522-functional-testing)
    + [5.2.3 Business Cycle Testing](#523-business-cycle-testing)
    + [5.2.4 User Interface Testing](#524-user-interface-testing)
    + [5.2.5 Performance Profiling](#525-performance-profiling)
    + [5.2.6 Load Testing](#526-load-testing)
    + [5.2.7 Stress Testing](#527-stress-testing)
    + [5.2.8 Volume Testing](#528-volume-testing)
    + [5.2.9 Security and Access Control Testing](#529-security-and-access-control-testing)
    + [5.2.10 Failover and Recovery Testing](#5210-failover-and-recovery-testing)
    + [5.2.11 Configuration Testing](#5211-configuration-testing)
    + [5.2.12 Installation Testing](#5212-installation-testing)
    + [5.2.13 API Testing](#5212-api-testing)
- [6. Entry and Exit Criteria](#6-entry-and-exit-criteria)
  * [6.1 Test Plan](#61-test-plan)
    + [6.1.1 Test Plan Entry Criteria](#611-test-plan-entry-criteria)
    + [6.1.2 Test Plan Exit Criteria](#612-test-plan-exit-criteria)
    + [6.1.3 Suspension and Resumption Criteria](#613-suspension-and-resumption-criteria)
  * [6.2 Test Cycles](#62-test-cycles)
      - [6.2.1 Test Cycle Entry Criteria](#621-test-cycle-entry-criteria)
      - [6.2.2 Test Cycle Exit Criteria](#622-test-cycle-exit-criteria)
      - [6.2.3 Test Cycle Abnormal Termination](#623-test-cycle-abnormal-termination)
- [7. Deliverables](#7-deliverables)
- [7.1 Test Evaluation Summaries](#71-test-evaluation-summaries)
- [7.2 Reporting on Test Coverage](#72-reporting-on-test-coverage)
- [7.3 Perceived Quality Reports](#73-perceived-quality-reports)
- [7.4 Incident Logs and Change Requests](#74-incident-logs-and-change-requests)
- [7.5 Smoke Test Suite and Supporting Test Scripts](#75-smoke-test-suite-and-supporting-test-scripts)
- [7.6      Additional Work Products](#76------additional-work-products)
  * [7.6.1     Detailed Test Results](#761-----detailed-test-results)
  * [7.6.2     Additional Automated Functional Test Scripts](#762-----additional-automated-functional-test-scripts)
  * [7.6.3     Test Guidelines](#763-----test-guidelines)
  * [7.6.4     Traceability Matrices](#764-----traceability-matrices)
- [8. Testing Workflow](#8-testing-workflow)
- [9. Environmental Needs](#9-environmental-needs)
  * [9.1 Base System Hardware](#91-base-system-hardware)
  * [9.2 Base Software Elements in the Test Environment](#92-base-software-elements-in-the-test-environment)
  * [9.3 Productivity and Support Tools](#93-productivity-and-support-tools)
  * [9.4 Test Environment Configurations](#94-test-environment-configurations)
- [10. Responsibilities, Staffing, and Training Needs](#10-responsibilities--staffing--and-training-needs)
  * [10.1 People and Roles](#101-people-and-roles)
  * [10.2 Staffing and Training Needs](#102-staffing-and-training-needs)
- [11. Iteration Milestones](#11-iteration-milestones)
- [12. Risks, Dependencies, Assumptions, and Constraints](#12-risks--dependencies--assumptions--and-constraints)
- [13. Management Process and Procedures](#13-management-process-and-procedures)


## 1. Introduction

### 1.1 Purpose

The purpose of the Iteration Test Plan is to gather all of the information necessary to plan and control the test effort for a given iteration. It describes the approach to testing the software.
This Test Plan for Vaultionizer supports the following objectives:

- Identifies the items that should be targeted by the tests.
- Identifies the motivation for and ideas behind the test areas to be covered.
- Outlines the testing approach that will be used.
- Identifies the required resources and provides an estimate of the test efforts.

### 1.2 Scope

The areas of tests that are considered in document are:
* Unit-Tests (Functionality)
* .feature-Files for Gherkin (UI)
* API tests (Postman)
We do not include Usertests or Stresstests. We decided to base the userinterface on the basic principe of UI design. This can be seen when comparing our Navigation bar to the one of Instagram.
Stresstests are not really important because the Application is based on local storage for most of the functionality.

### 1.3 Intended Audience

The Testplan document is written for Internal Use and for the Professor that is grading us.
This document is not written for end-users

### 1.4 Document Terminology and Acronyms

| Abbr | Abbreviation                        |
|------|-------------------------------------|
| API  | Application Programmable Interface  |
| CI   | Continuous Integration              |
| CD   | Continuous Delivery/Deployment      |
| PR   | Pull Request                        |
| n/a  | not applicable                      |
| SRS  | Software Requirements Specification |
| tbd  | to be determined                    |
| UI   | User Interface                      |

### 1.5  References

| Title                                                                   | Date       | Publishing organization   |
| ------------------------------------------------------------------------|:----------:| ------------------------- |
| [Blog](https://md4fd.wordpress.com/blog/)                               | MAI. 2021  |      Mood4Food            |
| [DOC GitHub Repository](https://github.com/JanPfenning/Mood4Food_Doc)   | MAI. 2021  |      Mood4Food            |
| [API GitHub Repository](https://github.com/JanPfenning/Mood4Food_Api)   | MAI. 2021  |      Mood4Food            |
| [APP GitHub Repository](https://github.com/JanPfenning/Mood4Food)       | MAI. 2021  |      Mood4Food            |
| [UC AnalyzeWaterBalance](../UCS/UCS - AnalyzeWaterBalance.md)           | MAI. 2021  |      Mood4Food            |
| [UC CrudLocalRecipe](../UCS/UCS - CrudLocalRecipe.md)                   | MAI. 2021  |      Mood4Food            |
| [UC FavorizeRecipe](../UCS/UCS - FavorizeRecipe.md)                     | MAI. 2021  |      Mood4Food            |
| [UC GetHealthDemandInformation](../UCS/UCS - GetHealthDemandInformation.md)| MAI. 2021  |      Mood4Food            |
| [UC ManageSettings](../UCS/UCS - ManageSettings.md)                     | MAI. 2021  |      Mood4Food            |
| [UC ManageWaterBalance](../UCS/UCS - ManageWaterBalance.md)             | MAI. 2021  |      Mood4Food            |
| [UC RateIngredients](../UCS/UCS - RateIngredients.md)                   | MAI. 2021  |      Mood4Food            |
| [UC ViewApiRecipe](../UCS/UCS - ViewApiRecipe.md)                       | MAI. 2021  |      Mood4Food            |
| [UC ViewRecommendedRecipes](../UCS/UCS - ViewRecommendedRecipes.md)     | MAI. 2021  |      Mood4Food            |
| [Test Plan](./Test_Plan.md)                                              | MAI. 2021  |      Mood4Food            |
| [SRS](../Software_Requirements_Specification.md)                        | MAI. 2021  |      Mood4Food            |
| [SAD](../Software_Architecture_Documentation.md)                        | MAI. 2021  |      Mood4Food            |

### 1.6 Document Structure

See Table of Contents

## 2. Evaluation Mission and Test Motivation

### 2.1 Background

Testing serves to ensure that the written code does what it is intended to do. It also prevents future code changes to break existing functionality unnoticed. In the context of integration it can also prevent broken software states to be merged into secured VC branches.
For the sake of this, we also decided to never directly push to the Development- or Masterbranch. The Masterbranch can only be updated by merging the Developmentbranch. The Developmentbranch can only be updated by merging a feature branch, and that merge can only be processed if all tests pass and another developer approves it. 

### 2.2 Evaluation Mission

Our mission is to spot mistakes early on so they wont propagate while further developing. By doing this we make as sure as reasonable that users wont encouter strange behaviour.

### 2.3 Test Motivators

The motivation for us to test the software is to make refactoring tasks as short as possible and to spot mistakes in the moment of pushing so they will not be found in a productive version. We want to keep the quality as high as posible while risks are as low as possible.

## 3. Target Test Items

The listing below identifies those test items software, hardware, and supporting product elements that have been identified as targets for testing. This list represents what items will be tested.

* API endpoints
* Converter Classes
* Repositories
* Entities

## 4. Outline of Planned Tests

### 4.1 Outline of Test Inclusions

*Frontend: Android Client*:

- FeatureFiles
- JUnitTest

*Backend: PHP API*:

- Api testing (Postman)

![Testing overview](./testing_overview.png)  <!--TODO-->

The tests themself will not be tested and will not account into code coverage.
Neither will files that are basically only representation of the UI (Views)

### 4.2 Outline of Other Candidates for Potential Inclusion

(n/a)

### 4.3 Outline of Test Exclusions

[Provide a high level outline of the potential tests that might have been conducted, but that have been explicitly excluded from this plan. If a type of test will not be implemented and executed, indicate this in a sentence stating the test will not be implemented or executed, and stating the justification, such as:

- These tests do not help achieve the evaluation mission.:
  - Gherkin execution
  - Stresstests
  - Userinteraction tests

- These tests draw too much resources:
  - Security and Access Control Testing

## 5. Test Approach

<!--[The Test Approach presents the recommended strategy for designing and implementing the required tests. Sections 3, Target Test Items, and 4, Outline of Planned Tests, identified what items will be tested and what types of tests would be performed. This section describes how those tests will be realized.
One aspect to consider for the test approach is the techniques to be used. This should include an outline of how each technique can be implemented, both from a manual and/or an automated perspective, and the criterion for knowing that the technique is useful and successful. For each technique, provide a description of the technique and define why it is an important part of the test approach by briefly outlining how it helps achieve the Evaluation Mission or addresses the Test Motivators.
Another aspect to discuss in this section is the Fault or Failure models that are applicable and ways to approach evaluating them.
As you define each aspect of the approach, you should update section 10, Responsibilities, Staffing, and Training Needs, to document the test environment configuration and other resources that will be needed to implement each aspect.]-->

### 5.1 Initial Test-Idea Catalogs and Other Reference Sources

(n/a) 
<!--[Provide a listing of existing resources that will be referenced to stimulate the identification and selection of specific tests to be conducted. An example Test-Ideas Catalog is provided in the examples section of RUP.]-->

### 5.2 Testing Techniques and Types

#### 5.2.1 Data and Database Integrity Testing

(n/a)
<!--
[The databases and the database processes should be tested as an independent subsystem. This testing should test the subsystems without the target-of-test's User Interface as the interface to the data. Additional research into the DataBase Management System (DBMS) needs to be performed to identify the tools and techniques that may exist to support the testing identified in the following table.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    | [Exercise database access methods and processes independent of the UI so you can observe and log incorrectly functioning target behavior or data corruption.]                  |
|Technique              | [Invoke each database access method and process, seeding each with valid and invalid data or requests for data. Inspect the database to ensure the data has been populated as intended and all database events have occurred properly, or review the returned data to ensure that the correct data was retrieved for the correct reasons.]   |
|Oracles                | [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.] |
|Required Tools         | [The technique requires the following tools: Test Script Automation Tool; base configuration imager and restorer; backup and recovery tools; installation-monitoring tools (registry, hard disk, CPU, memory, and so on); database SQL utilities and tools; data-generation tools]                    |
|Success Criteria       | [The technique supports the testing of all key database access methods and processes.]    |
|Special Considerations | [Testing may require a DBMS development environment or drivers to enter or modify data directly in the database.; Processes should be invoked manually.; Small or minimally sized databases (with a limited number of records) should be used to increase the visibility of any non-acceptable events.] -->                                                                |

#### 5.2.2 Functional Testing

JUnit-Tests
<!--
[Function testing of the target-of-test should focus on any requirements for test that can be traced directly to use cases or business functions and business rules. The goals of these tests are to verify proper data acceptance, processing, and retrieval, and the appropriate implementation of the business rules. This type of testing is based upon black box techniques; that is, verifying the application and its internal processes by interacting with the application via the Graphical User Interface (GUI) and analyzing the output or results. The following table identifies an outline of the testing recommended for each application.]
-->
<!--Todo-->

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  The App should build and start. Several tests should be carried out to find our whether everything is working correctly  |
|Technique              |  All tests are executed by the JUnit Framework. Tests that need Data will be given Mock-Data  |
|Oracles                |  The Application reacts as described in the predefined Tests  |
|Required Tools         |  JUnit 4 |
|Success Criteria       |  Framework considers all Tests as Passed |
|Special Considerations |  -  |

#### 5.2.3 Business Cycle Testing

<!--[Business Cycle Testing should emulate the activities performed on the  Project Name  over time. A period should be identified, such as one year, and transactions and activities that would occur during a year's period should be executed. This includes all daily, weekly, and monthly cycles, and events that are date-sensitive, such as ticklers.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  [Exercise target-of-test and background processes according to required business models and schedules to observe and log target behavior.]   |
|Technique              |  [Testing will simulate several business cycles by performing the following:; The tests used for target-of-test's function testing will be modified or enhanced to increase the number of times each function is executed to simulate several different users over a specified period.; All time or date-sensitive functions will be executed using valid and invalid dates or time periods.; All functions that occur on a periodic schedule will be executed or launched at the appropriate time.; Testing will include using valid and invalid data to verify the following:; The expected results occur when valid data is used.;The appropriate error or warning messages are displayed when invalid data is used.;Each business rule is properly applied.]   |
|Oracles                |   [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made, and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]  |
|Required Tools         |   [The technique requires the following tools:; Test Script Automation Tool; base configuration imager and restorer; backup and recovery tools; data-generation tools]  |
|Success Criteria       |  [The technique supports the testing of all critical business cycles.]   |
|Special Considerations |   [System dates and events may require special support activities.; A business model is required to identify appropriate test requirements and procedures.]  |-->

#### 5.2.4 User Interface Testing

.feature-Files
<!--
[User Interface (UI) testing verifies a user's interaction with the software. The goal of UI testing is to ensure that the UI provides the user with the appropriate access and navigation through the functions of the target-of-test. In addition, UI testing ensures that the objects within the UI function as expected and conform to corporate, or industry, standards.]
-->
<!--TODO-->
|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  The application should react properly to Input actions   |
|Technique              |  .feature files contain a human readable step by step plan that is to be translated and executed by the Testframework  |
|Oracles                |  The Gherkin Framework considers all tests as passed (if the translation was implemented and tests where actually executed)   |
|Required Tools         |  Gherkin  |
|Success Criteria       |  All Tests have passed the Gherkin execution  |
|Special Considerations |  We only provided the .feature files with appropriate description. The translation from the human readable format to the Gherkin execution is not part of the scope  |

#### 5.2.5 Performance Profiling
(n/a)
<!--
[Performance profiling is a performance test in which response times, transaction rates, and other time-sensitive requirements are measured and evaluated. The goal of Performance Profiling is to verify performance requirements have been achieved. Performance profiling is implemented and executed to profile and tune a target-of-test's performance behaviors as a function of conditions, such as workload or hardware configurations.

Note: Transactions in the following table refer to "logical business transactions". These transactions are defined as specific use cases that an actor of the system is expected to perform using the target-of-test, such as add or modify a given contract.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |   [Exercise behaviors for designated functional transactions or business functions under the following conditions to observe and log target behavior and application performance data:; normal anticipated workload; anticipated worst-case workload]  |
|Technique              |   [Use Test Procedures developed for Function or Business Cycle Testing.; Modify data files to increase the number of transactions or the scripts to increase the number of iterations that occur in each transaction.; Scripts should be run on one machine (best case is to benchmark single user, single transaction) and should be repeated with multiple clients (virtual or actual, see Special Considerations below).]  |
|Oracles                |  	[Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]   |
|Required Tools         |   [The technique requires the following tools:; Test Script Automation Tool; an application performance profiling tool, such as Rational Quantify; installation-monitoring tools (registry, hard disk, CPU, memory, and so on; resourse-constraining tools; for example, Canned Heat]  |
|Success Criteria       |  [The technique supports testing:; Single Transaction or single user: Successful emulation of the transaction scripts without any failures due to test implementation problems.; Multiple transactions or multiple users: Successful emulation of the workload without any failures due to test implementation problems.]   |
|Special Considerations |  [Comprehensive performance testing includes having a background workload on the server.; There are several methods that can be used to perform this, including:; "Drive transactions" directly to the server, usually in the form of Structured Query Language (SQL) calls.; Create "virtual" user load to simulate many clients, usually several hundred. Remote Terminal Emulation tools are used to accomplish this load. This technique can also be used to load the network with "traffic".; Use multiple physical clients, each running test scripts, to place a load on the system.; Performance testing should be performed on a dedicated machine or at a dedicated time. This permits full control and accurate measurement.; The databases used for Performance Testing should be either actual size or scaled equally.]   |
-->

#### 5.2.6 Load Testing
(n/a)
<!--
[Load testing is a performance test that subjects the target-of-test to varying workloads to measure and evaluate the performance behaviors and abilities of the target-of-test to continue to function properly under these different workloads. The goal of load testing is to determine and ensure that the system functions properly beyond the expected maximum workload. Additionally, load testing evaluates the performance characteristics, such as response times, transaction rates, and other time-sensitive issues.

[Note: Transactions in the following table refer to "logical business transactions". These transactions are defined as specific functions that an end user of the system is expected to perform using the application, such as add or modify a given contract.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  [Exercise designated transactions or business cases under varying workload conditions to observe and log target behavior and system performance data.] |
|Technique              |  [Use Transaction Test Scripts developed for Function or Business Cycle Testing as a basis, but remember to remove unnecessary interactions and delays.; Modify data files to increase the number of transactions or the tests to increase the number of times each transaction occurs.; Workloads should include—for example, daily, weekly, and monthly—peak loads.; Workloads should represent both average as well as peak loads.; Workloads should represent both instantaneous and sustained peaks.; The workloads should be executed under different Test Environment Configurations.]   |
|Oracles                |  [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]   |
|Required Tools         |   [The technique requires the following tools:; Test Script Automation Tool; Transaction load scheduling and control tool; installation-monitoring tools (registry, hard disk, CPU, memory, and so on); resource-constraining tools; for example, Canned Heat; data-generation tools]  |
|Success Criteria       |  [The technique supports the testing of Workload Emulation, which is the successful emulation of the workload without any failures due to test implementation problems.]   |
|Special Considerations |  [Load testing should be performed on a dedicated machine or at a dedicated time. This permits full control and accurate measurement.; The databases used for load testing should be either actual size or scaled equally.]   |
-->

#### 5.2.7 Stress Testing
(n/a)
<!--
[Stress testing is a type of performance test implemented and executed to understand how a system fails due to conditions at the boundary, or outside of, the expected tolerances. This typically involves low resources or competition for resources. Low resource conditions reveal how the target-of-test fails that is not apparent under normal conditions. Other defects might result from competition for shared resources, like database locks or network bandwidth, although some of these tests are usually addressed under functional and load testing.

[Note: References to transactions in the following table refer to logical business transactions.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |   [Exercise the target-of-test functions under the following stress conditions to observe and log target behavior that identifies and documents the conditions under which the system fails to continue functioning properly:; little or no memory available on the server (RAM and persistent storage space); maximum actual or physically capable number of clients connected or simulated; multiple users performing the same transactions against the same data or accounts; "overload" transaction volume or mix (see Performance Profiling above)]  |
|Technique              |   [Use tests developed for Performance Profiling or Load Testing.; To test limited resources, tests should be run on a single machine, and RAM and persistent storage space on the server should be reduced or limited.; For remaining stress tests, multiple clients should be used, either running the same tests or complementary tests to produce the worst-case transaction volume or mix.]  |
|Oracles                |  [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]   |
|Required Tools         |  [The technique requires the following tools:; Test Script Automation Tool; Transaction load scheduling and control tool; installation-monitoring tools (registry, hard disk, CPU, memory, and so on; resource-constraining tools; for example, Canned Heat; data-generation tools]   |
|Success Criteria       |  [The technique supports the testing of Stress Emulation. The system can be emulated successfully in one or more conditions defined as stress conditions, and an observation of the resulting system state, during and after the condition has been emulated, can be captured.]   |
|Special Considerations |  [Stressing the network may require network tools to load the network with messages or packets.; The persistent storage used for the system should temporarily be reduced to restrict the available space for the database to grow.; Synchronize the simultaneous clients accessing of the same records or data accounts.]   |
-->

#### 5.2.8 Volume Testing
(n/a)
<!--
[Volume testing subjects the target-of-test to large amounts of data to determine if limits are reached that cause the software to fail. Volume testing also identifies the continuous maximum load or volume the target-of-test can handle for a given period. For example, if the target-of-test is processing a set of database records to generate a report, a Volume Test would use a large test database, and would check that the software behaved normally and produced the correct report.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  [Stressing the network may require network tools to load the network with messages or packets.; The persistent storage used for the system should temporarily be reduced to restrict the available space for the database to grow.; Synchronize the simultaneous clients accessing of the same records or data accounts.]   |
|Technique              |  [Use tests developed for Performance Profiling or Load Testing.; Multiple clients should be used, either running the same tests or complementary tests to produce the worst-case transaction volume or mix (see Stress Testing) for an extended period.; Maximum database size is created (actual, scaled, or filled with representative data), and multiple clients are used to run queries and report transactions simultaneously for extended periods.]]   |
|Oracles                |   [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]  |
|Required Tools         |   [The technique requires the following tools:; Test Script Automation Tool; Transaction load scheduling and control tool; installation-monitoring tools (registry, hard disk, CPU, memory, and so on; resource-constraining tools; for example, Canned Heat; data-generation tools]  |
|Success Criteria       |  	[The technique supports the testing of Volume Emulation. Large quantities of users, data, transactions, or other aspects of the system use under volume can be successfully emulated and an observation of the system state changes over the duration of the volume test can be captured.]   |
|Special Considerations |  [What period of time would be considered an acceptable time for high volume conditions, as noted above?]   |
-->

#### 5.2.9 Security and Access Control Testing

(n/a)
<!--
[Security and Access Control Testing focuses on two key areas of security:; Application-level security, including access to the Data or Business Functions; System-level Security, including logging into or remotely accessing to the system; Based on the security you want, application-level security ensures that actors are restricted to specific functions or use cases, or they are limited in the data that is available to them. For example, everyone may be permitted to enter data and create new accounts, but only managers can delete them. If there is security at the data level, testing ensures that "user type one" can see all customer information, including financial data, however, "user type two" only sees the demographic data for the same client.; System-level security ensures that only those users granted access to the system are capable of accessing the applications and only through the appropriate gateways.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  [Exercise the target-of-test under the following conditions to observe and log target behavior:; Application-level Security: an actor can access only those functions or data for which their user type is provided permissions.; System-level Security: only those actors with access to the system and applications are permitted to access them].   |
|Technique              |  [Application-level Security: Identify and list each user type and the functions or data for which each type has permissions.; Create tests for each user type and verify each permission by creating transactions specific to each user type.; Modify user type and rerun tests for same users. In each case, verify those additional functions or data are correctly available or denied.; System-level Access: See Special Considerations below.]   |
|Oracles                |  [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.] |
|Required Tools         |  [The technique requires the following tools:; Test Script Automation Tool; "Hacker" security breach and probing tools; OS Security Administration tools]   |
|Success Criteria       |  [The technique supports the testing of the appropriate functions or data affected by security settings can be tested for each known actor type.]   |
|Special Considerations |  [Access to the system must be reviewed or discussed with the appropriate network or systems administrator. This testing may not be required as it may be a function of network or systems administration.]   |
-->

#### 5.2.10 Failover and Recovery Testing
(n/a)
<!--
[Failover and recovery testing ensures that the target-of-test can successfully failover and recover from a variety of hardware, software, or network malfunctions with undue loss of data or data integrity.

[For those systems that must be kept running, failover testing ensures that when a failover condition occurs, the alternate or backup systems properly "take over" for the failed system without any loss of data or transactions.; Recovery testing is an antagonistic test process in which the application or system is exposed to extreme conditions, or simulated conditions, to cause a failure, such as device Input/Output (I/O) failures, or invalid database pointers and keys. Recovery processes are invoked, and the application or system is monitored and inspected to verify proper application, or system, and data recovery has been achieved.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |  [Simulate the failure conditions and exercise the recovery processes (manual and automated) to restore the database, applications, and system to a desired, known state. The following types of conditions are included in the testing to observe and log behavior after recovery:; power interruption to the client; power interruption to the server; communication interruption via network servers; interruption, communication, or power loss to DASD (Dynamic Access Storage Devices) and DASD controllers; incomplete cycles (data filter processes interrupted, data synchronization processes interrupted); invalid database pointers or keys; invalid or corrupted data elements in database]  |
|Technique              |  [The tests already created for Function and Business Cycle testing can be used as a basis for creating a series of transactions to support failover and recovery testing, primarily to define the tests to be run to test that recovery was successful.; Power interruption to the client: power down the PC.; Power interruption to the server: simulate or initiate power down procedures for the server.; Interruption via network servers: simulate or initiate communication loss with the network (physically disconnect communication wires or power down network servers or routers).; Interruption, communication, or power loss to DASD and DASD controllers: simulate or physically eliminate communication with one or more DASDs or DASD controllers.; Once the above conditions or simulated conditions are achieved, additional transactions should be executed and upon reaching this second test point state, recovery procedures should be invoked.; Testing for incomplete cycles utilizes the same technique as described above except that the database processes themselves should be aborted or prematurely terminated.; Testing for the following conditions requires that a known database state be achieved. Several database fields, pointers, and keys should be corrupted manually and directly within the database (via database tools). Additional transactions should be executed using the tests from Application Function and Business Cycle Testing and full cycles executed.]   |
|Oracles                |  [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]  |
|Required Tools         |  [The technique requires the following tools:; base configuration imager and restorer; installation-monitoring tools (registry, hard disk, CPU, memory, and so on; backup and recovery tools]  |
|Success Criteria       |  [The technique supports the testing of:; One of more simulated disasters involving one or more combinations of the application, database, and system.; One or more simulated recoveries involving one or more combinations of the application, database, and system to a known desired state.  ] |
|Special Considerations |  [Recovery testing is highly intrusive. Procedures to disconnect cabling (simulating power or communication loss) may not be desirable or feasible. Alternative methods, such as diagnostic software tools may be required.; Resources from the Systems (or Computer Operations), Database, and Networking groups are required.; These tests should be run after hours or on an isolated machine.]  |
-->

#### 5.2.11 Configuration Testing
(n/a)
<!--
[Configuration testing verifies the operation of the target-of-test on different software and hardware configurations. In most production environments, the particular hardware specifications for the client workstations, network connections, and database servers vary. Client workstations may have different software loaded (for example, applications, drivers, and so on) and, at any one time, many different combinations may be active using different resources.]

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |   [Exercise the target-of-test on the required hardware and software configurations to observe and log target behavior under different configurations and identify changes in configuration state.]  |
|Technique              |   [Use Function Test scripts.; Open and close various non-target-of-test related software, such as the Microsoft Excel and Word applications, either as part of the test or prior to the start of the test.; Execute selected transactions to simulate actors interacting with the target-of-test and the non-target-of-test software.; Repeat the above process, minimizing the available conventional memory on the client workstation.]  |
|Oracles                |   [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]  |
|Required Tools         |   [The technique requires the following tools:; base configuration imager and restorer; installation-monitoring tools (registry, hard disk, CPU, memory, and so on ] |
|Success Criteria       |   [The technique supports the testing of one or more combinations of the target test items running in expected, supported deployment environments.]  |
|Special Considerations |   [What non-target-of-test software is needed, is available, and is accessible on the desktop?; What applications are typically used?; What data are the applications running; for example, a large spreadsheet opened in Excel or a 100-page document in Word?; The entire systems' netware, network servers, databases, and so on, also need to be documented as part of this test.]  |
-->

#### 5.2.12 Installation Testing
<!-- TODO -->
[Installation testing has two purposes. The first is to ensure that the software can be installed under different conditions (such as a new installation, an upgrade, and a complete or custom installation) under normal and abnormal conditions. Abnormal conditions include insufficient disk space, lack of privilege to create directories, and so on. The second purpose is to verify that, once installed, the software operates correctly. This usually means running a number of tests that were developed for Function Testing.]

|      Step             | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |   [Exercise the installation of the target-of-test onto each required hardware configuration under the following conditions to observe and log installation behavior and configuration state changes:; new installation: a new machine, never installed previously with Project Name; update: a machine previously installed Project Name, same version; update: a machine previously installed Project Name, older version]  |
|Technique              |   [Develop automated or manual scripts to validate the condition of the target machine.; new: never installed; same or older version already installed; Launch or perform installation..; Using a predetermined subset of Function Test scripts, run the transactions.]  |
|Oracles                |   [Outline one or more strategies that can be used by the technique to accurately observe the outcomes of the test. The oracle combines elements of both the method by which the observation can be made and the characteristics of specific outcome that indicate probable success or failure. Ideally, oracles will be self-verifying, allowing automated tests to make an initial assessment of test pass or failure, however, be careful to mitigate the risks inherent in automated results determination.]  |
|Required Tools         |   [The technique requires the following tools:; base configuration imager and restorer; installation-monitoring tools (registry, hard disk, CPU, memory, and so on ] |
|Success Criteria       |   [The technique supports the testing of the installation of the developed product in one or more installation configurations.]  |
|Special Considerations |   [What transactions should be selected to comprise a confidence test that application has been successfully installed and no major software components are missing?]  |

#### 5.2.13 API Testing

|        Step           | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    |   The API-Endpoints are delivering correct results  |
|Technique              |   Possible requests are executed and the result is compared to the expected result |
|Oracles                |   All API-Endpoints respond with the correct data  |
|Required Tools         |   Postman |
|Success Criteria       |   All API-Endpoints responded with the correct data  |
|Special Considerations |   -  |

## 6. Entry and Exit Criteria

### 6.1 Test Plan

#### 6.1.1 Test Plan Entry Criteria

New Pullrequests to the protected branches "master"/"main" and "develop" or changes in open Pullrequests trigger the GitHub-Actions CI/CD pipeline that contains UnitTests.

#### 6.1.2 Test Plan Exit Criteria

After executing every given Tests the Testing is complete. All UnitTests and the Build has to pass to allow Contributers to accept the PR.

#### 6.1.3 Suspension and Resumption Criteria

n/a

### 6.2

##### 6.2.1 Test Cycle Entry Criteria

n/a

##### 6.2.2 Test Cycle Exit Criteria

n/a

##### 6.2.3 Test Cycle Abnormal Termination

n/a


## 7. Deliverables

## 7.1 Test Evaluation Summaries

test results can be viewed in the logs on GitHub actions. https://github.com/JanPfenning/Mood4Food/actions

## 7.2 Reporting on Test Coverage

The Tests will be executed with every Pullrequest. Tests have to pass to allow be merge to fulfill.
Testcoverage can be viewed at https://github.com/JanPfenning/Mood4Food

## 7.3 Perceived Quality Reports

n/a

## 7.4 Incident Logs and Change Requests

Tests are automated with GitHub-Actions which is also writing the Reports. CodeCoverage is reviewed by Codecov.io 

## 7.5 Smoke Test Suite and Supporting Test Scripts

n/a

## 7.6      Additional Work Products

n/a

### 7.6.1     Detailed Test Results
n/a

### 7.6.2     Additional Automated Functional Test Scripts

https://github.com/JanPfenning/Mood4Food/tree/develop/.github/workflows

### 7.6.3     Test Guidelines

n/a

### 7.6.4     Traceability Matrices

n/a

## 8. Testing Workflow

When new functionality is implenmented that can be meaningfully tested, this should be done. First tests are written locally and when local tests pass the new functionality with the corresponing tests can be pushed. The new Tests will automatically run before the Pullrequest can be merged.

## 9. Environmental Needs

Non-human resources required:
- GitHub Actions (Automatic-Remote-Execution costs points)

### 9.1 Base System Hardware

The following table sets forth the system resources for the test effort presented in this Test Plan.

| Resource                                                                | Quantity | Name and Type |
|-------------------------------------------------------------------------|----------|---------------|
| Local test machine                                                      |          | Own Notebook  |
| - Include special configuration requirements (Mobile Emulator)          |1         | IDE Emulator  |

### 9.2 Base Software Elements in the Test Environment

The following base software elements are required in the test environment for this Test Plan.

| Software Element Name |  Type and Other Notes                        |
|-----------------------|----------------------------------------------|
| Android Studio        | Test Runner / IDE                            |
| JUnit 4               | Unit testing library                         |
| Postman               | API-testing                                  |

### 9.3 Productivity and Support Tools

The following tools will be employed to support the test process for this Test Plan.

| Tool Category or Type             | Tool Brand Name |
|-----------------------------------|-----------------|
| Version Control                   | GitHub          |
| Test Coverate Monitor or Profiler | Codecov.io      |
| Project Management                | Jetbrains YouTrack|

### 9.4 Test Environment Configurations

n/a

## 10. Responsibilities, Staffing, and Training Needs

### 10.1 People and Roles

See the staffing assumptions for the test effort.

https://md4fd.wordpress.com/2020/10/06/2-week-team-and-tools/

### 10.2 Staffing and Training Needs

n/a

## 11. Iteration Milestones

We want to keep over [20]% code coverage. Files that are for visual presentation like Views and XML files are excluded.

## 12. Risks, Dependencies, Assumptions, and Constraints

| Risk                                    | Mitigation Strategy                                           | Contingency (Risk is realized)                                                                              |
|-----------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|
| Unexpected failrues                     | Especially cover edge-cases and Calculation                   | Check are shown as failures at PR. No merge to productive system |
## 13. Management Process and Procedures
When new functionality is implenmented that can be meaningfully tested, this should be done. First tests are written locally and when local tests pass the new functionality with the corresponing tests can be pushed. The new Tests will automatically run before the Pullrequest can be merged by another contributer. The PR-Issuer is never allowed to merge an own PR. (You may also want to visit the blogarticle about this topic: https://md4fd.wordpress.com/2021/05/02/week-2-5-tests/)

Additionally a Metrics-Check is executed with every new/updated PR. This shows quality of code. (To get more information about metrics visit the blog: https://md4fd.wordpress.com/2021/05/28/week-2-9-metrics/)