# Mood4Food_Doc - Software Requirements Specification 

## Table of contents
- [Table of contents](#table-of-contents)
- [Introduction](#1-introduction)
    - [Purpose](#11-purpose)
    - [Scope](#12-scope)
    - [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
    - [References](#14-references)
    - [Overview](#15-overview)
- [Overall Description](#2-overall-description)
    - [Vision](#21-vision)
    - [Use Case Diagram](#22-use-case-diagram)
	- [Technology Stack](#23-technology-stack)
- [Specific Requirements](#3-specific-requirements)
    - [Functionality](#31-functionality)
    - [Usability](#32-usability)
    - [Reliability](#33-reliability)
    - [Performance](#34-performance)
    - [Supportability](#35-supportability)
    - [Design Constraints](#36-design-constraints)
    - [Online User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
    - [Purchased Components](#purchased-components)
    - [Interfaces](#39-interfaces)
    - [Licensing Requirements](#310-licensing-requirements)
    - [Legal, Copyright And Other Notices](#311-legal-copyright-and-other-notices)
    - [Applicable Standards](#312-applicable-standards)
- [Supporting Information](#4-supporting-information)

## 1. Introduction

### 1.1 Purpose
This Software Requirements Specification (SRS) describes all specifications for the application "Mood4Food". It includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.


### 1.2 Scope
The project is going to be realized as an Android App.  
Actors of this App will be users who want to *spicen* theire life.

### 1.3 Definitions, Acronyms and Abbreviations

| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| n/a         | not applicable                         |
| tbd         | to be determined                       |
| UCD         | overall Use Case Diagram               |
| FAQ         | Frequently asked Questions             |

### 1.4 References

| Title                                                              | Date       | Publishing organization   |
| -------------------------------------------------------------------|:----------:| ------------------------- |
| [Mood4Food Blog](http://md4fd.wordpress.com)                       | 13.10.2020 | Mood4Food Team            |
| [GitHub](https://github.com/JanPfenning/Mood4Food)                 | 13.10.2020 | Mood4Food Team            |


### 1.5 Overview
The following chapter provides an overview of this project with vision and Overall Use Case Diagram. The third chapter (Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally there is a chapter with supporting information. 
    
## 2. Overall Description

### 2.1 Vision
We came to the conclusion that there were days when you didn't know what to eat - Enough days when you run to the fridge 10 times an hour out of pure boredom to "wonder" just one more time that there is still nothing inside. With our app we want to help you with this.

### 2.2 Use Case Diagram

<iframe frameborder="0" style="width:100%;height:988px;" src="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=UC#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2FUC"></iframe>
</br>
<p style="font-size:0.8rem">
Use the following link to see the diagramm when the iframe doesn't work:</br>
<a href="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=UC#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2FUC">Overall Use-Case Diagram</a></p>

- Green: Planned till end of december
- Yellow: Planned till end of june

### 2.3 Technology Stack
The technology we use is:

Frontend:
-Kotlin and XML/JSON

IDE:
-Android Studio (IntelliJ)

Project Management:
-YouTrack
-GitHub

Testing:
-JUnit
-Espresso (Gherkin)

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  
Until December we plan to implement:
- 3.1.1 Goals Use Case:
Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Goals#R7Vpbc5s4GP01fmxGgMDw2NhxurNdb2Y8nbaPCsigBiOPkG%2F99SsZES7CDrGNL5t6MhP0SSB0zvkukt2zBrP1I0Pz6B8a4LhngmDds4Y90zTEn%2FgnLZvM4kA7M4SMBGpQYZiQ31gZgbIuSIDTykBOaczJvGr0aZJgn1dsiDG6qg6b0rg66xyFWDNMfBTr1u8k4JGyGo5XdHzBJIzU1K7pZB3PyH8JGV0kar6eaU23n6x7hvJnqYWmEQroqmSyHnrWgFHKs6vZeoBjiW0OW3bfaEfv63sznPA2N5jZDUsUL9TSv6WYqXfjmxyPdEVmMUpE634VEY4nc%2BTLrpWgX59SvcUSM47XJZN6hUdMZ5izjRiS9zrwTglkk0vIzdqrAn7TVaBFJeTtvjIiRXn4%2BvRi2eJCrbwZBVtDQUNA3CDEJwEQlM2lMeWI8QlHXBqnJI4HNKZsO9oC248czBl9waWe6VT16LCZ74YNgApoEGiYWQ2QWSdAzGmBWCBcSjVx%2FExXD4XhfmsQHRFl5DdNOBIT3cuVE%2BGEn2MSJqLzmXJOZ3J0EnyWXi1sdI6TzKKihtuE8mikUBbjRkSuYmiI1tYxsVwC2Al%2FShfMxxVdyJUcw0cT0OohT5SI%2BYsnGHVH8GrPEKILMVe31fh6faNWFP7tfnkcT75Px0PuicA1%2BvXya%2FYJGhqx%2F0rETfBIUZxqJBeIGo2xwbqP%2BCyHHzFfkQYlN1PBe5PP1HxJRk%2B%2FjS9pjtPA707u7BrspuZKhtngS%2FsobutLjUTYQCPiISBSKk%2FRJpVeIi4HNBE2QpMPw4sJLk6MHvoUMeMFZx%2BLDevybHgaG4OY%2BC%2FSOVDsL2KZnk0nFu9x%2FyzqGieUV2OMg48Ty%2BA5WbI0PiablOOZhnbHJSWEly0pm7Orq6HzlaJAbmQWbLtYTaoq7QI5sQkmmHOShNIwZaI00oZ%2FpVlmmHDK5B7nhjVu7eXXBfVC6eKhCOrSR0ssI1GEklBsZzW2OBW9H4Yyx767umSuO%2BQfzvZydvmU7%2BhnFmO0JOE20wNJT1O6LxUEN16hvZOws2b%2FZsL0mkDDv3xYQBmPaEgTFJdPDEr4n%2B6c4BV5gS7b%2FBBGmVZU86ds5o3hutLaqFav6YCgeoiwV8QasULB2x2%2BMrnNZDMsdbysTtr%2BmAGadZXYuUpOf85g6TFWp187XZPEHXi2tgvYdxysGfXqwjZ0L%2BrqbE2vI779pSHWcfncN6%2BwfLb1yD8k6TxGm30VdFEz327Mh3vJ8urefPFaGOrb8isO%2BZWAX8T%2FE4f8fPPX4JflkL9H%2BSfPA45bPbC26oLo%2BrRZd%2BjrlckncAccWNUKdPtvqGXbesKMCKwwO1ZCDaGhrYRgN6WEWZPQub%2BwsPUvLK5OQofSbTfUMjvS9pEs2kYtENhnZvF%2FvEXAa8JLt4nWT%2FWS8rq4STaOzTF5hXRQjgGdSMut5xjzzNJq8%2BX%2BH2m9LS14hLScbqJWvyotWN99dS2t%2Fi1J6zxVbv716EEyOU%2BJYoPzysS5gRLlkEhy4jOzBsW8rTa3rbS8bqTlVaXltExuDRr17mAf2K4rai%2FTg7CqWLf22AyY7hSr%2F%2Fjk%2BhR77sDm7ZTpm%2Bpzutm%2B1wObY5wqsIlm8RvUbHjxQ1%2Fr4T8%3D
Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/editGoals.feature

Until June, we want to implement:
- 3.1.6 (tbt)

### 3.2 Usability
We plan on designing the user interface as intuitive and self-explanatory as possible to make the user feel as comfortable as possible using the app.

#### 3.2.1 No training time needed
Our goal is that a user installs the android application, opens it and is able to use all features without any explanation or help.

#### 3.2.2 Familiar Feeling
We want to implement an app with familiar designs and functions. This way the user is able to interact in familiar ways with the app without having to get to know new interfaces.

### 3.3 Reliability

#### 3.3.1 Availability
Since we do not think of implementing a Serversided connection the Application should run a full 100% of the time! 

### 3.4 Perfomance

#### 3.4.1 Capacity
(tbt)

#### 3.4.2 Storage 
(tbt)

#### 3.4.3 App perfomance / Response time
(tbt)

### 3.5 Supportability

#### 3.5.1 Coding Standards
We are going to write the code by using all of the most common clean code standards. For example we will name our variables and methods by their functionalities. This will keep the code easy to read by everyone and make further developement much easier.

#### 3.5.2 Testing Strategy
The application will have a high test coverage and all important functionalities and edge cases should be tested. Further mistakes in the implementation will be discovered instantly and it will be easy to locate the error.

### 3.6 Design Constraints
(tbt)

### 3.7 On-line User Documentation and Help System Requirements
(tbt)

### 3.8 Purchased Components
Currently no purchased components are integrated. As soon as this changes we will list them here.

### 3.9 Interfaces

#### 3.9.1 User Interfaces
The User interfaces that will be implented are:
- Receipe Overview - 
- ...

#### 3.9.2 Hardware Interfaces
(n/a)

#### 3.9.3 Software Interfaces
The app will currently only be runnable under Android.

#### 3.9.4 Communication Interfaces
(n/a)

### 3.10 Licensing Requirements

### 3.11 Legal, Copyright, and Other Notices
We do not take responsibilty for any incorrect data or errors in the application.

### 3.12 Applicable Standards
The development will follow the common clean code standards and naming conventions.

## 4. Supporting Information
For any further information you can contact the Mood4Food Team or [check our Blog](http://md4fd.wordpress.com). 
The Team Members are:
- Rico Peter Rauschkolb
- Konrad Schewe
- Jan Pfenning
