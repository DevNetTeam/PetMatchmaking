##

# Software Requirements Specification

## for

# PetMatchMaking

Version 1.0

Prepared by Georgi Marinov

DevNetTeam

12.03.2020

Table of Contents

| Table of Contents        |
| --- |
| Revision History        |
| 1.        Introduction        |
| 1.1        Purpose        |
| 1.2        Document Conventions        |
| 1.3        Intended Audience and Reading Suggestions        |
| 1.4        Project Scope        |
| 1.5        References        |
| 2.        Overall Description        |
| 2.1        Product Perspective        |
| 2.2        Product Features        |
| 2.3        User Classes and Characteristics        |
| 2.4        Operating Environment        |
| 2.5        Design and Implementation Constraints        |
| 2.6        User Documentation        |
| 2.7        Assumptions and Dependencies        |
| 3.        System Features        |
| 3.1        System Feature 1        |
| 3.2        System Feature 2 (and so on)        |
| 4.        External Interface Requirements        |
| 4.1        User Interfaces        |
| 4.2        Hardware Interfaces        |
| 4.3        Software Interfaces        |
| 4.4        Communications Interfaces        |
| 5.        Other Nonfunctional Requirements        |
| 5.1        Performance Requirements        |
| 5.2        Safety Requirements        |
| 5.3        Security Requirements        |
| 5.4        Software Quality Attributes        |
| 6.        Other Requirements        |
| Appendix A: Glossary        |
| Appendix B: Analysis Models        |
| Appendix C: Issues List        |



# 1.Introduction

## 1.1Purpose

The purpose of this document is to give a detailed description of the requirements for the &quot; **PetMatchmaking**&quot; web application (&quot; **web app**&quot;), and mobile application (&quot; **mobile app**&quot;), (or both generally: &quot; **app**&quot;). It will illustrate the purpose and complete declaration for the development of system. It will also explain system constraints, interface and interactions with other external applications – прим. логване с фейсбук. This document is primarily intended to be proposed to a customer for its approval and a reference for developing the first version of the system for the development team.

## 1.2Document Conventions

ОСТАВЯМ ЗА ПОСЛЕ ЕВЕНТУАЛНО

## 1.3Intended Audience and Reading Suggestions

**ОСТАВЯМ ЗА ПОСЛЕ ЕВЕНТУАЛНО**  **–**

## 1.4Project Scope

The &quot; **PetMatchmaking**&quot;app is a web and mobile app which helps people to find the best pet-partner for their pets based on the user&#39;s resident – permanent or temporary location and other criteria like breed, age of their pet and more. The app also helps people to find the best pet to adopt, abiding by the same criteria, as well as criteria based on the qualities of the current owner of the pet and the perspective adopter. The web app is free-accessed via internet, based in a datacenter. The mobile application should be free to download from either a mobile phone application store or similar services.

Logged-in users can provide their personal information and information about their pets using the web-portal or mobile application. This information will act as the bases for the search results displayed to the user.

An administrator uses the web-portal in order to administer the system and keep the information accurate. The administrator can, for instance, verify pet ownersand perspective pet-adopters and manage user information.

The app needs internet connection to fetch and display results. The app does not need GPS connection, since the user information is not real time but predefined generally. All system information is maintained in a database, which is located on a web-server. The application also has the capability of representing both summary and detailed information about the pets, their owners and the perspective pet adopters.

## 1.5References

**ОСТАВЯМ ЗА ПОСЛЕ ЕВЕНТУАЛНО**  **–**

# 2.Overall Description

## 2.1Product Perspective

Thesystem will consist of three two parts: one mobile application and one web portal. Both mobile and web app will be used to input and extract information and the web app will be used also for managing the information about the pets, owner and perspective adopters as well as about the system as a whole.

Since this is a data-centric product it will need somewhere to store the data. For that, a database will be used. Both the mobile application and web portal will communicate with the database, however in slightly different ways. The mobile application will use the database to input and get data while the web portal will also manage data, user-rights and the system as a whole. All of the database communication will go over the Internet.

