	Mar 28 2025
Class: [[Database]]
- - -
How many records are there in each of the tables in the world database?

- City: 4079
- Country: 239
- CountryLanguage: 984
- - -
Based on this description, predict what will happen when each of the create table statements is executed:

- How many tables (relations) will be created?
	- 4
- How many attributes will each table have?
	- Customers: 7
	- Order details: 4
	- Orders: 3
	- Products: 7
- What are the types of the attributes?
	- INTEGER
	- VARCHAR
	- CHAR
- - -
1. Were you able to enter this third record?
		Yes
2. Should you have been able to enter this third record?
	  No
    - _Hint:_ Take a look at the data. Is there any duplicated data?
3. What type of integrity constraint does this record violate?
	Entity integrity
- - -
1. Were you able to enter this record?
		Yes
2. Are any constraints violated by this action? Explain why/why not.
		Yes - Entity integrity 
- - -
1. What do these record represent in terms of the overall database management system? That is, the DBSM is representing things in the "real-world". What do these records correspond to in the "real world"?
	- CUSTOMERS: customer info
	- ORDER_DETAILS: the info of each order
	- ORDERS: Links to order info
	- PRODUCTS: 
2. Were you able to enter these new records?
		Yeah
3. Are any constraints violated by these records? Explain why/why not.
		Yes - Relational integrity
- - -
- Could you execute the statement, that is, did the insert work?
	- 1 - pass
	- 2 - fail, duplicate entry
	- 3 - fail, primary key is NULL
	- 4 - fail, invalid foreign key
- If the insert did not work, what integrity constraint(s) were violated?
	- Relational
	- Entity
	- Uniqueness
- - -
For **each** of the below database operations (note these are _descriptions_ of database operations, and not SQL statements.):

1. Identify whether any integrity constraints of the above relational database schema are violated by each operation, or not
2. For every violation, explain why the violation occurred, and actions you can take to make sure that the operation avoids violating any integrity constraints.

1.1 Uniqueness 
1.2 Duplicate SSN 

2.1 Uniqueness 
2.2 Duplicate Pnumber

3.1 Entity
3.2 Primary key is null

4.1 Relational
4.2 Foreign key (Essn) doesn't exist in home relation (Employee)

5.1 No error

6.1 No error

7.1 Uniqueness
7.2 SSN 666884444 already exists


