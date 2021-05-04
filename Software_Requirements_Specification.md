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
<a href="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=UC#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2FUC.drawio">Overall Use-Case Diagram</a></p>

- Green: Planned till end of december
- Yellow: Planned till end of june
- Purple: Optional

### 2.3 Technology Stack
The technology we use is:

Frontend:
-Kotlin and XML/JSON

IDE:
-Android Studio (IntelliJ)
-Visual Studio Code

Project Management:
-YouTrack
-GitHub

Testing:
-JUnit
-Espresso (Gherkin)

Backend:
-PHP

Database:
-MySQL

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  
Until December we plan to implement:
- 3.1.1 CRUD Recipe:
	- Mockup: https://konrad400294.invisionapp.com/public/prototype/skghts6bg00as9401o6extwkc/546d7292
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=createrecipe.drawio#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2Fcreaterecipe.drawio
	- Feature Files:
		- Create Recipe: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/addrecipe.feature
		- Read Recipe: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/viewRecipe.feature
		- Update Recipe: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/editRecipe.feature
- 3.1.2 Waterbalance Use case:
	- Mockups: h.invisionapp.com/public/prototype/skghuj5co00lz1301ofl2uuaf/32f0279c
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Water_Management.drawio#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2FWater_Management.drawio
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/checkwaterbalance.feature
- 3.1.3 Edit your Goals Use Case:
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Goals#R7Vpbc5s4GP01fmxGgMDw2NhxurNdb2Y8nbaPCsigBiOPkG%2F99SsZES7CDrGNL5t6MhP0SSB0zvkukt2zBrP1I0Pz6B8a4LhngmDds4Y90zTEn%2FgnLZvM4kA7M4SMBGpQYZiQ31gZgbIuSIDTykBOaczJvGr0aZJgn1dsiDG6qg6b0rg66xyFWDNMfBTr1u8k4JGyGo5XdHzBJIzU1K7pZB3PyH8JGV0kar6eaU23n6x7hvJnqYWmEQroqmSyHnrWgFHKs6vZeoBjiW0OW3bfaEfv63sznPA2N5jZDUsUL9TSv6WYqXfjmxyPdEVmMUpE634VEY4nc%2BTLrpWgX59SvcUSM47XJZN6hUdMZ5izjRiS9zrwTglkk0vIzdqrAn7TVaBFJeTtvjIiRXn4%2BvRi2eJCrbwZBVtDQUNA3CDEJwEQlM2lMeWI8QlHXBqnJI4HNKZsO9oC248czBl9waWe6VT16LCZ74YNgApoEGiYWQ2QWSdAzGmBWCBcSjVx%2FExXD4XhfmsQHRFl5DdNOBIT3cuVE%2BGEn2MSJqLzmXJOZ3J0EnyWXi1sdI6TzKKihtuE8mikUBbjRkSuYmiI1tYxsVwC2Al%2FShfMxxVdyJUcw0cT0OohT5SI%2BYsnGHVH8GrPEKILMVe31fh6faNWFP7tfnkcT75Px0PuicA1%2BvXya%2FYJGhqx%2F0rETfBIUZxqJBeIGo2xwbqP%2BCyHHzFfkQYlN1PBe5PP1HxJRk%2B%2FjS9pjtPA707u7BrspuZKhtngS%2FsobutLjUTYQCPiISBSKk%2FRJpVeIi4HNBE2QpMPw4sJLk6MHvoUMeMFZx%2BLDevybHgaG4OY%2BC%2FSOVDsL2KZnk0nFu9x%2FyzqGieUV2OMg48Ty%2BA5WbI0PiablOOZhnbHJSWEly0pm7Orq6HzlaJAbmQWbLtYTaoq7QI5sQkmmHOShNIwZaI00oZ%2FpVlmmHDK5B7nhjVu7eXXBfVC6eKhCOrSR0ssI1GEklBsZzW2OBW9H4Yyx767umSuO%2BQfzvZydvmU7%2BhnFmO0JOE20wNJT1O6LxUEN16hvZOws2b%2FZsL0mkDDv3xYQBmPaEgTFJdPDEr4n%2B6c4BV5gS7b%2FBBGmVZU86ds5o3hutLaqFav6YCgeoiwV8QasULB2x2%2BMrnNZDMsdbysTtr%2BmAGadZXYuUpOf85g6TFWp187XZPEHXi2tgvYdxysGfXqwjZ0L%2BrqbE2vI779pSHWcfncN6%2BwfLb1yD8k6TxGm30VdFEz327Mh3vJ8urefPFaGOrb8isO%2BZWAX8T%2FE4f8fPPX4JflkL9H%2BSfPA45bPbC26oLo%2BrRZd%2BjrlckncAccWNUKdPtvqGXbesKMCKwwO1ZCDaGhrYRgN6WEWZPQub%2BwsPUvLK5OQofSbTfUMjvS9pEs2kYtENhnZvF%2FvEXAa8JLt4nWT%2FWS8rq4STaOzTF5hXRQjgGdSMut5xjzzNJq8%2BX%2BH2m9LS14hLScbqJWvyotWN99dS2t%2Fi1J6zxVbv716EEyOU%2BJYoPzysS5gRLlkEhy4jOzBsW8rTa3rbS8bqTlVaXltExuDRr17mAf2K4rai%2FTg7CqWLf22AyY7hSr%2F%2Fjk%2BhR77sDm7ZTpm%2Bpzutm%2B1wObY5wqsIlm8RvUbHjxQ1%2Fr4T8%3D
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/editGoals.feature
- 3.1.4 Get Health Demand Information Use Case:
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Calculation#R7Vttc5s4EP41%2FtgOSIDxx9p5uev0ep3zdNr0m4JlrAlGHiHHcX%2F9SUYYkLBNHDC200xmglZCQvs8u9pdSA%2BO5i%2F3DC1m%2F9AJjnrAmrz04E0PAFv8ij9Ssk4lnuOmgpCRiRqUC8bkN1ZCS0mXZIKT0kBOacTJoiwMaBzjgJdkiDG6Kg%2Bb0qi86gKF2BCMAxSZ0h9kwmdKanuDvOMvTMKZWtoHXtrxiIKnkNFlrNbrATjd%2FKTdc5TNpTaazNCErgoieNuDI0YpT6%2FmLyMcSd1makvvu9vRu31uhmNe5waQ3vCMoqXa%2BvcEM%2FVsfJ3pI1mReYRi0RquZoTj8QIFsmsl4DeXVE%2FxjBnHLwWReoR7TOeYs7UYkvV6zkdFkHVGIT9tr3L1A18pbVbQvNtXQqQgD7ez59sWF2rn1VpwDS0YGhA3CPJJBQjIFlKYcMT4mCMuhVMSRSMaUbYZDa3NjxzMGX3ChZ7pVPWYagOvVptllZTmWIbOYIXKYAMa82pobCJMSjVx9EhXt7lguBGIjhll5DeNORILDeXOiTDCTxEJY9H5SDmnczk6nnySVi1kdIHjVKK8hl%2Bl5bs7pWUx7o7IXdzYorUxTCy3YO1Uf0KXLMAlXsidvAWPKkWrSb5RItbPZ7Bd3RBsbRLBuhBzdZ8G2PaRamHof4aLKLCGnxfhj18UR%2FNPDH7wbAPZUUSCJyG6x%2FJJ%2F8PJMpIXw6VAJzZgz3VsV3oLOJzxeQYIYoGC0ZFoTQUTqqxIsy7pT4M61mWYUgXie9AsAQEGwLAuG1SY1z7U65pXJTSO6aYyaG4nREJyT1GUXDEiULeO7kHx%2FJ2gjNEz3hpMki6eYvQOrMfToXKcE0IFDVDG64Tj%2BakDG8fpNrCp9iMDQztf0TMJZSQj4%2Bwe8ISDh8NHEQd6oby6eL8CX8fVM3ArjulWUBQsoxSkrxhP3hMg0O0akMwaiy5F8%2B%2B61WzdfbLDrL7QYHMWjDllMiG9Wjz73R4G5hFtqNpM72SGcWRyV62d15wbwv1rGnOBqbG2krtKA3BNAzC1WEj5KOMzGtIYRcW8r0DY5rK9LVWFwtn6pxBaQnuq%2BSCbWePmpdRaq1avKs2rhLCYHe49XNM0rUhAE2yGhTsnz%2BVF6yeLjrvTrA4ki0K9aF0YtpADkt0rAccuu2MbaHxKZ2w0E%2B2D6yUcfiH8p3osef2QTyFa%2BU2y0QJJs8PsBCSFhu%2BHfj2SmsWRwcGp0p03URwx46%2Fvfxv025s9SN7ICmHKI4FNVc3v1RlFH5xjRmEWjfaa6rmWA%2FcaV9u1P9AflGYAtn%2BcnYiJdIoMtKmas5NqPpiu%2B18JFLCyJIZcdu3jQPRm6wBs3%2Fd0Vzw0SyKqaDjGnJM4rEhg6FR0B0u22bcYSPjy3SEHYefIme9avlA0KUKjA5dDak2ZcJnXnHnuB9QFZ2eIfQNOVUgYzVAc4go7lLUD6%2F1Apr146d4Cs%2BJTAbIbkiyiTQ5VwwivFSkflJHq3rhc85TbG4h2mzOWMsY8gTy%2BSKFEh4sU6kgp5n97mN94Uuj5monrhGj5JbdrZnfnS5MP1kfLc8pccfz%2BoQqDbH3DjAhdYdYChUBNCqVca5xCQKMQGJyYQnW%2BGeqYQk3CvaPA%2F0YUjbPePTGKr%2FyO6RJrjHld8aGXVxyPrjHWZYxb20G0Qy1fP2PAiallxvl%2FqNWQM%2BrXpZbbztljFNgc%2FbVb21%2FpXVSce53k8nYkR28ObAxy1YyOzdNVd4G%2BNlHLZWDvol4Zd5eNuXXd2aAdxrmWzrg%2BPK07MwssV0OUBt3ZQSZ5u1l42J057ZALln2Qe%2BIwzDMj%2FLx2V3oblX%2FIdbX1Oi3bcvyu63XenyC5GcP33mD47Xz44fc1w9eDj7YN%2FwIKNA0HH4dp4ryBJu3U8VydJvpHKm3TxPwY%2FuxocjTc%2FvFw961W4DZTZ6%2Bx1Fk083%2BcTYfn%2F50Mb%2F8H
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/calculateNeeds.feature
- 3.1.5 Rate Ingredient use Case:
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Favorite%20Ingredients#R7VvZcuI4FP0aHjNlywvmMYGQTk2mZmqoruk8KlgYdYRFyWLrrx8Jy3iRHdwGm9A0Dwm6Wizfc%2B6ia9OzhovtE4PL%2BV%2FUR6QHDH%2Fbs0Y9AEzD8sQ%2FKdnFEsdWgoBhXw1KBRP8AyUzlXSFfRTlBnJKCcfLvHBKwxBNeU4GGaOb%2FLAZJfmrLmGANMFkCoku%2FQ%2F7fK6kpjtIO74gHMzVpT3gxh1vcPoeMLoK1fV6wJrtP3H3AiZrqRuN5tCnm4zIeuxZQ0Ypj78ttkNEpG4TtcXzxhW9h30zFPI6E0A8YQ3JSt361wgxtTe%2BS%2FQRbfCCwFC0HjZzzNFkCaeyayPg1y%2BpdrFGjKNtRqS28IToAnG2E0OSXtf%2Bw4knKcKYQBFmk6ofeEpp84zmnb4SQgV5cFg9vW3xRd15uRYcTQuaBsQEQT6pAAHZUgojDhmfcMilcIYJGVJC2X60Zew%2FcjBn9B1lemYz1aOrDfy02gwjpzTb0HRmlajMOoPG3Boa84VJqSYib3TzmAoe9gLRMacM%2F6Ahh%2BJCD%2FLOsTDCe4KDUHS%2BUc7pQo4O%2FXtp1UJGlyiMJcpreGVaHo%2BVlsW4MZZ3MTJFa2%2BYSN6CUan%2BiK7YFOV4Ie%2FkFDzKFK0W%2BYdicf10BdMpGoJZWESwLkBczSsAdthSLQxf3fX3uy%2BbO4%2Bsh8Hr9z%2BfwJLe2aaG7N9S5cAYw7UAS7AdGM9hwJCPheoiDfZUx2apt7Ae5nyRAALZVMFoS7RmggllVlSwLulPp3WsSzOlEsQr0XSKQADNukxQYl4foV7XvMqh6WvQ3Pt%2BDo7bQWNwaTQcHY1%2F0YKu0W0CYlsdAmJpqp%2FsIo4WXecttn3ZvKXcTejaeaHQ%2F8CDGzMmwiwwXqgIvuL%2FhFMmE%2BQr5q71IW6eoUXZS7sTV89BVdwdYUhosD%2FFsIJvMSaIiOMPpuEtYXVx19%2FXsZrAveMP0abKzvZH2Js2Msu%2BOHB6zBZHE7RH6jGMd3%2FzvrDTSG5rgHx97jqK98FnjOK6jxnhaEmg3PgLjqQ%2FoTMtku%2FoSvwl%2BF1SGob%2BQeRL3xNSfui9Xj7bR%2Fj8ySK7M9A5vvTh3ukoIDdYbC2JHrmQ8VyW1f6qWH2CAKFjVXqoS4C7KXg6DQyl8Hh6cUrTvl6olbXChmXa03VognxocUr8UVtF2nIdgho6zJRuKeNzGtAQkmz9NsPg81VtD9xFMhf7JoQyN1HNV9lMGqNtrrVLWlvMM9NE61VtUn5PJ8lGMie%2B%2BUKJtwThfGX4Q%2B8Rl2iP8ljnDEMEcrzO76R%2B9XhQsFcX5FeoKB1r69y5g2JOWFwq1kV7VWg9L%2FzEJM1RNGVsBUkrCHeUXUldpyTXPUq4OJs8O%2BEO6W9Ck2I63PbDiqvyZR3RpMSB1aZJxVHxRJqAftGfWMUUoW2i%2FOTzyhsNesfJ5ZxArn4r5PK0dwc6J5d3TeTqyAv1mxPFbSlY2cXTZrc0cY0roEkDX9LUbzWlVlJPaUItpx0fZJt5arkdv7TR1%2FOgIQyniCC%2Fl31IZI01xrE5XbytouOFipYqEB%2BXZh3tAas1UGlw5vxcVpltr0SkP14N6WmGDJUBEzTj7dh1U1tLiNXE1voVbjw5ZKp1TjQ9t3joBR2bnn5S3SH9rahz8oHT5UUSzUuQqMphn5dEWqXT6Tg1%2BIWPJ01Z455w1IgZd%2FYw7xbf7%2Bza11wDTVQGmeSMmWNGjQzyLIeTEsYc91FOXYc0aIVaXpFag3rU0jlaeC8PFEtyLVdund%2BH4cpXRRu5snZOLMWI53Z8GO7%2Fpknl20mNaNKOW3K8vDdx3XPRRDTTXznFw9OfklmP%2FwM%3D
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/setFavoriteIngredient.feature

