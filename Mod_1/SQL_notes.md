# SQL

## Questions

Is doing an SQL comand for filtering faster than doing a pandas command for an already loaded dataset?

## Lecture

### non-SQL databases

<ul>
<li>neo4J
<li>graphQL
</ul>

sqlite3 connect has default arguments:

sqlite3.connect(host=host, user=user, passwd=passwd, db=db)

conn.cursor() is like a mouse cursor, it's how you interact with the DB
whatever DB you have the cursor set on is what db you will be esecuting on.

### triggers

<ul>
<li>CREATE</li>
used to create tables

make querey like:
query = """CREATE TABLE students (
first_name text,
birth_date text,
num_siblings integer
)"""

c.execute(query)
