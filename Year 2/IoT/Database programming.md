Created: Mar 23 2026
Class: [[IoT]] 
- - -
# MySQL
```
pip install mysql-connector-python
```

## Create DB
```python
mydb = mysql.connector.connect(
	host="localhost",
	user="yourusername",
	password="yourpassword"
)

mycursor = mydb.cursor()  
  
mycursor.execute("CREATE DATABASE mydatabase")
```

## Connect to DB
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

# SQLite3
```
pip install sqlite3
```

## Connect to DB
```python
sql = sqlite3.connect('database_name.db')
cursor = sql.cursor()
cursor.execute("SELECT * FROM TABLE_1")
	```x