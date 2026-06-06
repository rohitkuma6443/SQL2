
<h1>MySQL SELECT and UPDATE Query Notes</h1>

<h3>Topics Covered</h3>

<ul>
    <li>Create Database</li>
    <li>Create Table</li>
    <li>Insert Data</li>
    <li>SELECT Query</li>
    <li>WHERE Clause</li>
    <li>UPDATE Query</li>
    <li>Best Practices</li>
</ul>

<hr>

<h2>1. Create Database</h2>

<pre>
create database School;
</pre>

<h3>Explanation</h3>

<ul>
    <li>CREATE DATABASE is used to create a new database.</li>
    <li>School is the name of the database.</li>
</ul>

<hr>

<h2>2. Select Database</h2>

<pre>
use School;
</pre>

<ul>
    <li>USE command selects the database for working.</li>
</ul>

<hr>

<h2>3. Create Student Table</h2>

<pre>
create table Student(

    ID int primary key,
    Name varchar(100),
    Course varchar(50),
    City varchar(50),
    Contact varchar(20)

);
</pre>

<h3>Explanation of Columns</h3>

<table border="1">

<tr>
    <th>Column</th>
    <th>Meaning</th>
</tr>

<tr>
    <td>ID</td>
    <td>Unique Student ID</td>
</tr>

<tr>
    <td>Name</td>
    <td>Student Name</td>
</tr>

<tr>
    <td>Course</td>
    <td>Student Course Name</td>
</tr>

<tr>
    <td>City</td>
    <td>Student City</td>
</tr>

<tr>
    <td>Contact</td>
    <td>Student Contact Number</td>
</tr>

</table>

<hr>

<h2>4. Insert Data into Student Table</h2>

<pre>
insert into Student values

(101,"Rahul","Python","Mumbai","9876543210"),
(102,"Kajal","Java","Delhi","9123456780"),
(103,"Raju","MySQL","Pune","9988776655"),
(104,"Aman","Excel","Mumbai","9012345678");
</pre>

<h3>Explanation</h3>

<ul>
    <li>INSERT INTO is used to add records into a table.</li>
    <li>Multiple rows can be inserted in one query.</li>
</ul>

<hr>

<h2>5. SELECT Query</h2>

<p>
SELECT query is used to read or retrieve data from a MySQL database table.
</p>

<hr>

<h2>6. Read All Data from Table</h2>

<pre>
select * from Student;
</pre>

<ul>
    <li>SELECT means retrieve data.</li>
    <li>* means all columns.</li>
    <li>Student is the table name.</li>
</ul>

<hr>

<h2>7. Read Specific Columns</h2>

<pre>
select Name, Course from Student;
</pre>

<ul>
    <li>This query displays only selected columns.</li>
    <li>Useful when large datasets are available.</li>
</ul>

<hr>

<h2>8. SELECT Query with WHERE Clause</h2>

<pre>
select * from Student
where ID = 103;
</pre>

<ul>
    <li>WHERE clause filters records.</li>
    <li>Only the student with ID 103 will be displayed.</li>
</ul>

<hr>

<h2>9. UPDATE Query</h2>

<p>
UPDATE query is used to modify existing data inside a table.
</p>

<hr>

<h2>10. Update Student Contact Number</h2>

<pre>
update Student
set Contact = "9999999999"
where ID = 103;
</pre>

<h3>Explanation</h3>

<table border="1">

<tr>
    <th>Part</th>
    <th>Meaning</th>
</tr>

<tr>
    <td>UPDATE Student</td>
    <td>Selects Student table for updating</td>
</tr>

<tr>
    <td>SET</td>
    <td>Specifies new value</td>
</tr>

<tr>
    <td>WHERE</td>
    <td>Specifies which record to update</td>
</tr>

</table>

<hr>

<h2>11. Verify Updated Data</h2>

<pre>
select * from Student
where ID = 103;
</pre>

<hr>

<h2>12. Important Note About UPDATE</h2>

<h3>Wrong Method</h3>

<pre>
update Student
set Contact = "8888888888"
where Name = "Raju";
</pre>

<h3>Problem</h3>

<ul>
    <li>Multiple students can have the same name.</li>
    <li>This may update multiple records accidentally.</li>
</ul>

<hr>

<h2>13. Best Practice</h2>

<pre>
update Student
set Contact = "8888888888"
where ID = 103;
</pre>

<ul>
    <li>Always use unique identifiers like ID.</li>
    <li>This prevents accidental updates.</li>
</ul>

<hr>

<h2>14. Difference Between SELECT and UPDATE</h2>

<table border="1">

<tr>
    <th>SELECT</th>
    <th>UPDATE</th>
</tr>

<tr>
    <td>Reads data</td>
    <td>Modifies data</td>
</tr>

<tr>
    <td>Does not change records</td>
    <td>Changes existing records</td>
</tr>

<tr>
    <td>Used for viewing data</td>
    <td>Used for editing data</td>
</tr>

</table>

<hr>

<h2>15. Most Important Commands</h2>

<table border="1">

<tr>
    <th>Command</th>
    <th>Purpose</th>
</tr>

<tr>
    <td>CREATE DATABASE</td>
    <td>Create database</td>
</tr>

<tr>
    <td>USE</td>
    <td>Select database</td>
</tr>

<tr>
    <td>CREATE TABLE</td>
    <td>Create table</td>
</tr>

<tr>
    <td>INSERT INTO</td>
    <td>Insert records</td>
</tr>

<tr>
    <td>SELECT</td>
    <td>Read data</td>
</tr>

<tr>
    <td>WHERE</td>
    <td>Filter records</td>
</tr>

<tr>
    <td>UPDATE</td>
    <td>Modify data</td>
</tr>

</table>

<hr>

```html
<hr>

<h2>16. DELETE Query</h2>

<p>
DELETE query is used to remove records from a table.
</p>

<hr>

<h2>17. Delete Specific Record Using WHERE Clause</h2>

<pre>
delete from Student
where ID = 104;
</pre>

<h3>Explanation</h3>

<ul>
    <li>DELETE removes data from a table.</li>
    <li>WHERE clause specifies which record should be deleted.</li>
    <li>Only the student with ID 104 will be deleted.</li>
</ul>

<hr>

<h2>18. Delete All Records from Table</h2>

<pre>
delete from Student;
</pre>

<h3>Explanation</h3>

<ul>
    <li>Deletes all records from the table.</li>
    <li>Table structure remains safe.</li>
    <li>Columns and table design are not removed.</li>
</ul>

<hr>

<h2>19. Drop Entire Table</h2>

<pre>
drop table Student;
</pre>

<h3>Explanation</h3>

<ul>
    <li>DROP TABLE completely removes the table.</li>
    <li>Both data and table structure are deleted permanently.</li>
</ul>

<hr>

<h2>20. Difference Between DELETE and DROP</h2>

<table border="1">

<tr>
    <th>DELETE</th>
    <th>DROP</th>
</tr>

<tr>
    <td>Deletes records only</td>
    <td>Deletes complete table</td>
</tr>

<tr>
    <td>Table structure remains</td>
    <td>Table structure is removed</td>
</tr>

<tr>
    <td>Can use WHERE clause</td>
    <td>Cannot use WHERE clause</td>
</tr>

</table>

<h2>Conclusion</h2>

<ul>
    <li>Create database and table</li>
    <li>Insert records into MySQL table</li>
    <li>Read data using SELECT query</li>
    <li>Filter records using WHERE clause</li>
    <li>Modify records using UPDATE query</li>
    <li>Use unique IDs for safe updates</li>
</ul>
