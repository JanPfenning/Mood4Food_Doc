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
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=ApiRecipe.drawio#R7Vtbc5s4FP41ftwdzMUmjzFxs51Jp916d5o87SggjFpAHiHHdn%2F9HhlhQCK%2BxQbXTSbTooOQxPedmw5Kz%2FKS5T1Ds%2BgTDXDcM41g2bPueqbZNywX%2FhOSVS5xbCmYMhLITqVgQn7i4kkpnZMAZ7WOnNKYk1ld6NM0xT6vyRBjdFHvFtK4PusMTbEmmPgo1qXfSMCjXOo6Rin%2FC5NpVMzcN%2BSdBBWdpSCLUEAXFZE17lkeo5TnV8nSw7EAr8Alf%2B7DK3c3C2M45fs8EP8MBrff3HBx%2F8%2F8eTz579MXf%2FGHHOUFxXP5wv9mmMkF81WBAsdLmGMU8SQGQR8uM87oD%2BzRmDKQpDSFnqOQxLEiQjGZptD0YZUwsDV6wYwTwPdW3khIEIhpRouIcDyZIV%2FMuQBtAhmj8zTA4gUMaOlvXCwfxsTLikgicI9pgjlbQZfi7kCyIdXRls1FyW0hiiq0FhwiqU3TzcAl4HAhMT8Af1PH%2F%2BP1om9dGPqWhv5klXGcXC8DzoUxYGsMaNjDKODssQJ%2FhGbifsYR4xOOuAp%2Fz7SM9Y%2FGFdwJQ3nnJB7FqSE60BG1GhC1zoWosweiAYQ42aSMR3RKUxSPS2kVaVVfnynnNIEbOA1uRYAVg8xwmktkAHePQz2jc%2Bbj3eoiXmArNwzHiJOXegxvglo%2B%2BoUSWErJqVu3kr6jsAVaN8VcPqUQtlnG8RwONA69mPg%2FQDTBiPkRXHyEhEcjtnQX%2FVccSoVYGEiyZQtSQpryJuNRjCqEH%2F%2F8RmW%2BQkDFqjZ9qmZln8ushtdsVoN2zMpSWR22a1auxuFngTAYUzqbi3WGBMP24GqtSsO%2Fc6u6uXyrArjZ6lGOv248iXTsT6do3i1lepa3VruStZ3WKNU0N4Yt%2FYot8tnNVomG5p7REABHq0q3meiQHTBPfUMLF%2FmIJ%2FUJpnOExtXT8rLPA6UzqSnfMecrqWBozmldT%2FGS8MdSjaD1VLlTapRorKrq9VjXvaea6jUroupq0MBtzoq9oeW8MZAUKrlTd4sRT6e7b%2FJDxborjmi83q%2BZxt9zLCe4ypigZlqm0XVM6Os1kU3WG1KWl9b8iKTTtXr4ZIaz6%2BXHUfix%2Bp3zo1dN3oP2Rmt3R%2B2W9rCOEk2tm%2FNEbW2eYQtRu6%2FXjSYRKIppPJBMLI6G8M%2FXa3cOakJvdZ7Q93%2BB8lMHzsHe1zm0tRNXjNZuKaW3jTacg14%2Bm%2BBYfBw0jc8pvl53oOZyG%2FS7cwe%2FQNms3Fe15g4G%2B7oDtx13oNa7bfc87kCbp5VcQS%2F7yVzhDnNE4t8oP7C7zw%2FeK35bVHR32aSjkp%2FTUn7gyPzxvCU%2Fvdij6%2BC2j85CkTr95DxUUGuo2bT6zdkcHGHEJyuiFtcVK72AImrF%2F%2FgxyjLi58IPJC5e4HiHsTkKtzODME%2FtMN6mKDddKopxlKIcFgTarLbvrQVnChuHenvl7JHpKgcWt3dvJzboByI9moaEJYBL04mLiCbP82x3mtjNhtBWEG84nOS2mf6Zw07t%2F4CvbW1Y5WV9A7P0tMhDqS%2FOcyuUydOQ2tFGsfcpqGzKzTdHHTMwE5JOH3Ao8LFKyVepg5ZmGfI4JaOQeKHn9RSCJulyYFnOCH7hFTzBsgPL9KDdL9vwK7oz2J2lMDQia14xyvgCZ%2Fw09qY5OHsvcyvSp9NT2nDAFVKQd0L3JdRUv46ej1Foln8LkIez8i8qrPH%2F
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/getApiRecipe.feature
- 3.1.7 Get Recommendations Use Case
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Recommendations_flow.drawio#R7Vpbk6o4EP41Pu4WEBjlcXQuO1tna6eOtXXmPGagldQAoUK87a%2FfRIJI4oUZBT3W%2BqCkE5LwdffX6ZYeGiXLZ4az6C8aQtxzrHDZQw89x7EtNBA%2FUrIqJJ6rBFNGQjWoEozJv1DeqaQzEkJeG8gpjTnJ6sKApikEvCbDjNFFfdiExvVVMzwFQzAOcGxKf5CQR4V04FmV%2FA8g06hc2bZUT4LLwUqQRzikiy0ReuyhEaOUF1fJcgSxBK%2FEpbjvaU%2FvZmMMUt7khvnznx9vT%2FOX4ccP94140d%2FJ3P1NzTLH8Uw98D85MLVhvipR4LAUawwjnsRCYIvLnDP6ASMaUyYkKU3FyOGExLEmwjGZpqIZiF2KidFwDowTge%2B96khIGMplhouIcBhnOJBrLoQ1CRmjszQE%2BQCWaJlPXG5fzAnLLZFC4BloApytxJCNQSptlOaomotKt64SRVtqLXWIlTVNNxNXgIsLhfkn8HdM%2FF9uF33kXBf6yEB%2FvMo5JLerAQ9dlwZcQwMG9mIWQfagwR%2FhTPbnHDM%2B5pjr8PccZK0%2Fhq5Ez2Sies7CKF4N0YGJKNqBKGoLUa8BoqEIcapJGY%2FolKY4fqyk20jr9vpOOaeJ6IA0vJcBVk6SQVpIVAAffA31nM5YAMfNRT7AQd0wiDEn83oM3wW1uvWVErGVSqcaT9l9TVvC6qbA1V2awjbb%2BLoOByYvAQjBi%2BQQyAVoT4ZSWUST91m%2Bh0i2FKp5yUR8gta9ZLAH0C0vGezwErctL%2FENhFN6mp%2BURB%2FDhLfjNgJ9tnqTseB3r2z%2BVKFh3XhY1lqrY2HjqLspOyys%2FdAp0m7ol8oaymPniW7q3GlW5TdzU4E%2FXm0Ny%2BSA%2FAAd9HevUxlgMeNZOaBMgLZMdAV5qzbKaXYhXm9saP2LGJpf179rtWNne8z5qdlwpA4i%2B4b7B4e3ZMRmfvkdJiKERWb82hx17eMxDLNAWaQrDW9CU77r4HeRUGfbdaCdHbFuc8DoJNjZZpZ5Go%2B0Gtxqoa2KdGcPbqVtHicd1JB0TmQZT6tNOCeHs3OfS20zYX4G%2BQQpLMT3dwhIJmOU9Y5z4cqORVPx9a03Qr370cda8pJOGYQE1ju0JkyYjWPdv5pFj5vhA9e%2FOj5oknVfCx%2FYnfEBasoHXkd84GkRu2EW%2Btljh7GO18Xx1qxTPJA8i9c71%2BjkVplBz4oRujgz3P3PDPtt9SgzdFSeQq6Wj%2BjFxDMRg76O30XG0DcscAyx%2FGdP3Mhvlwv0ZM6%2FOBWYRcjrpYLukoZ%2B00OC3w0X6KVqd9ANF7j24eLEkfEtkYdZ1v1GsUw7HoBjEt%2FwWUJPHi9PIOVivwSBfPIssW69AiMCKvmv7qms4jdkFaejUgTSUgKvpYqnd7d7nVZZwjGrGFXqURDFulRR5B%2B3Sxl6%2BuHu%2BOu6Y8r4BQoTX%2FfyzpxXC71ewyPB2fyrySsIh17qkKq45CsdyPF2A3j%2BdzpEs3oDsFBA9R4levwP
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/getRecommendations.feature
- 3.1.8 Favorize Recipe Use Case
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=favorizeRecipe.drawio#R7Vvbkps4EP0aPzrFRdjMY%2BIZZ5OaqdpaJ5XkUQPikgByCXls79evAMmAZI%2FxmItD1i9GjcSl%2B5zuVktMzEW8%2B0jgOnjCLoomhubuJub9xDB0zbTZXybZFxILcIFPQpd3KgWr8F8kRnLpJnRRWutIMY5ouK4LHZwkyKE1GSQEb%2BvdPBzV77qGPlIEKwdGqvRb6NKgkNqWVsr%2FQqEfiDvrGj8TQ9GZC9IAunhbEZkPE3NBMKbFUbxboChTntBLMW554uzhwQhKaKMBG38Dn58%2BYP37Fzugy1n8%2BdtUnxWXeYHRhr8xf1q6Fypgl2HaZo0PAY0jJtPZIXubdXY%2BpZDQFYU0O%2B%2BFUbTAESb5QFPLf1lnSvAvVDnjefyM%2BhL8vV4QoWhXEfGX%2BohwjCjZsy787B3XLwfYjDe3pbVMLgoqhhIyyPHhH65bqpAdcC1eotF5A426DGO8iQkNsI8TGD2U0qqmM02EDJDvo9BPmOwZU4pjdgIl7vsM4dlF1igpJJxB9tu0nuINcVADvGRv8KpxCIogDV%2FqLDqmbD70bxyyZzkYVdesmlV1S7IXg52PKB8lmezwGFdY0Vas%2BDVFRLEkwyiViFHTeoITmRhcBLk5HWYDdmHVznHoujkWtkFI0WoNc8NsmZtlMoI3iYuyN2iJRbakb5VF4AiLjM5YdKfof7VPKYrHawHD1m7KBOLCVQp8Gq%2F6LXBj6tcV9a9QlKU4hvYPckIWfVk6Q1gkEO3pY5hSxUClovQTqqzYDhKHBxCQqdXDCT0Wz6U477Gf03mcByciQsVAunHEQqAzCxljjvSiY9eR%2FpCwCbvO%2B430hqlY8RFDt8qye0RhGKXjpZZig%2BG5BUbNLbMfblnGwNyyFCveh%2Bk6gvs%2FgVWK9odnVZPZ%2FsCsYvom%2B%2B%2F8%2BnnjR5bkvbNE837Hk76itT%2BXAp5nI0dpQYZXOoqaQee0lWYCRsPJL9N4zizRbZ11SC%2B%2FTwmx4oqt%2BgRTnVZ8wb4fZYF2CV8wYXxnh58cnIzXNUi57KEaNZhnMNXZxu16Bq0vzyDMct4zGP14BrksZsplzJY8g3IfvQ%2FPoM6nFhuSW63iGsyl6hYCHD9v0vMuYZjkWipQH9rDkV2d8iT4OrqLYk6EPNo1%2B0vC%2F6jxvXX2G03ZP2%2FIfo6IKX%2BCK50B0OvAEiRt2xkA4%2Fh9unUG6gRwj9TJQpsgpXg90HywcfhoF0CmJhnW7nd6aKrTw6%2BJlzt6pu7RJn8GOKH24QLCbzAvvIJdVj%2FJ2Uzyx0Drxh%2FLtAV30sL%2Fuee668N%2Fq8vgy9Ez25zdHLPVdeybY3Yls5vXUrtDBaj91G7eMLUzevIdco4Feg7FAoDVVRAEX0bMVXBiJj0YVcH%2FJZhXgHmWqQD0w1S5NAJ6KsFYZg9RG6iVgRvG4DvjokoA2oW0Oo41D1GGHZejskaPywoC4p0jdy5VnWfNkKuuG8gVLTnRLXRz%2FfqEJd1H3uEqB9Hrup9Jo2Xt9ZFFA7UKUtucMH3KFlETD49874%2B8QcE6sjur52it1i5u2FP2Fq1BU5%2FX0z5iU8qrZw1rpG0R2NLfgIr63sayzyPOKpQ5Wn4iSvccBHBDcR1LZaSbN490by2wyw7BdpDjHMPls20B60p8zZriy%2B4EX5dGMLn0Yl0WY6xeYoxa%2FCs36SRom6MX5ovy2JuUK3HTP2LXqbyJ5wYiz2%2FwgckAkaepZ%2BhrX6u8uaZp5Ll2E49on3Ixske6rLvYQditR2pStHzto7QMpkN%2BkjY7Yfr2v0ljzfILwkL%2F5XeY5sN%2F
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/favorizeRecipe.feature
- 3.1.9 Analyze Waterbalance Use Case
	- Flow Diagram: https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Analyse_Waterbalance.drawio#R5Vpbc%2BI2FP41eQyjiyH2YzZJt5lpO5mhO9l9VLAAzxqLyiJAf30lLNmWZIMJty3hgbGOLpbO%2FXzyDX6Yrb5yMp%2F%2ByWKa3iAQr27w4w1CCEL5rwjrgtAPwoIw4UlckGBFGCb%2FUk0EmrpIYppbAwVjqUjmNnHEsoyOhEUjnLOlPWzMUvutczKhHmE4IqlPfU1iMS2oIbqr6L%2FTZDI1b4aDqOiZETNYnySfkpgtayT8dIMfOGOieJqtHmiqeGf4Usz7raW33Binmegy4e%2Fvz%2F%2B8rW8X9y%2Bz6PllMVz1v%2BDbvl7mnaQLfWK9W7E2LJDLSG7LxpepmKWSBuWjPM1c9eeCcDEURKj%2BcZKmDyxlfDMRg81PDRac%2FaS1nvFY9%2FiHMBuiXNBVjaQP9ZWyGRV8LYfo3ijqF1O0hmHN72UlLkOa1iRlaEQryKRcuOKhfNBs3IelqANLY6lkusm4mLIJy0j6VFHrrFasSKRG3qfJJJO0NyYEm8kOmsX3SsXVInOaFRRtQuFWtktu8%2FV3SQS9vmn%2BUE3TeFxZrbVutYpLasGEim1cwcVAdfKtUuU0JSJ5t82vSUh66gtL5F5KbYDAeA6tDrfIXqLYqZ5VNxdvIRD1otovtJbth%2FayOVvwEfWW3WhQeboDlAp7SnUvNWYtzRKBV2l9%2FI2kJBtRT9U4W2QxjbUuLaeJoMM5GanepfTYtqoRPtL6Eyhxj1kmmuzZsfOx%2FI1Ob%2Bd9W7B3oWfnEDUYenAyQ488mTwm%2BTwl608jEwgDWyhw4Hvf80pl0OR%2BB6l87Zc3Lp8mojz6Rx0y0Y44pWNxYv8MLe9cOesW%2F0xXidBuXeYhRVvNhD0AAt2upqpGfeYL5YkUAuW7vH3h7LYIAYKoa1yIOsYFrXG3oAejCNueQIv80NCBsZNJuDlCS%2ByQQt7YvBk2VwPybS8KHauB4fZY5E0IrVxPPhR7aJ7u2OgtdEIiG49zepKwNQg8Y%2FyDkVjVA0SQTT7OlT7RVObuVNGXlP68Yn%2BJnSBW1jkX85cme%2F6V09VWzp88m0TQdglVwNs7n9y91IlzSJkadxB1JaSMZUq0Mcmnpe3V5PxxodR0vd%2Bg6oZ2qOxkBm8xPILd%2BL17JXehFh04nuC6lJTXIzjslHAR%2Bqjg8NYa7uxi9Iu4b7nMtlxRymAiHLTFco1avvUIpkkmMx1J0ao0znPGsySONw67KYhWYfZo0Eyz3dT0KGjQI1fcR4t1EPj5yLfn6%2BU%2FhA42dnkB%2BNnGcJ0LOrtiIeBfzgoGHcLJpRFKXcnCWhWr69%2F2GrZENfermluFvLPONbDczjK3LIhPnrFCp8KIHKCyO%2F6JHLVF54U8IQiPrKZnwG0M%2FvIRrd0T6zlAa7uCM9C4qj3QmTCEkaU3%2BEjoDBg4%2Bhh2S9%2Fa0ZlW3Ud21DQ3Ou14SZP1OFhSx%2BLjeNbjo9NN0MtowTcKhMDrlSMv2Fafi18flMZVk9Bf5D2ZqLtUaZxT5YEKQCy%2FXrm4tzqXv0CABh79P6RHVXD5UUuWmgPNxwNG9zhwcOnv4qMdIfgGB%2BxC5qBb%2BrI3mO9eOJstt4MSLWdsBPOPFg%2BgDz58ynuxM5iLufXokF8Fe%2BdXJ7v9Qne2WuIA9sIAVD98YLrV8t4Auu9F2%2B0HDbZOOPplWMOWQdhDNpaI3Gz01Pkd9KGsT%2F%2F1AUYXTx6An9T5TnXbB3XKFV7yczoIncDZBz5Tz%2FpBnbkdv5LQtecnd%2BfO9DrHLtA1J7xE7Op3Sxv3DlbIuQnE4Y5kz0Xg8Ym%2F3GgIVg6OV4bPgyOVbFafLxfDq2%2FA8dN%2F
	- Feature File: https://github.com/JanPfenning/Mood4Food/blob/master/app/src/androidTest/assets/features/analyseWaterbalance.feature

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