## 2.2Product Features

With the app, the users will be able to search for pets. The result will be based on the criteria the user inputs. There are several search criteria and it will be possible for the administrator of the system to manage the options for those criteria that have that.

The result of the search will be viewed either in a list view, accompanied by a picture, if such is stored.

## 2.3User Classes and Characteristics

There are three types of users that interact with the system: non-logged-in users, logged-in users and administrators. Each of these three types of users has different use of the system so each of them has their own requirements.

The **non-logged-in users** can only use the application to read articles, make a search, or comment in a forum. This means that the user have to be able to search for pets based on the chosen criteria, see published data, read that data or see uploaded photos, enter a forum and comment there. In order for the users to get a relevant search result there are multiple criteria the users can specify and all results matches all of those.

The **non-logged-in users** can also create content, including posting announcement, uploading pictures.

The **administrators** are managing the overall system so there is no incorrect information within it via the web portal. An administrator can manage the information for each announcement as well as the options for both the mobile and web apps.

## 2.4Operating Environment

## 2.5Design and Implementation Constraints

Both the web and the mobile apps will be constrained by the **capacity of the database**. Since the database is shared between both application it may be forced to queue incoming requests and therefor increase the time it takes to fetch data.

The Internet connection is also a constraint for the application. Since the application fetches data from the database over the Internet, it is crucial that there is an Internet connection for the application to function.

## 2.6User Documentation

**ОСТАВЯМ ЗА ПОСЛЕ ЕВЕНТУАЛНО**  **–**** да напиша, че ще има **** user manual**

## 2.7Assumptions and Dependencies

**ОСТАВЯМ ЗА ПОСЛЕ ЕВЕНТУАЛНО**  **–**

# 3.System Features

Functional requirements:

**ID: FR ..**  **- TITLE:  Search**

DESC: Given that a user enters the app, then the first page that is shown should be the ………. page. The user should be able to choose what to do ………… enter the MatchMaking section, ………. .

**ID: FR…**  **- TITLE:  Search**

DESC: Given that a user enters the app,

and the users chooses to enter the MatchMaking section

and the users chooses the search option

then the user should be able to search for a pet, according to 2 search options. The search options are pet breed and pet town and ………. There should also be a free-of-choice search option. A user should be able to select multiple search options in one search.



**ID: FR…**  **- TITLE: Search result in a list view**

DESC:

 Search results can be viewed in a list. Each element in the list represents a specific pet. Each element should include the pet name, pet breed, pet town, pet years,pet photo and an information link.

**ID: FR…**  **- TITLE: Selecting the information link**

DESC: A user should be able to select the information link, which is included on all result items.

When the user selects the link

then the link should disclose to the user additional information if added by the pet&#39;s owner.

**ID: FR…**  **- TITLE: Search by**  **town**

DESC: A user should be able to select a town from a drop-down menu.

When the user selects the town and the user clicks the search button,

then the result fetched is only the pets in the selected town.

**ID: FR**** … **** – TITLE: Search by **** breed**

DESC: A user should be able to select a pet&#39;s breed from a drop-down menu. When the user selects the breed and the user clicks the search button,

then the result fetched is only the pets in the selected breed.

**ID: FR**** … **** – TITLE: Search by **** town and breed**

DESC: A user should be able to select a town and a pet&#39;s breed from the separate drop-down menus.

When the user selects the town and the user selects the breed and the user clicks the search button,

then the result fetched is only the pets in the selected town and the selected breed.

**(с буда да координирам дали  после да има и по години на кучето евентуално )**

**ID: FR**** … **** free-of-choice search**

DESC: A user should be able to conduct a search by not choosing neither filtering option.

When the user does not choose a filtering option and the user clicks the search button,

then the result fetched is all the pets from all the towns and all the breeds.

**ID: FR**** … **** TITLE: No match found**

DESC: When the user selects the town and/or the user selects the breed and no match is found

