# Database Systems

![c](https://user-images.githubusercontent.com/116082827/235316862-e40038da-f391-48e6-9032-e9da811d7079.jpeg)


Database systems are software systems that store and manage large amounts of structured and unstructured data. Understanding database systems is essential for developing software that interacts with databases. Here's an example of a simple database program in Python using the 

SQLite library:



import sqlite3



# Create a connection to the database

conn = sqlite3.connect('example.db')



# Create a table

conn.execute('''CREATE TABLE IF NOT EXISTS users

                 (id INTEGER PRIMARY KEY, name TEXT, age INTEGER)''')



# Insert data into the table

conn.execute("INSERT INTO users (name, age) VALUES ('Alice', 25)")

conn.execute("INSERT INTO users (name, age) VALUES ('Bob', 30)")



# Query the table

result = conn.execute("SELECT * FROM users")

for row in result:

    print(row)



# Close the connection

conn.close()
