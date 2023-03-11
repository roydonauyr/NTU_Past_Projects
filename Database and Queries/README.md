# 1. BC2402 SQL-and-NoSQL-Queries
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/SQL-and-NoSQL-Queries)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/SQL-and-NoSQL-Queries)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/SQL-and-NoSQL-Queries)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/SQL-and-NoSQL-Queries)

In this project, we were tasked with running SQL and NO-SQL Queries on Covid19 data to study how covid19 has affected different countries and the integrity of data.

Some ERD diagrams:
![image](https://user-images.githubusercontent.com/44868878/178111961-401d9b3b-d9a7-4ce3-8dc7-3e3d1859212b.png)
![image](https://user-images.githubusercontent.com/44868878/178111966-f49c609a-cc0b-4244-a020-4e751aa34d08.png)

We also explored the difference between storing data in sql vs no-sql databases. (Pros and cons)

Lastly, we made a few recommendations to WHO on considerations when storing data:

One major health-related aspect WHO is interested in is COVID-19 data. Generally, health-related data, such as COVID-19 data, are often largely unstructured, constantly being updated and revised in real-time in large amounts and spatial in nature. Keeping in mind these characteristics of health-related data like COVID-19, we further examine the differences in relational and non-relational databases to decide on a more suitable option for WHO.

In the context of COVID-19, the flexible nature of non-relational databases will prove to be valuable. The process of inserting and updating data is especially efficient provided that it does not follow a predefined structure as mentioned. COVID-19 data will be obtained across many different countries, but not all countries will have the same amount of information. In other words, certain countries may not have information for certain attributes. Data received will be largely inconsistent, with no fixed structure to it. The flexibility of a non-relational database allows for ease of updating and insertion of data. Time is saved as existing data received does not need to be constantly refined before it can be inserted into the database. This way, WHO can continue being a reliable source of information as they are able to keep up with the fast pace of information being received. 

Besides that, if such sparse data were to be inserted into a relational database, this would result in the creation of unnecessary cells that have missing or null values. This is because in a relational database, every attribute is required to be filled in due to its predefined structure, as mentioned above. This could lead to inefficient implementation of databases. Furthermore, this could mislead users into assuming these missing values are information that are available but have yet to be updated. Users might inaccurately account for these missing or null values and expect results higher than expected. In reality, those missing or null values for that particular country are unavailable and no such attribute exists at all. One example of such a misleading situation happening can be seen from Question 8 of the SQL queries. There was an inconsistency in terms of the dates recorded for Germany, where the ‘covid19data’ table has earlier records of dates than the ‘country_vaccinations_by_manufacturer’ table. However, majority of the attributes’ information related to the ‘covid19data’ table is missing or null. This could lead to users misinterpreting those dates to still be important. Users assume that these attributes exist and information regarding those attributes are available. Consequently, this led to us inaccurately accounting for these dates in our final query, with the assumption that the attribute data is available but has yet to be updated.

Our team would also like to advise WHO to make use of non-relational databases when recording COVID-19-related data to avoid misleading users, or possibly conveying inaccurate information.
Given that WHO is a well-established organisation known for providing a large range of global data, their database is constantly expanding. Moreover, as the pandemic has yet to stabilise, COVID-19 related datasets are likely to continue growing over the years. Thus, it would be financially beneficial for them to leverage on non-relational databases, that is capable of handling large volumes of data while still ensuring optimal performance.
One main health-related aspect WHO is focusing on in recent times, is COVID-19 data. The geospatial feature of non-relational databases will be especially relevant in this aspect for WHO. COVID-19 related data is inherently spatial in nature. 

To minimise the spread of this disease globally, it is critical to identify the exact location of individuals tested positive for COVID-19 and to track their movements. By relying on non-relational databases, WHO can offer additional valuable geospatial insights during this pandemic. Tracking geospatial data will be helpful in assisting countries to respond quickly in the midst of this pandemic. However, one critical aspect WHO should be aware of when leveraging on non-relational databases is its importing method and the resulting differences. A non-relational database with the use of MongoDB Compass and noSQL booster platform, gives WHO 2 different importing options. Each option will result in a different dataset.
Based on the aforementioned reasons, it is clear that the effectiveness of relational and non-relational databases will vary depending on the circumstances. In the case of WHO, non-relational databases will be a more suitable option for them. This is mainly due to their need to update their database of information quickly and with large amounts at any one time. Ultimately, in the context of COVID-19 related data, the use of non-relational databases is also highly recommended. This is due to its additional ability to handle and track geospatial data. Overall, our team would recommend the use of non-relational databases to WHO, provided they are focused on recording data related to the recent global pandemic – COVID-19.


# CZ4031-Advanced-Database

## Project 1:
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/CZ4031-Advanced-Database-Project)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/CZ4031-Advanced-Database-Project)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/CZ4031-Advanced-Database-Project)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/CZ4031-Advanced-Database-Project)

