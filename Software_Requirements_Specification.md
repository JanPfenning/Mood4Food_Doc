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
This Software Requirements Specification (SRS) describes all specifications for the application "Common Playground". It includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.


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

<div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#0000ff&quot;,&quot;nav&quot;:true,&quot;resize&quot;:true,&quot;toolbar&quot;:&quot;zoom layers lightbox&quot;,&quot;edit&quot;:&quot;_blank&quot;,&quot;xml&quot;:&quot;&lt;mxfile host=\&quot;app.diagrams.net\&quot; modified=\&quot;2020-10-13T10:10:15.114Z\&quot; agent=\&quot;5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36\&quot; etag=\&quot;O9iXtrPlEsQpluZHJTFd\&quot; version=\&quot;13.7.9\&quot; type=\&quot;device\&quot;&gt;&lt;diagram id=\&quot;ToanAmvhAh_Zf448w_O6\&quot; name=\&quot;Page-1\&quot;&gt;7Vpbc9o4FP41PLbjCxh45JKkO5tMM6U7bZ86whagRra8srjl1+85kgw2cmiyA6Tp9CWRjm7W952rTSscpZsbSfLFnUgobwVesmmF41YQ+F7Yg38o2RpJp20Fc8kSO2kvmLBHWq600iVLaFGbqITgiuV1YSyyjMaqJiNSinV92kzw+qk5mVNHMIkJd6VfWKIWRtoLunv5B8rmi/JkP+qbkZSUk+1NigVJxLoiCq9a4UgKoUwr3YwoR/BKXMy66ydGdw8maaaes+DuS3cRhzfdzw/z/uNH4ZOA+u/sLivCl/bCrSDisN9wJmBbeGq1tVBE/y5FOfCu0EQNYILfzzf7QWjN8f8gS6SAkwNvkOecxUQxkZVbT2U5rZTAU5vzSnFQOzpYqJRDy4cxTqaU34uC6R3DcQzXpxIGVlQqOIjfHkxQIodRwtm8cfrADkyFUiLdHV7FtQQJVtBNRWRxvqEipUpuYYodDUvtLZXedtd7DQrbVraoaE+3FBKrtfPd1ntioWG5fQHPgcPzIFZCOkCDkubYXKbcTHga1x1gh0gawCuUnQBR/wDRttd1IG1CNHo5oP8UVH6c/kBnEnha28zSD5RwOCrw7kgGVp/iZfTeR4EPK9eyRDXAjW5JayVawcSOI3RFTmKWzT8jpGPAIBwqMi0dkR9awc4Dta2gQhOnM1Wn48UWlLIkwSfaGZHds5l4vf1QSLjQSHBUoXEmMrq/zK1ePe6cyNaCumZEDbYWNGjGzi+/QDWgW9GOF5hf2zG/CaWtYITPuWAxalW2VJIBDIUOXBQjCCsKgMuxUTgPoh8CCmsVnQCqOLKGAFwn2vF5M8Z5yUkrCGczGsUxEqOkeKCVkaTbn3reiQgK6wTtTLnCkN/oDc/lDDsupAkEfdsVUi3EXGSEX+2lQymWWUJxV4RlP+dWGNME4Q+q1NZmMGSpRJ0MumHqq12O7W+V9hihQi213a027o7t3lPJ4OLI4PgoJ4VYypgeuXhkEygi51QdywosQgjLUYol5RDZV/Vc6QS+9hONWQ5p38/9a/THv17Wv4becx1seEEH23UcLBjmAx6utMKDTmh1rajV7+NRw4b88rIetefA/zelOSIvSYw0iJmJdguogCCyLXXI24olisgKo92U0gzrRMmyBx31PAGI4BYLHE7I9ny0JR3aS9pNtPWCaRhFZwqEfZe2wGugrX8u2vpHraZQ4NsL8EBFlTtDGktzCfwkRiD1A5v0+G2bVrv/P5MV3zsXSeUTVFi6ocp4M5FCGZLo4roo00nNnWEpJmhSVEsyulFvnZ1DC2q3X9vx+e4LlFv2gA4L9wW3xQpu+tBaYOhxX4HgvMI4QUgaS4c3IyshgZM3H60OTeqc0eqpfHICqTkElecklH7wJ6O8bEbZaXo99uoZpR86lj0iPF5CwUMrWQnjW+1oATZskAxDYlnL4wyaatnvlbpEDUXAhR1v28X0AkV8Bs++q+Kx863aqdbxul8p5LF/ukq+rNB/Wsrbkv/slfwzWes4RuXQSIrcfMiZsQ1yVcU/FwzfkMG8zrDVGTfZB0v1Fx3jlw2P4NJ38jFLoba45mwKf8njUlK8Esnz7+AlVizGeHs9gO7EdL/fc5IV74vVHPaYS5KgXR94yRMYWNc7yGy80DGwqO3aVyk7PVOR6/4kNb5PrLNLFNOXcW2H6ckvkFO6LzMG9385OCtM6JtQPEhIDmP+LjeoB/dwL/lkLxk62FuFlwJKQzLVR3iOWQ4BmJH3voMGCjVJZ+jv+9pmc/C8I6hYlCRM80ZJoda0UKdhNDpkNHK/FUW9hvQiOheh7uuRia7gTBJBWFrsSrY10WmDLgTA3uIzVtSvY1+/QOrgvvao0gEGIGlSfooxrCRIRyZ0VaHLubfNiZPO9c7HCXT3v3HQY5VfioRX/wE=&lt;/diagram&gt;&lt;/mxfile&gt;&quot;}"></div>
<script type="text/javascript" src="https://viewer.diagrams.net/js/viewer-static.min.js"></script>


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

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  
Until December we plan to implement:
- 3.1.1 (tbt)

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
For any further information you can contact the Common Playground Team or check our [Common Playground Blog](http://commonplayground.wordpress.com). 
The Team Members are:
- Rico Peter Rauschkolb
- Konrad Schewe
- Jan Pfenning