Until June, we want to implement:
- 3.1.6 Read Cloud Recipes Use Case
- 3.1.7 Get Recommendations Use Case
- 3.1.8 Favorize Recipe Use Case
- 3.1.9 Analyze Waterbalance Use Case

### 3.2 Usability
We plan on designing the user interface as intuitive and self-explanatory as possible to make the user feel as comfortable as possible using the app.

#### 3.2.1 No training time needed
Our goal is that a user installs the android application, opens it and is able to use all features without any explanation or help.

#### 3.2.2 Familiar Feeling
We want to implement an app with familiar designs and functions. This way the user is able to interact in familiar ways with the app without having to get to know new interfaces.

### 3.3 Reliability

#### 3.3.1 Availability
Since we do not think of implementing a Serversided connection the Application should run a full 100% of the time!
Update: We care about an own backend API. The Server is running on side of Strato - so Strato is responsible for the availability.

### 3.4 Perfomance

#### 3.4.1 Capacity
~ 10MB
App needs more capacity when entries are created in the local phone storage.

#### 3.4.2 Storage 
While interacting with the User Interface with actions like...
- creating, updating, deleting recipes
- adding water to the waterbalance
- changing settings
- adding favorite recipes
... there are created entries in the local phone storage.

An API is used to get a big list of recipes which the user can read from the app.

