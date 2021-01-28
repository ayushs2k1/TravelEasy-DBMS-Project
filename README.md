# TravelEasy


### Table of Contents

- Abstract
-  1.Introduction
      - 1.1 Overview
      - 1.2 Motivation
      - 1.3 Objective 
      - 1.4 Organization of Project
-  2.Project Resource Requirements       
      - 2.1 Software Requirements 
      - 2.2 Hardware Requirements
-  3.Literature Survey
-  4.Design of the Project 
      - 4.1 ER Diagram 
      - 4.3 ER to Relational Mapping 
      - 4.4 Tables and Constraints
-  5.Normalized Tables
-  6.Output Screenshots
-  7.Conclusion and Future work
-  8.References 

### Abstract

Over the years, the importance of travel has grown. Travel is educational, recreational,
and absolutely essential in today’s era of globalization. Many technologies are being
implemented to make this travel experience smoother and more accessible around the
globe. Travel booking websites enable us to easily compare different travel plans to
provide most cost- effective solution. This project is aimed at implementing a database
management system to facilitate the process of a tourism website in which users can
plan their future holiday or work trips. Users will have the option to "LOG IN" or
"SIGN UP" using their email-id, phone number and password. The user credentials will
also be stored in the database itself. Users can join pre-existing travel packages after
viewing all necessary details such as detailed itinerary and total cost. Users can also
take a short survey in order to get trip recommendations based on their preferences.
Once the destination is finalized, users can make a booking by providing necessary
details such as current city, meal preferences, accommodation preferences, number of
passengers, Aadhar card number etcetera. After filling in all the details in correct
format, user will be re-directed to an online payment portal in order to complete
payment and finalize booking. The database for this project has been implemented
using MySQL, the backend server-side scripting language used is PHP, and HTMLCSS,
JavaScript have been used for front-end development


### 1.Introduction

- 1.1 Overview

Tourism is a very booming industry and has developed as an important part of
the economic foundation of many countries. People see holidays as a necessity,
and not as a luxury in the present scenario. Tourism calls for coordination and
cooperation between various parameters such as accommodation, mode of travel,
budget for travel, number of travelers, etc.

- 1.2 Motivation

The importance of travel and leisure has been highlighted during these difficult
Covid-19 times. The demand for an easy to use, reliable travel booking website
is bound to increase once the situation returns to normalcy and travel restrictions
are lifted.

- 1.3 Objective

This project aims at implementing a system that helps users to plan and
coordinate their trips in an easy-to-use and reliable manner.

- 1.4 Organization of the project

We will be using MySQL to create the tables and designing a website as our
final presentation in which a user can create travel plans, join pre decided travel
plans and also submit reviews for destinations they have visited along with
filling a survey using which the website will recommend travel destinations to
the user.

### 2.Project Resource Requirements

- 2.1 Software Requirements
      - HTML5
      - CSS3
      - Javascript
      - PHP
      - MySQL
      - Visual Studio Code

- 2.2 Hardware Requirements
      - Hard Disk(2 GB)
      - RAM(1 GB)
      - Processor(Dual Core or Above)
 
 ### 3.Literature Survey

![](Output_images/dbms(1).png)
![](Output_images/dbms(2).png)
![](Output_images/dbms(3).png)

### 4.Design of the Project

- 4.1 ER Diagram

![](Output_images/dbms(4).png)

- 4.2 ER to Relational Mapping (Schema Diagram)

![](Output_images/dbms(5).png)

- 4.3 Tables and Constraints

![](Output_images/dbms(6).png)


### 5.Normalized Tables

a)Admin

![](Output_images/dbms(7).png)


b)Trip

![](Output_images/dbms(8).png)


Functional Dependencies:

i)Total_Price -> StartDate, EndDate: The total cost of the trip is directly dependant on
the starting date and ending date of the trip

ii) GuideName, GuideContact -> TripId, Itinerary: Since the overall packages of the trips
will be set by the admin, hence the guides will also be the chosen by the admins and
also the kind of guide depends upon the itinerary chosen by the user hence these two
attributes are directly dependent on the TripID and Itinerary.

After Normalization:

![](Output_images/dbms(9).png)

c)Hotels

![](Output_images/dbms(10).png)

d)Cities

![](Output_images/dbms(11).png)

e)Distance

![](Output_images/dbms(12).png)

f)Trip_Group

![](Output_images/dbms(13).png)

g)Recommendation

