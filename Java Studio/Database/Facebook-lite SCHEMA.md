```sql
CREATE TABLE USERS

(email VARCHAR(20) PRIMARY KEY,

full_name VARCHAR(20) ,

screen_name VARCHAR(20),

status VARCHAR(20) ,

DOB DATE,

gender VARCHAR(10),

location VARCHAR(20),

visibility VARCHAR(10)

);

CREATE TABLE POSTS

( email VARCHAR(20),

parentId VARCHAR(20)DEFAULT NULL,

postId VARCHAR(20),

body VARCHAR(100),

timeStamp DATE,

likeCount INTEGER,

PRIMARY KEY (email, parentId, postId)

FOREIGN KEY (email) REFERENCES USERS(email)

FOREIGN KEY (parentId) REFERENCES POSTS(postId)

);

  

CREATE TABLE LIKES

(

postId VARCHAR(10),

email VARCHAR(20),

PRIMARY KEY(postId, email)

FOREIGN KEY (postId) REFERENCES POSTS(postId)

FOREIGN KEY (email) REFERENCES USERS(email)

);

  

CREATE TABLE FRIENDS

(

senderEmail VARCHAR(20),

recieverEmail VARCHAR(20),

startDate DATE,

PRIMARY KEY(senderEmail, recieverEmail)

FOREIGN KEY (senderEmail) REFERENCES USERS(email)

FOREIGN KEY (recieverEmail) REFERENCES USERS(email)

);

  

CREATE TABLE FRIENDREQUESTS

(

senderEmail VARCHAR(20),

recieverEmail VARCHAR(20)

PRIMARY KEY(email1, email2)

FOREIGN KEY (senderEmail) REFERENCES USERS(email)

FOREIGN KEY (recieverEmail) REFERENCES USERS(email)

);
```