#### 3.4.3 App perfomance / Response time
Depends on the device performance.

The Backend API always returns a maximum of 100 datasets. To get more, the "limit" and the "offset" parameter can be set.

### 3.5 Supportability

#### 3.5.1 Coding Standards
We are going to write the code by using all of the most common clean code standards. For example we will name our variables and methods by their functionalities. This will keep the code easy to read by everyone and make further developement much easier.

#### 3.5.2 Testing Strategy
The application will have a high test coverage and all important functionalities and edge cases should be tested. Further mistakes in the implementation will be discovered instantly and it will be easy to locate the error.

### 3.6 Design Constraints
- The Design is following the constraints of Material Design: https://material.io/design/introduction#principles
- Icons used from Google Material Icons
- Keeping everything in Dark Mode
- Color Theming:
	- colorPrimary: #333D4A
	- colorPrimaryDark #222731
    	- colorAccent: #C6A334
    	- colorSoft: #EABE7C
    	- colorHighlight: #BA823F

### 3.7 On-line User Documentation and Help System Requirements
(n/a)

### 3.8 Purchased Components
Currently no purchased components are integrated. As soon as this changes we will list them here.

### 3.9 Interfaces

#### 3.9.1 User Interfaces
The User interfaces that will be implented are:
- Home Page
- Recipe Overview
- Recipe Detail (Read & Edit Mode)
- Waterbalance Page
- Settings Overview
- Need Calculation Page
- Goals Page
- Favorite Ingredients Page

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