![](Output_images/dbms(14).png)

Functional Dependencies:

i)Location -> Category: Locations are directly dependent on the category of the
location like a beach location, a historical location, a hill station etc.

After Normalization:

![](Output_images/dbms(15).png)

h)Age_Group

![](Output_images/dbms(16).png)

i)Recom_Locs

![](Output_images/dbms(17).png)

j)User

![](Output_images/dbms(18).png)

Functional Dependencies:

i)Review -> Rate: The review given by the user is directly dependent on the rating
given by the user, as if the user gives a good rating to the trip/plan/location, the
review for the same is also going to be good

ii)Mobile -> City: City Codes are common to phone numbers issued in the same city, be
it landlines or mobile numbers, hence mobile number is directly dependent on the city
of the User.

After Normalization:

![](Output_images/dbms(19).png)

k)Get_Recommendation

![](Output_images/dbms(20).png)

l)Join_Trip

![](Output_images/dbms(21).png)

m)Trip_Location

![](Output_images/dbms(22).png)

n)User_Pref

![](Output_images/dbms(23).png)

### 6.Output Screenshots

![](Output_images/dbms(24).png)

![](Output_images/dbms(25).png)

![](Output_images/dbms(26).png)

![](Output_images/dbms(27).png)

![](Output_images/dbms(28).png)

![](Output_images/dbms(29).png)

![](Output_images/dbms(30).png)

![](Output_images/dbms(31).png)

### 7.Conclusion

- 7.1 Conclusion

We were able to implement a fully functional web application for tours and travel planning
during the course of this project. Due to this project, we were also able to explore the
practical purposes of a database management system and put our Web Development skills to
the test using HTML-CSS, JavaScript, and PHP. The project overall was a great learning
experience for the entire team and has helped us understand the various components of a
DBMS to a much greater depth.

- 7.2 Future Work

Future improvements involve using an actual payment API instead of a dummy test
API to give it a better feel, and add more travel destinations. Adding more
functionality on booking page like custom facilities like choosing travel mode.
Adding booking services of buses and cabs and hot air balloons. Adding Visa
extension services. Adding more cities and hotels to choose from.

### 8.References

[1] Kirti Singh Dahiya, Dr. K. K. Batra “Travel industry selecting between online and
offline Mode”, International Journal of Scientific and Research Publications, Volume 6, Issue
9, September 2016, 694 ISSN2250-3153

[2] Faudziah Ahmad, Fauziah Baharom and Moath Husni “Current Web Application
Development and Measurement Practices for Small Software Firms (May 2012): Acceptance
Degree Identification”

[3] Narayan B. Prabhu M, “An exploratory study on online travel trends and travel behaviour
of employees working in I.T. organizations in Bengaluru, India”, Global Review of Research
in Tourism, Hospitality and Leisure Management (GRRTHLM) An Online International
Research Journal (ISSN: 2311-3189) 2014 Vol: 1 Issue 3

[4] Soloman Anthony, “A review and analysis of technologies for developing web
application.(March 2012):ASP.NET”,A_review_and_analysis_of_technologies_for_developi
ng_web_Applications

[5] Anton Bogdanovych, Helmut Berger, Simeon Simoff and Carles Sierra, “Travel Agents
vs. Online Booking: Tackling the Shortcomings of Nowadays Online Tourism Portals”,
Conference: Information and Communication Technologies in Tourism, ENTER 2006,

[6] Punam Kumari and Rainu Nandal, “A Research Paper On Website Development
Optimization Using Xampp/PHP(May-June 2017)”, 3792-8121-1-PB.pdf

[7] Faudziah Ahmad, Fauziah Baharom and Moath Husni, “Current Web Application
Development and Measurement Practices for Small Software Firms (May 2012): Variable
Clustering”

[8] Faudziah Ahmad, Fauziah Baharom and Moath Husni, “Current Web Application
Development and Measurement Practices for Small Software Firms (May 2012): Variable
Clustering: Data Coding”

[9] Soloman Anthony, “A review and analysis of technologies for developing web
application.(March 2012):LAMP”,A_review_and_analysis_of_technologies_for_developing_
web_Applications

[10] Soloman Anthony, “A review and analysis of technologies for developing web
application.(March 2012):J2EE”,A_review_and_analysis_of_technologies_for_developing_
web_Applications

### Our Team

Keerthana Balamurugan, Harshit Vijay, Anant Tiwari and Ayush Sharma