then the user should be informed that the search finds no matching announcements and the user should be kept on the search page in order to get the possibility to conduct a new search right away.

**ID: FR… TITLE:  Sorting results**

DESC: When viewing the results in a list, a user should be able to sort the results according to any of the filtering criteria.

When sorting by pet breed, then the results should be ordered alphabetically, ascending.

When sorting by pet town, then the results should be ordered alphabetically, ascending.

**ID: FR… TITLE:  Profile page – edit account**

**ID: FR…**  **–примерно раздел:**  **РЕГИСТРИРАНИ ПОТРЕБИТЕЛИ**

Feature: Create an account

Scenario: Required information for registration

Given the user wants to create an account

And the user does not have an account for the same username and/or e-mail address

When the user clicks the sign up link and the user provides username And password And e-mail address Then the user should be able to create and account and receive a verification message;

Scenario: Confirmed registration

Given the user has receive a verification message Then the user should be able to log in from the LogIn section.

**ID: FR…**

**Feature: User log-in**

In order to use the app as a registered user

A user Should be logged in to the app

Scenario: Successful log-in

Given the user wants to log in When the user provides an username And the user provides a password

Then the user should be logged in to his/her account.



**ID: F.**  **- TITLE: Retrieve password**

**ID: FR. Feature: Manage information**

**ID: FR… Feature: Administrator log in**

**ID: FR… Feature: Manage**  **листа с градовете и**

**ID: FR**** … ****Feature:**  **Manage**  ** листа с породите**

**ID: FR**** … **** Feature: Manage **** PET **** information – да внимавам да не се припокрие с др**

**ID: FR**** … **** Feature: Manage users**

# 4.External Interface Requirements

## 4.1User Interfaces– да добавя wireframes

A first-time user of the app should see the home page with a log-in and sign-up options when he/she opens the application, see Figure. If the user has not registered, he/she should be able to do that on the sign-up page.

Every user **should have a profile page** where they can edit their username, e-mail address, phone number and password, as well as optional additional data, like does the user want to offer a pet for **matchmaking** or/and to offer a pet for **adoption,** breed of the pet, years of the pet, to add additional information as text up to 200 symbols, to upload a picture of the pet - see Figure. Also, the user can set the app to his/her preferred language.

Anyways, no matter **logged-in/sighed-up or not** , the user should be able to see the two sections of the app – **Matchmaking** and **Adoption,** as well as **additional information** and to choose by clicking then enter in any of them. When entering a section, a respective search menu appears - see Figure. Here the user should be able to choose the criteria of the search he/she wants to conduct.

In Figure, the list view for the results is shown.

In **both sections** when a user searches by **breed** , this view should be the default one. Each result item includes information about the pet - breed of the pet, years of the pet, additional information as text, the picture of the pet if any.

A **logged-in user** should be able to perform the same actions as the non-logged-in user and additionally to upload announcement for matchmaking or adoption in any of the two sections (Matchmaking and Adoption).

An **administrator** should be able to log in to the web-portal where he/she can administer the system by for instance editing an announcement, or user information, or banning an announcement if inappropriate.

The section Additional information (see Figure …) should contain headings hyperlinked to another page, with pictures next to the headings. When clicking a heading, the user should be transferred to the page with the whole text of the respective article, to which the heading is hyperlinked (see Figure …).

## 4.2Hardware Interfaces

Since neither the web or mobile apps have any designated hardware, it does not have any direct hardware interfaces.

## 4.3Software Interfaces

The communication between the database and the web portal and mobile app consists of operation concerning both reading and modifying the data.

## 4.4Communications Interfaces

The communication between the different parts of the system is important since they depend on each other. However, in what way the communication is achieved is not important for the system and is therefore handled by the underlying operating systems for both the mobile the web app.

# 5.Other Nonfunctional Requirements

## 5.1Performance Requirements

## 5.2Safety Requirements

## 5.3Security Requirements

## 5.4Software Quality Attributes

# 6.Other Requirements

Appendix A: Glossary

Appendix B: Analysis Models

Appendix C: Issues List