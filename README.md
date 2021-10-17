# Database-Systems-for-Online-shoppers-and-Ecommerce-website
Postgres such as Relational database management system is leveraged to store and manage large datasets with fixed attributes such as personal details of registered customers on an Online shopping  application.

## Introduction
A crucial component in the design of software development projects is the choice of database model most suitable for data storage and database management operations whether for an Online shopping application, E-commerce website or an Online gaming application. This project evaluates three database management systems including models of different NoSQL genres each accompanied with appropriate use cases. From PostgreSQL designed to handle related data structures into its predefined schema and ACID compliancy to MongoDB developed to store and manage document data types that obey BASE theory to Redis implemented to operate set of strings arranged in key-value pairs suited to manage highly scalable Big Data and store frequently retrieved data, no database system can offer all three CAP properties simultaneously. Also, the most appropriate method of selecting a database system for a system development project is to carry out entity-relationship modelling which can inform choice of data model by identifying the attributes of the datasets and their familiarities.

## PostGreSQL for customer details of an online shopping application
Customer details such as Customer’s identification number, Name, Email, Mobile number, Contact-address and Gender are related attributes built into PostgreSQL have a uniform 
structure with predictable tuple of fixed customer’s information that requires flexible query activities as such meets the database requirements. They also obey domain rules regardless of their data types whether integers, strings, binary, boolean or variable characters. With this, Postgres aid easy guidance for database managers and other service users in submitting their information while registering on the application. 

-  After installing PostgreSQL on a computer system, the first step is to create related tables for the database which requires administrative privilege for this. This requires
naming the table title, defining the variable types, setting value limit for each column, identifying the primary key and set a constraint with the Check domain function for Gender for options between Male, Female and Prefer Not to say.

![image](https://user-images.githubusercontent.com/76513466/137634619-3d388d28-b6a6-425b-adc7-95785d969f95.png)

![image](https://user-images.githubusercontent.com/76513466/137634633-120e2351-c9b5-43cb-97f7-4096bcbcd23e.png)

- It is necessary to insert values into the multidimensional table of tuples (rows) and attributes (columns) for easy manipulation in the main table named Customer_details. By inserting data values of defined columns into the Address table.

![image](https://user-images.githubusercontent.com/76513466/137634651-bd920cf5-39c5-427a-a69c-9a1827dea184.png)

![image](https://user-images.githubusercontent.com/76513466/137634664-7d9f631c-d767-45f4-b025-76a9cc294e6c.png)

- In order to retrieve both tables of related data, the following syntaxes are used:

![image](https://user-images.githubusercontent.com/76513466/137634685-71e67692-0a45-495d-8195-7f8b1bcd0c57.png)

- To update a customer’s last name from the customer_details table, we use the code below. Note that Postgres is not case sensitive therefore case letters are not a point of observation.

![image](https://user-images.githubusercontent.com/76513466/137634760-305964d2-7514-4367-952c-2da83ca38ec1.png)

![image](https://user-images.githubusercontent.com/76513466/137634774-3ddaca4c-b742-49e1-a476-e764f4ea5ab0.png)

-  To delete a tuple/row from the contact address table with regards to CRUD operations.

![image](https://user-images.githubusercontent.com/76513466/137634836-f0f18754-dcd3-433d-b0b3-abc6de5b31ce.png)

- Table join is one of the advantages of handling large datasets for correlation and comparison purposes. A join is an SQL command function used to combine rows of more than one related tables. Between the Customer_details and Address tables, customer_id is the common column which will be used to demonstrate an Inner/Center join.

![image](https://user-images.githubusercontent.com/76513466/137634861-18b2878c-ebdc-48df-bc02-60beca7f3b9e.png)

![image](https://user-images.githubusercontent.com/76513466/137634866-7bc6c643-c262-48c9-9cd5-c1fc582b9eb2.png)

Other types of joins include Left/outer join, Right join and Full join.

- To query a database, Index statements are invoked to create an index in the table used to retrieve data from the database system to fasten the search process. There are also scans that iterate over records.

![image](https://user-images.githubusercontent.com/76513466/137634894-7ecdba32-09ea-4f2d-b215-1bf17a93a36b.png)

-  The SQL Group clause is used to aggregate functions by more than one column. For example, the following statement returns the number of addresses using the group by, count and left join clauses. This also demonstrate an example of nested database.

![image](https://user-images.githubusercontent.com/76513466/137634918-dc62b968-604d-43d4-81cc-9788239bfffc.png)

## MongoDB for E-commerce website
MongoDB is one of the prominent non-tabular NoSQL database system designed to store and manage Big Data stored in document format as JSON objects in form of trees with high 
query performance and scalability. MongoDB is equipped to store and modify the product catalogue for an E-commerce website with different properties.
Product catalogue grouped into collections of documents of heterogenous data consisting of Fresh food, Bakery, Frozen food, Cereals, Diary, household cleaning and Skincare with 
various properties is suitable for MongoDB to manage as it stores documents as JSON object with less schema and high query flexibility by assigning object identification to each 
document as master slave arrangement. With its query, schema less and indexing features, MongoDb can support product filtering and search engine. Field-values in form of Boolean, Date, object_id, String, and Integer as well as atomic operations within a single document is supported by MongoDB as document formats for data storage and management operations in Javascript.

- Initialisation: After initialising a command-line user interface and scripting language, in this case Powershell 7, Mongo is entered to connect to the MongoDB and the 
databases present is retrieved. Then, a new database system is created and switched to as Products and retrieve Products.

![image](https://user-images.githubusercontent.com/76513466/137635428-7e9ed04f-b8bf-4ef6-aa7f-335546959675.png)

- Create User: A stakeholder such as a user with an administrative role where username is Ibrahim and Password is 1234.

![image](https://user-images.githubusercontent.com/76513466/137635445-11c8249b-5b48-4f43-ba2d-f79ff392c693.png)

-  Collection: A collection of documents can be created to group unstructured data together as shown below:

![image](https://user-images.githubusercontent.com/76513466/137635467-6364b18e-83fb-4e1c-891c-a561f8e30a82.png)

- To insert data into the selected database, Product.

![image](https://user-images.githubusercontent.com/76513466/137635496-f56e272f-2f98-4e8a-8a8b-6024ea41831c.png)

- Query: In order to enquire about the whole products in the collection/catalogue, the following is carried out. Also, the find() command function does not arrange the documents by default except with the pretty() clause.

![image](https://user-images.githubusercontent.com/76513466/137635528-d60a5c9e-680d-4c64-bae7-ba1b011f40f8.png)

![image](https://user-images.githubusercontent.com/76513466/137635545-67a3ab02-4770-4f83-a1cb-13b3bc236521.png)

### Database management Privacy Protection
- By legislation, all stakeholders must uphold national laws stipulated such as the General Data Protection Regulation (GDPR, 2018), Data Protection Act (2018), and Computer Misuse Act (1990) to prevent unlawful disclosure and identity theft.
- IT stakeholders and all regulating bodies must ensure proper oversight and accountability to ensure duties are conducted ethically.
- Open-source data is also protected by the GDPR on the basis of privacy by design and not at the end of build.
- Ethically, it is also obligatory for IT professionals to avoid or report any conflict of interest that may arise with relevant authority in the act of carrying out their responsibilities.

