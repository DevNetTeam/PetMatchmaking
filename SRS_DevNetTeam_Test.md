Software
========

Requirements
============

Specification
=============

for
===

PetMatchMaking
==============

/social network for pets - web application/
===========================================

**Prepared**\*\* by:\*\*

**Georgi**\*\* Marinov\*\*

DevNetTeam
==========

**Version 3**\*\* / \*\*\*\*approved\*\*\*\* /\*\*

**Version date:**\*\* 10.03.2020\*\*

**Software Requirements Specification for PetMatchMaking Web Application**

**Page ii**



**Introduction**

**1.1**

**Purpose**

The purpose of this document is to give a detailed description of the
requirements for the " **PetMatchmaking**" web application (" **web app**"), a
part of the " **PetMatchmaking**" application " **app**". The latter is to
consist of the above mentioned **web app** as well as of a mobile application ("
**mobile app**"), which is going to be released at a later stage of the overall
project and together with the web app will constitute the final long-term
strategic product vision. The current document will illustrate the purpose and
complete declaration for the development of the web app. It will also explain
system constraints, interface and interactions with other external applications
– прим. логване с фейсбук. This document is primarily intended to be proposed to
the customer for his final approval and a reference for further developing the
third version of the system for the development team.

**1.2**

**Document Conventions**

Wherever in the document a blue colored font is placed, the respective
requirement / functionality specifies a high level of significance of the
requirement / functionality. Wherever in the document a **blue bolded** colored
font is placed, the respective requirement / functionality specifies a highest
level of significance of the requirement / functionality.

For a reference of any non-defined currently definitions, acronyms, or
abbreviations, please see Appendix A:Glossary.

**1.3**

**Project Scope**

The scope of the project is the " **PetMatchmaking**" web app, whose main focus
is to help people establish communication on the basis of their love and
affection towards pet-animals. There are 3 main directions to which the app is
targeting:

**matchmaking** , or finding the best pet-partner for users' pets based on the
users' residence –

permanent or temporary location and other criteria like breed, age of their pet
and more;

**meeting** with other people, who have relevant pets' affection and/or similar
interests connected with

animals; this could be common walks, common gatherings, chats, etc.;

searching for **help** from other people. This could be ask for help with
temporary walking the pet, hosting the pet, buying special food for pet, taking
care for pet (e.g. asking for help by elderly people being not able to take the
full necessary care for their pet);

The criteria on which the users could potentially meet, match-make or help each
other is defined in the app by

the definition of the user' profile characteristics as well as on his/her pets'
description.

The app could also potentially help people to find the best pet to adopt,
abiding by the same criteria. The web app is free-accessed via internet, (to be)
based in a datacenter.

Logged-in users can provide their personal information and information about
their pets using the web-portal. This information will act as the bases for the
search results displayed to theuser.

An administrator uses the app in order to administer the system and keep the
information accurate. The administrator can, for instance, verify pet owners and
manage userinformation.

The app needs internet connection to fetch and display results. The app does not
need GPS connection, since the user information is not real time but predefined
generally.

All system information is maintained in a database, which should be located on a
web-server. The application also has the capability of representing both summary
and detailed information about the pets, their owners and the perspective pet
sitters / adopters.

**1.4**

**References**

<https://seilevel.com/requirements/specifying-quality-requirements-with-planguage>

![](media/06143ae61b4d399b8eb8960bf637ad20.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 2**

**2. Overall**\*\* Description\*\*

**2.1 Product**\*\* Perspective\*\*

The app is a new, self-contained product. The system will consist of web app and
a database. The **web app** will be used to input, extract and manage
information, including user information,

information about the pets, their owner(s), user-rights, as well as system
features.

Since this is a data-centric product it will need somewhere to store the data.
For that, a **database** will be used. The web app will communicate with the
database. All of the database communication will go over the Internet.

**2.2 Product**\*\* Features\*\*

With the app, the users will be **able to** search for pets for mating purposes
(matchmaking), look for event connected with pets, organize events connected
with pets, ask for help connected with pets or offer help connected with pets.

The **result** will be based on the criteria the user inputs. There are several
search criteria and it will be possible for the administrator of the system to
manage the options for those criteria.

The result of the search will be viewed either in a **list view** or in a **map
view** and will be accompanied by

**text** as well as by a **picture** , if such is stored.

**2.3 User Classes and**\*\* Characteristics\*\*

There are three types of users that interact with the system: Non-registered
user, logged-in users and administrators. Each of these three types of users has
different use of the system so each of them has their own requirements.

The **Non-registered users** can only use the application to see the Home page,
see the Info page, read articles if such are placed there, use the Contact us
form.

The **Logged-in users** will be able to use the functionalities accessed by
Non-registered users, also to use the search features, to manage their account
by placing and editing user data, see published requests, read the information
in the requests including seeing the uploaded photos in the requests. In order
for the users to get a relevant search result there are multiple criteria the
users can specify.

The **administrators** are managing the overall system so there is no incorrect
information within it. An administrator can manage the information for each
request/announcement as well as to specify the drop- down menus by adding items
there.

**2.4**

**Operating Environment**

The app operates via any kind of web browser.

**2.5 Design and Implementation**\*\* Constraints\*\*

**2.5.1**

**Design**

The system design consists of Front end and Back end,

including Database:

-   The **Front end** includes HTML, Bootstrap andCSS;



The **Back end** includes PHP and MySQL.

**2.5.2**

**Constraints**

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 3**

The app will be constrained by the **capacity of the database**. The database
may be forced to queue lots of incoming requests and therefore increase the time
it takes to fetch data.

The **Internet connection** is also a constraint for the application. Since the
application fetches data fromthe database over the Internet, it is crucial that
there is an Internet connection for the application to function.

The **legal constraints** for using the app are connected with the exposure of
personal data in the app and the respective user consent that should be ensured
regarding the local personal data legislation, as well as General Data
Protection Regulation (GDPR).

**2.6**

**User Documentation**

The user documentation consists of the current SRS, as well as User manual.

**3. System Features and Functional**\*\* requirements\*\*

**3.1 User Class 1 – Non-registered user**\*\* functionalities\*\*

**Overview:** Non-registered users should be able to see the Home page, the Info
section with all its pages and the Contact us page and to read the content of
these sections and pages.

**3.1.1**

**ID: FR1**

**DESC:** Given the user has entered the app

Then the user should be able to see the Login form

**3.1.2**

**ID: FR2**

**DESC:** Given the user has entered the app

Then the user should be able to see a Sign-up link and the user should be able
to enter a Sign-up form

**3.1.3**

**ID: FR3**

**DESC:** Given the user has entered the app

Then the user should be able to reach the Info section and the user should be
able to read all the content of the Info section

**3.1.4**

**ID: FR4. Feature: Contact us form**

**Overview:** Non-registered users should be able to send messages using the
Contact us form.

**DESC:** Given the user has entered the app and the user has entered the
Contact us form When the user wants to send a message

And the user has entered Message title and Message content and Name and an
e-mail address Then the user should be able to send a message and to see a text
verifying the successful sending.

**3.1.5**

**ID: FR5. Feature: Create an account**

Scenario: Required information for registration Given the user wants to create
an account

And the user does not have an account for the given username and/or e-mail
address

When the user selects the sign up link And the user provides a first name And an
e-mail address and a password And successfully confirms the correct password,

Then the user should be able to create an account and receive a verification
message; Scenario: Confirmed registration

Given the user has receive a verification message

Then the user should be directed automatically to the Requests page of the app.

**3.2 User Class 2 – Logged-in**\*\* User\*\*

**Overview: Logged-in Users** should be able to see and use the above-described
sections of the app which are visible and usable by non-registered users (see
art. 3.2…..) except FR1, FR2 and FR5, as well as to see and use the below
described functionalities applicable for Logged-in User.

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 4**

**3.2.1**

**ID: FR6. Feature: User log-in**

**Overview:** In order to use all the functionalities of the app applicable for
logged-in users, a user should be logged in to the app.

Scenario: Successful log-in Given the user wants to log in

When the user enters the app and the user provides a username And a password If
the username and password are existing and corresponding and correct

Then the user should be logged in to his/her account and directed automatically
to the Requests section.

**3.2.2**

**ID: FR7. Feature: Profile page – edit account's information**

**DESC:** In order to manage (add, edit or delete) information, a user Should be
logged in to the app Given the user is logged in and the information exists

When the user wants to edit his/her account information Then the user should be
able to edit the information in a form. **Scenario: Delete information in
mandatory**\*\* fields\*\*

When the user deletes the information from a mandatory field

And the user does not enter another information in the mandatory field Then the
user should NOT be able to submit the form.

**3.2.3**

**ID: FR8. Feature: Search**

**DESC** : Given that a user enters the app, And the users selects the Requests
section

And the users selects the All Requests sub-section

then the user should be able to perform a search, according to 2 search
criteria. The search criteria are location and type of the request. There should
also be a free-of-choice/Show all search option. A user should be able to select
one or more search criteria in one search.

**3.2.4**

**ID: FR9. TITLE: Search result in a list view**

**DESC** : The default view of the search results is a list. Search results can
be viewed in a list.

Each element in the list represents a specific user request.

Each element in the list should include the type of request, date of request,
pet species, pet name, request/pet town, name of the user who requested, short
subject of the request, pet photo and an information link/ **button**.

**3.2.5**

**ID: FR10. TITLE: Search result in a map view**

**DESC** : Search results can be viewed on a map. On the map, the location,
according to the user's request, is shown.

A specific pin will represent the request's location. On each pin there should
be a short information according to what is specified in the corresponding
request.

The map view should have a default zoom.

**3.2.6**

**ID: FR11. TITLE: Selecting the information link**

**DESC** : A user should be able to select the information link/ **button** ,
which is included on each of the result items in the list view.

When the user selects the information link/ **button** then the link/ **button**
should disclose to the user

the whole information of the request provided by the pet's owner, including
additional information if added by the pet's owner

pets in the request section, including all the information of the pet, added by
the pet's owner;

pet owner data section, including all the information of the pet's owner, added
by the pet's owner;

a map view, showing the location of the address in the request, shown on a map.

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 5**

**3.2.7**

**ID: FR12. TITLE: Search by town**

**DESC** : A user should be able to select a town from a drop-down menu. When
the user selects the town and the user clicks the search button,

then the result fetched is a list consisting of only the requests, for which (an
address and/or neighborhood in) the selected town is specified.

**3.2.8**

**ID: FR13. TITLE: Search by request's type**

**DESC** : A user should be able to select a requests' type from a drop-down
menu. When the user selects

the requests' type and the user clicks the search button,

then the result fetched is a list consisting of only the requests for which the
selected type is specified.

**ID: FR14 – TITLE: Search by multiple criteria**

DESC: A user should be able to select both a town and a request's type from the
separate drop-down

lists.

When the user selects the town and the user selects a request's type and the
user clicks the search

button,

then the result fetched is a list consisting of only the requests matching ALL
of the selected criteria.

**ID: FR17 free-of-choice search**

DESC: A user should be able to conduct a search by not choosing neither
filtering option. When the user does not choose a filtering option and the user
clicks the search button, then the result fetched is a list of all the requests
published in the app.

**ID: FR18 TITLE: No match found**

DESC: When the user selects the town and/or the user selects the breed and no
match is found

then the user should see a message informing that the search finds no matching
requests Then the user should be kept on the search page in order to get the
possibility to conduct a new search right away.

**ID: FR…**

**Feature: Add new request**

DESC: The user should be able to add a new request. In order to add new request

A user should fill the mandatory fields In a form.

**Scenario: Filling in mandatory fields**

Given the user wants to fill the mandatory fields

When the user selects one or more of his/her added pets And the user selects
location And the user selects type of the request And the user selects Start
date And the user enters About information And the user enters a phone number

Then the user has filled the mandatory fields of the form.

**Scenario: Filling in optional fields**

Given the user wants to fill in optional fields in the form

When the user provides End date And the user checks the Offering payment option
Then the user has filled in optional fields in the form

**Scenario: Adding a new request with mandatory fields** Given the user has
filled in the mandatory fields of the form When the user submits the form

Then the new request containing the data filled in the mandatory fields should
be added.

**Scenario: Adding a new request with mandatory And optional fields**

Given the user has filled in the mandatory fields of the form

And the user has filled in one or more optional fields of the form When the user
submits the form

Then the new request containing the data filled in the mandatory And in the
optional fields should be added.

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 6**

**ID: FR…**

**Feature: Edit a request**

DESC: The user should be able to edit each one of his request, one at a time.
Given the user wants to edit a request

When the user selects one of his/her requests And the user edits, adds or
deletes information And the user submits the form

Then the request should be edited.

**Scenario: Delete information in mandatory fields**

If the user deletes the information from a mandatory field Then the user should
NOT be able to submit the form

**ID: FR…**

**Feature: Delete a request**

DESC: The user should be able to delete each one of his request. Given the user
wants to delete a request

When the user selects one of his/her requests And the user selects a delete
option Then the request should be deleted.

**ID: FR…**

**Feature: Add a new**\*\* Pet\*\*

DESC: The user should be able to add a new pet. In order to add newpet

A user should fill the mandatory fields In a form.

**Scenario: Filling in mandatory fields**

Given the user wants to fill the mandatory fields

When the user enters a name And the user selects species And the user enters
About info Then the user has filled the mandatory fields of the form.

**Scenario: Filling in optional fields**

Given the user wants to fill in optional fields in the form

When the user provides pet's sex and birthday And the user enters Food habits
And the user uploads a

photo of the pet

Then the user has filled in optional fields in the form

**Scenario: Adding a new pet with mandatory fields**

Given the user has filled in the mandatory fields of the form When the user
submits the form

Then the new pet containing the data filled in the mandatory fields should be
added.

**Scenario: Adding a new pet with mandatory And optional fields**

Given the user has filled in the mandatory fields of the form

And the user has filled in one or more optional fields of the form When the user
submits the form

Then the new pet containing the data filled in the mandatory And in the optional
fields should be added.

**ID: FR…**

**Feature: Edit a pet**

DESC: The user should be able to edit each one of his pets, one at a time. Given
the user wants to edit a pet

When the user selects one of his/her pet

And the user edits, adds or deletes information And the user submits theform

Then the pet should beedited.

**Scenario: Delete information in mandatory fields**

If the user deletes the information from a mandatory field Then the user should
NOT be able to submit the form

**ID: FR…**

![](media/e1066fd7a53e26ede37fd59d7ba5de37.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 7**

**Feature: Delete a pet**

DESC: The user should be able to delete each one of his pets. Given the user
wants to delete a pet

When the user selects one of his/her pets And the user selects a delete option
Then the pet should be deleted.

**3.3 User Class 3 –**\*\* Administrator\*\*

**ID: FR26 Feature: Administrator log in**

**ID: FR28 Feature: Manage листа с градовете и**

**ID: FR29 Feature: Manage листа с породите**

**ID: FR30 Feature: Manage restaurant information – да внимавам да не се
припокрие с 31**

**ID: FR31 Feature: Manage users**

**4.**

**External Interface**\*\* Requirements\*\*

**4.1**

**User Interfaces**

**4.1.1**

**Login screen**

A non-registered user of the app should see the home page with a log-in and
sign-up options when he/she opens the app. If the user has not registered,
he/she should be able to do that on the sign-up page.

On the Login page there should be the following items:

Link to "Info" section on the

Navigation bar

Link to "Contact us" form on the

navigationbar

Title "Signin",

input field "Email address" input field "Password"

Button named "Sign in" Link named "Sign up"

**4.1.2**

**Sign-up screen**

![](media/3ad3534ea4f2439d4d78edb135be5849.jpg)

![](media/c5a43a6ccd6345d5efc9059c060ff8aa.jpg)

![](media/37113664c62e4b99c0854b9c98f77fbf.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 8**

When selecting the Sign up link, a user should be directed to a sign up form

In the sign up form there should be the following items:

on the Navigation bar – Company's logo on the Navigation bar - Link to "Info"
section

on the Navigation bar - Link to "Contact us" form

Title "Sign in",

Input field "First name" Input field "Last name" Input field "Enter e-mail"

Text "We will never share your e-mail with anyone else"

Input field "password"

1.  Input field "confirm password"

2.  Submit Button named "Signup"

3.  Text "Already have anaccount?"

4.  Link to "Sign in" form

**4.1.3**

**Contact us screen – non-logged-in users view**

on the Navigation bar – Company's logo

on the Navigation bar - Link to "Info" section on the Navigation bar - Link to
"Home" page Title "Tell us what's on your mind",

Input field "Message title" Input field "Message text" Input field "Your name"

Input field "Your e-mail address"

Submit Button named "Message us"

**4.1.4 Request Section**  **All**\*\* requests screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

Text "Signed in as \&lt;*First and Second name of the user*\&gt;"

**Below the Navigation bar – Filtering interface section**

Text "Requests"

Drop down list Filter for location, named

"City"

![](media/cd7bd695f401387a237fcf442db2e72f.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 9**

1.  Drop down list Filter for type of requests, named"Type"

2.  Check box named "Only futurerequests"

3.  Button named"Filter"

4.  Button named "Filter all on amap"

**Results section**

1.  RESULTS LISTshowing

-   ON THE LEFT: the type of request, date of requested event, Location of
    request,Reward

information (if any), Name of requested user, button named "View",



ON THE RIGHT: Picture of the pet in the request (if any);

**4.1.5 Request Section**  **Add a new request**\*\* screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

Text "Signed in as \&lt;*First and Second name of the user*\&gt;" **Submit
form**\*\* section\*\*

Text "NewRequest:"

Check box named "Select one or more pets for this request"

1.  Drop down list Filter for location, named "Search address, area or location"

2.  Drop down list Filter for type of request, named"Type"

3.  Date-type input field,named

"Start date"

1.  Date-type input field,named

"End date"

1.  Check box named"Offering reward"

2.  Text Input field,named

"Description"

1.  Text Input field, named "Phone number forcontact"

2.  Submit button named "Publish therequest"

![](media/33c5087518a83457112df6b26ba56473.jpg)

![](media/d92a6cd19f4692d8f9b3b48a5442736d.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 10**

**4.1.6 Request Section**  **My requests**\*\* screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

*Text "Signed in as \&lt;First and Second name of the user\&gt;"*

**Results section**

RESULTS LIST showing for each result:

-   ON THE LEFT: the type of request, date ofrequested

event, Location of request, Reward information (if any), button named "Delete",
button named

"Edit", button named "View",



ON THE RIGHT: Picture of the pet in the request (if any);

**Request Section**  **View a request Overview screen**

**4.1.7**

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

*Text "Signed in as \&lt;First and Second name of the user\&gt;"*

**View section** /below navigation bar/:

**Button named Request Overview**

 **when pressed exposes:**

Text: "Requested by \&lt;Names of the

user requested\&gt;"

Text: "Type of request: \&lt;Type of the request\&gt;"

1.  Text: "Date of request: \&lt;Date of the request\&gt;"

2.  Text: "Location: \&lt; Location of the request\&gt;"

3.  Text: "Rewardinformation:

\&lt;Description of the terms with regard to the reward if any\&gt;"

1.  Text: "Description \&lt;Description of the request ifany\&gt;"

2.  Photo of the pet ifany

**Map** /below View section/:

1.  Pin on the map pointing to the location /town, neighborhood/ of therequest

**Button named Pets in the request**

**Button named \&lt;Names of the user requested\&gt;'s profile**

![](media/00d3ef82391b071969a31e27b3ae5cc1.jpg)

![](media/f2a33fcb1a84b0136dede4297653091e.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 11**

**4.1.8 Request Section**  **View a request – Pets in the request**\*\*
screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page

1.  Link to "Sign out" option \_Text "Signed in as \&lt;First and Second name of
    the__user\&gt;"\_

**View section** /below navigation bar/: **Button named Request Overview Button
named Pets in the request**  **when pressed**\*\* exposes:\*\*

Text: "Sex: \&lt;Pet'ssex&gt;"

Text: "Birthday\&lt;Pet's birthday\&gt;" if any

1.  Text: "Food habits: \&lt;Food habits if any\&gt;"

2.  Text: "About: \&lt;Description of the request ifany\&gt;"

**Button named \&lt;Names of the user requested\&gt;'s profile**

**Map** /below View section/: Pin on the map pointing to the location /town,
neighborhood/ of the request

**Request Section**  **View a request – Owner's profile screen**

**4.1.9**

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page

Link to "Sign out" option

*Text "Signed in as \&lt;First and Second name of the user\&gt;"*

**View section** /below navigation bar/:

**Button named Request Overview Button named Pets in the request Button named
\&lt;Names of the user requested\&gt;'s profile**  **when pressed exposes:**

Text: "Name: \&lt;First and Last names of the user requested\&gt;"

Text: "Birthday\&lt;User's birthday\&gt;" if any

1.  Text: "Rating: \&lt;User's rating \&gt;" if any

2.  Text: "About: \&lt;Description of the user\&gt;" ifany

3.  Text "All \&lt;First and Last names of the user requested\&gt;'spets"

4.  Photos, resp. names of the user's pets ifany

![](media/e783f3225a071cd6ade3b22a8c3ec1d4.jpg)

![](media/3d1fbf9bbaa0e682104dabb764ab048b.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 12**

**Map** /below View section/: Pin on the map pointing to the location /town,
neighborhood/ of the request

**4.1.10 My Pets Section**  **Add a Pet**\*\* screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page

Link to "Sign out" option

Text "Signed in as \&lt;*First and Second name of the user*\&gt;"

**Adding new pet Form section**

Text "Adding new pet" Text "Name"

1.  Drop-down list Filter named"Type"

2.  Drop-down list Filter named"Sex"

3.  Date-type input field,named

"Birthday"

1.  Text Input field, named "Foodhabits:"

2.  Text Input field, named"About:"

3.  FileUpload Button named "ChooseFile"

4.  Submit button named "Savepet"

**4.1.11 My Pets Section**  **Pets List**\*\* screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

Text "Signed in as \&lt;*First and Second name of the user*\&gt;"

**Below Navigation bar and above Result section:**

Button named "Add a pet"

**Results section**

1.  Text "My pets"

2.  RESULTS LIST showing for eachresult:

-   UP: Name of the pet, Species of the pet



DOWN: Sex, Birthday, Food habits Description if any inputted in About section,
button named

"Delete", button named "Edit"

**4.1.12 My Pets Section**  **Edit pet**\*\* screen\*\*

The screen is the same as "My Pets Section Add a Pet screen" except the
following difference: The title name is: "Edit \&lt;name of the pet\&gt;"
instead of "Adding new pet"

![](media/c214387652872c3cc4e19fe3fcb2493a.jpg)

![](media/1d32189019b6c76092edca4bb90fe58b.jpg)

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 13**

**4.1.13 My Profile section**  **General screen**

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

Text "Signed in as \&lt;*First and Second name of the user*\&gt;"

**Below Navigation bar and above Pets added by the:**

Page title with text "My Profile"

INFO ABOUT THE USER SECTION:

-   Name of theuser







Birthday if entered Rating if received About if entered

1.  Button named "Edit profile" directing to

Edit profile form

1.  A LIST SECTION, with pets added by the usercontaining:

-   Photo of the pet ifadded



Name of the pet

1.  OTHER INFORMATION ABOUT THE USERSECTION:

-   e-mailaddress

-   Phone number ifentered

-   Button named "Change password" directing to Change passwordform

**4.1.14 My profile section**  **Edit Profile**\*\* screen\*\*

**Navigation bar:**

Link to "Info" page

Link to "Requests" page Link to "My profile" page Link to "My pets" page

Link to "Contact us" page Link to "Sign out" option

Text "Signed in as \&lt;*First and Second name of the user*\&gt;" **Below
Navigation bar:**

Page title with text "Edit Profile"

Input field named "e-mail address" – inactive; The user will not be able to
change the e-mail address

1.  Text Input field named"First name"

2.  Text Input field named"Last name"

3.  Text Input field named "Phonenumber"

4.  Date input field named"Birthday"

5.  Text Input field named "Aboutme"

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 14**

1.  Submit Button named "Update profile"

Every user should have a profile page where they can edit their username, e-mail
address, phone number and password, as well as optional additional data, like
does the user want to offer a pet for matchmaking or/and to offer a pet for
adoption, breed of the pet, years of the pet, to add additional information as
text up to 200 symbols, to upload a picture of the pet - see Figure 4. Also, the
user can set the app to his/her preferred language.

Anyways, no matter logged-in/sighed-up or not, the user should be able to see
the two sections of the app – Matchmaking and Adoption, as well as additional
information and to choose by clicking then enter in any of them. When entering a
section, a respective search menu appears - see Figure 3. Here the user should
be able to choose the criteria of the search he/she wants to conduct.

In Figure 5, the list view for the results is shown.

In both sections when a user searches by breed, this view should be the default
one. Each result item includes information about the pet - breed of the pet,
years of the pet, additional information as text, the picture of the pet if any.

A logged-in user should be able to perform the same actions as the non-logged-in
user and additionally to upload announcement for matchmaking or adoption in any
of the two sections (Matchmaking and Adoption).

An administrator should be able to log in to the web-portal where he/she can
administer the system by for instance editing an announcement, or user
information, or banning an announcement if inappropriate.

The section Additional information (see Figure …) should contain headings
hyperlinked to another page, with pictures next to the headings. When clicking a
heading, the user should be transferred to the page with the whole text of the
respective article, to which the heading is hyperlinked (see Figure …).

**4.2 Hardware**\*\* Interfaces\*\*

Since neither the web or mobile apps have any designated hardware, it does not
have any direct hardware interfaces.

**4.3 Software**\*\* Interfaces\*\*

The communication between the database and the web portal and mobile app
consists of operation concerning both reading and modifying the data.

**4.4 Communications**\*\* Interfaces\*\*

The communication between the different parts of the system is important since
they depend on each other. However, in what way the communication is achieved is
not important for the system and is therefore handled by the underlying
operating systems for both the mobile application and the web portal.

**5. Other Nonfunctional**\*\* Requirements\*\*

**5.1 Performance**\*\* Requirements\*\*

**ID: QR1 TITLE** : Prominent search feature

DESC: The search feature should be prominent and easy to find for the user.

**ID: QR2 TITLE:** Usage of the search feature

DESC: The different search options should be evident, simple and easy to
understand.

**ID: QR3 TITLE:** Usage of the result in the list view

**DESC:** The results displayed in the list view should be user friendly and
easy to understand. Selecting an element in the result list should only take one
click.

**Software Requirements Specification for PetMatchMaking Web Application**

**Page 15**

**ID: QR4 TITLE** : Usage of the result in the map view

**DESC** : The results displayed in the map view should be user friendly and
easy to understand. Selecting a pin on the map should only take one click.

**ID: QR5 TITLE** : Usage of the information link **/button**

**DESC** : The information link **/button** should be prominent and it should be
evident that it is a usable link

**/button**. Selecting the information link **/button** should only take one
click.

**ID: QR6 TAG: ResponseTime**

GIST: The fastness of the search SCALE: The response time of a search METER:
Measurements obtained from 1000 searches during testing. MUST: No more than 2
seconds 100% of the time. WISH: No more than 1 second 100% of the time.

**6.**

**Other Requirements**

*\&lt;Define any other requirements not covered elsewhere in the SRS. This might
include database requirements, internationalization requirements, legal
requirements, reuse objectives for the project, and so on. Add any new sections
that are pertinent to the project.\&gt;*

**Appendix A: Glossary**

**Term**

**Definition**

The app

The application specified in the current document

The system

All the components making possible the functioning of the app, incl. front end
and back end

User

Someone who interacts with the app

Non-registered user

Someone who interacts with the app without having a user account

Registered user

Someone who interacts with the app and has a user account

Logged-in user

A Registered user who interacts with the app after he/she has logged-in with
their username/e-mail and password

Non-Logged user

A Registered user who interacts with the app without having logged-in with their
username/e-mail and password

Admin/Administrator

System administrator who is given specific permission for managing and
controlling the system

Stakeholder

Any person who has interaction with the system who is not a developer.

DESC

Description
