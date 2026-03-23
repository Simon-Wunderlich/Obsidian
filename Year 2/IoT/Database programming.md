Created: Mar 23 2026
Class: [[IoT]] 
- - -
```
pip install mysql-connector-python
```

# Create DB
```python
mydb = mysql.connector.connect(
	host="localhost",
	user="yourusername",
	password="yourpassword"
)

mycursor = mydb.cursor()  
  
mycursor.execute("CREATE DATABASE mydatabase")
```

# Connect to DB
```python
mydb = mysql.connector.connect(
	host="localhost",
	user="yourusername",
	password="yourpassword",
	database="database
)

mycursor = mydb.cursor()  
  
mycursor.execute("SELECT * from TABLE_1")
```