The aim of this project is to implement a B+ Tree in C++ which supports searching (both search
query and range queries), insertion and deletion operations.

Our implementation consists of the following classes:
1. BlockManager: Manages the creation and deletion of new blocks. Handles all the logic
related to blocks.
2. Record class: Holds the fields of a record.
3. B+ Tree: Handles the logic of search, insertion and deletion operations of nodes in the
tree.
4. Block classes: Consists of B+ tree nodes, recordBlocks and linkedList Blocks

More information can be found in our pdf report.

B+ Tree Structure:
![image](https://user-images.githubusercontent.com/44868878/224474247-565e913a-e8de-4225-8680-eea90997ac26.png)

### Functions:
We have 4 vital functions to help us perform the experiments, namely Insert(), Delete(), searchKeys(),
searchRangeOfKeys(). 
Details can be found in the pdf report

### Requirements and how to fun
To install, run a C++ compiler with minimum C++11 support to compile main.cpp, then run the produced binary. Assuming g++, run the following command: g++ main.cpp -O2 -o main

To run: .\main.exe

In the case that some middle output disappears in the terminal (Happened sometimes in vsc terminal, could be due to too many information to print out), do output it out into a text file. That way the full output always comes out correctly. (Use .\main.exe > someTxtFile.txt)


## Project 2:
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/CZ4031-Advanced-Database-Project-2)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/CZ4031-Advanced-Database-Project-2)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/CZ4031-Advanced-Database-Project-2)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/CZ4031-Advanced-Database-Project-2)

### Project description:

**Introduction**

In this project, we are tasked with the goal to translate and annotate a given SQL Query by
obtaining their Optimal QEP and respective AQPs. Using these AQPs, we are able to explain how
different components of the query are executed by the underlying query processor and why the
operators are chosen among other alternatives.

**File structure**

Our project is split into four main python files:
1) Project.py

This is the main file that our application uses that invokes all the necessary procedures
from the other three files.

2) Interface.py

This file is incharge of the display of the optimal query plan together with annotations on
the plan. This file also contains the logic for how the user interacts with the program. (e.g.
Handling errors from user inputs)

3) Preprocessing.py

The main responsibilities of these file are:

● To establish connection with the database tables

● Obtain Optimal QEP

● Obtain AQPs

● Make preparations before passing over to annotations to annotate the Optimal QEP.


4) Annotation.py

This file is in charge of annotating respective tree nodes in the optimal QEP.

**Libraries Used:**
The libraries that are required to run this project are:

● Psycopg2, which is a library that is used as a PostgreSQL database adapter for Python.

● Tkinter, which is a built-in python library that is made for building simple GUI for
application in python

### Running Instructions
a. Ensure python version is 3.8 (For 3.10 version and above psycopg2 wont run and an error
will show: ModuleNotFoundError: No module named 'psycopg2')
b. Pip install psycopg2 (If that doesn’t work, use pip install psycopg2-binary)
c. Change to the correct directory and Run the project.py file

