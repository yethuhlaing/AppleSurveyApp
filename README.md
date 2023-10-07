## Introduction

This Assignment project was made for the Level4 Diploma in Computing (UK). The program focuses 
focus on undertaking surveys of its branded Apple smartwatches and evaluating
the responses. The program will allow two characters (Administrators & Customers). Therefore,
program will be designed for each role. Users are allowed to create secure accounts, login and
perform their respective tasks. For the administrators, efficient pages will be built for creating
surveys and analyzing the responses. As regards the customers, attention-grabbing pages will
be definitely developed for answering the surveys and reviewing them. 


## Assumption
An integrated development environment (IDE) is required for coding so Microsoft Visual
Studio has to be installed. Furthermore, Microsoft SQL server is installed to create databases
and tables for storing input data. C# language is used throughout the program. Images
concerning the company product are applied for background images. User Interfaces of
program are taken screenshot for black box testing. As regards white box testing, some pieces
of coding have to be taken screenshots. Whenever data have been inputted into database,
successful results have to be recorded and incorporated into test results.

## Class Diagram
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/bbbcf096-3f7a-4149-acc2-daf5eecb8993)

## Justification of Class Diagram

Class diagrams act as building blocks in object-oriented modeling describing a variety of objects in a system. In this program, four class diagrams are constructed to model the static perspective of a program. The top portion of each diagram contains the class name. The middle part includes encapsulated attributes by making the variables as private and exposing the property for the entrance of private data which would be public. The bottom partition is composed of operations for class to execute the program.

The Admin class is designed with private operations and attributes providing data hiding and security. The operations are to insert administrators’ information into database when they are invoked. On top of that, “Login Admin” operation is created to check the input and allow admins only if the input data match with ones in database. As one admin can create many surveys and one survey should have only one admin, the Admin class links to the Survey class by means of one-to-many relationship.

The Survey class is built for storing the input concerning surveys with encapsulated attributes. In this class, the operations are developed for updating and deleting surveys as well as refreshing the page. “Save Survey” operation, main features of program, is to transfer the surveys to the database. Moreover, the specific operation “Show Survey Questions” is to exhibit only survey questions. As one survey can have many responses but one response must have only one survey, the “Survey” class links to the “Customer Response” class by means of one-to- many relationship.

The Customer Response class is constructed for collecting the answers and adding them to database. There is one operation for each choice of survey question. For the rating question, the average value will be calculated for each survey by the “Count Response”. The “Search Survey” operation is to explore surveys easily. The attributes are string data type with the exception of “Q6Answer”. This is because the “Count Response” operation gets only integer data type to determine the average. As one customer can answer many responses but one response must be answered by only one customer, the “Survey” class links to the “Customer Response” class by means of one-many relationship.

The customer class is much similar to the admin class. In this class, the “Save Customer” operation is designed for adding clients’ information into database instead of admin’s when they are invoked. “Login Customer” operation examines whether the customer input data match with ones in database. And then, allow login process only when the correct data are inputted.

## User Manual


![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/7a6b54d1-1ab9-4a6c-a0d8-75965b127529)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/e91a5da3-6ad2-4564-82b6-636189d76706)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/18a6804f-3b6b-48d8-adfe-402598d2564b)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/e77ac59b-a395-427f-90a0-4a43f38a1d65)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/f7a202ae-0c9f-4c3d-85df-a2aa5e77c200)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/93937855-d116-42d5-a91a-159149c68b81)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/5bb1a90e-e0e7-4a47-8a68-3de0313a994e)

## Test Scripts
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/2fd06c04-11d6-4381-acec-228c3d04f6d5)
![image](https://github.com/yethuhlaing/Apple-Survey-Destop-Application/assets/112906488/b0094dd4-274a-4199-89c7-6634495d6529)
