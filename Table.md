<h1>SQL Notes – School Database</h1>
<h3>Topics Covered</h3>
<ul>
        <li>Create Database</li>
        <li>Use Database</li>
        <li>Create Table</li>
        <li>Insert Data</li>
        <li>View Data</li>
        <li>Delete Data</li>
        <li>Remove Table</li>
</ul>

<hr>

<h2>1. Create Database</h2>

    <pre>
create database School;
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li><b>CREATE DATABASE</b> is used to create a new database.</li>
        <li>Here, the database name is <b>School</b>.</li>
    </ul>

    <p>
        A database is like a container that stores tables, records, and information.
    </p>

    <hr>

    <h2>2. Select Database</h2>

    <pre>
use school;
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li><b>USE</b> command selects the database to work on.</li>
        <li>All tables will be created inside the selected database.</li>
    </ul>

    <hr>

    <h2>3. Create Student Table</h2>

    <pre>
create table Student(
    Id int primary key,
    Name varchar(100) not null,
    Std varchar(10) not null,
    Address varchar(200),
    Age int
);
    </pre>

    <h3>Column Explanation</h3>

    <table border="1" cellpadding="10">
        <tr>
            <th>Column Name</th>
            <th>Data Type</th>
            <th>Meaning</th>
        </tr>

        <tr>
            <td>Id</td>
            <td>INT</td>
            <td>Stores numeric student ID</td>
        </tr>

        <tr>
            <td>Name</td>
            <td>VARCHAR(100)</td>
            <td>Stores student name</td>
        </tr>

        <tr>
            <td>Std</td>
            <td>VARCHAR(10)</td>
            <td>Stores class/standard</td>
        </tr>

        <tr>
            <td>Address</td>
            <td>VARCHAR(200)</td>
            <td>Stores address</td>
        </tr>

        <tr>
            <td>Age</td>
            <td>INT</td>
            <td>Stores student age</td>
        </tr>
    </table>

    <hr>

    <h2>Important Keywords</h2>

    <h3>PRIMARY KEY</h3>

    <pre>
Id int primary key
    </pre>

    <ul>
        <li>Uniquely identifies each record.</li>
        <li>Duplicate values are not allowed.</li>
        <li>NULL values are not allowed.</li>
    </ul>

    <h3>NOT NULL</h3>

    <pre>
Name varchar(100) not null
    </pre>

    <ul>
        <li>This field cannot remain empty.</li>
    </ul>

    <h3>VARCHAR</h3>

    <pre>
varchar(100)
    </pre>

    <ul>
        <li>Used to store text data.</li>
        <li>100 means maximum 100 characters allowed.</li>
    </ul>

    <hr>

    <h2>4. View Table Data</h2>

    <pre>
select * from Student;
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li><b>SELECT</b> is used to fetch data.</li>
        <li><b>*</b> means all columns.</li>
    </ul>

    <hr>

    <h2>5. Insert Single Record</h2>

    <pre>
insert into
Student(id,name,std,Address,Age) values
(1,"Harshit","1st","Mumbai",25);
    </pre>

    <h3>Explanation</h3>

    <table border="1" cellpadding="10">
        <tr>
            <th>Part</th>
            <th>Meaning</th>
        </tr>

        <tr>
            <td>INSERT INTO</td>
            <td>Adds data into table</td>
        </tr>

        <tr>
            <td>Student</td>
            <td>Table name</td>
        </tr>

        <tr>
            <td>VALUES</td>
            <td>Actual data</td>
        </tr>
    </table>

    <hr>

    <h2>6. Insert Data Without Column Names</h2>

    <pre>
insert into student values
(2,"Kuldeep","3rd","Delhi",29);
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li>Values must follow the exact column order.</li>
        <li>If column order changes, data may go into wrong columns.</li>
    </ul>

    <hr>

    <h2>7. Insert Multiple Records</h2>

    <pre>
insert into student values
(3,"Rahul","4th","Pune",30),
(4,"Kajal","1st","Ludhiyana",28);
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li>Multiple rows can be inserted in one query.</li>
        <li>Saves time and improves performance.</li>
    </ul>

    <hr>

    <h2>8. Create Teachers Table</h2>

    <pre>
create table Teachers(
TeacherID int primary Key,
Name varchar(100),
Subject varchar(50),
Experience INT,
Email varchar(100));
    </pre>

    <h3>Explanation of Columns</h3>

    <table border="1" cellpadding="10">
        <tr>
            <th>Column</th>
            <th>Meaning</th>
        </tr>

        <tr>
            <td>TeacherID</td>
            <td>Unique teacher ID</td>
        </tr>

        <tr>
            <td>Name</td>
            <td>Teacher name</td>
        </tr>

        <tr>
            <td>Subject</td>
            <td>Subject taught</td>
        </tr>

        <tr>
            <td>Experience</td>
            <td>Years of experience</td>
        </tr>

        <tr>
            <td>Email</td>
            <td>Teacher email</td>
        </tr>
    </table>

    <hr>

    <h2>9. Insert Records into Teachers Table</h2>

    <pre>
insert into Teachers Values
(1,"Aditya","Mathematics",10,"aditya@gmail.com"),
(2,"Aditya2","Mathematics1",10,"aditya@gmail.com"),
(3,"Aditya3","Hindi",10,"aditya@gmail.com"),
(4,"Aditya4","Excel",10,"aditya@gmail.com");
    </pre>

    <hr>

    <h2>10. TRUNCATE TABLE</h2>

    <pre>
truncate table teachers;
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li>Removes all records from the table.</li>
        <li>Table structure remains safe.</li>
        <li>Faster than DELETE.</li>
    </ul>

    <hr>

    <h2>Difference Between DELETE and TRUNCATE</h2>

    <table border="1" cellpadding="10">
        <tr>
            <th>DELETE</th>
            <th>TRUNCATE</th>
        </tr>

        <tr>
            <td>Removes selected rows</td>
            <td>Removes all rows</td>
        </tr>

        <tr>
            <td>Can use WHERE condition</td>
            <td>Cannot use WHERE</td>
        </tr>

        <tr>
            <td>Slower</td>
            <td>Faster</td>
        </tr>
    </table>

    <hr>

    <h2>11. DROP TABLE</h2>

    <pre>
drop table teachers;
    </pre>

    <h3>Explanation</h3>
    <ul>
        <li>Completely deletes the table.</li>
        <li>Both structure and data are removed.</li>
    </ul>

    <hr>

    <h2>Most Important SQL Commands</h2>

    <table border="1" cellpadding="10">
        <tr>
            <th>Command</th>
            <th>Purpose</th>
        </tr>

        <tr>
            <td>CREATE DATABASE</td>
            <td>Creates database</td>
        </tr>

        <tr>
            <td>USE</td>
            <td>Select database</td>
        </tr>

        <tr>
            <td>CREATE TABLE</td>
            <td>Creates table</td>
        </tr>

        <tr>
            <td>INSERT INTO</td>
            <td>Adds data</td>
        </tr>

        <tr>
            <td>SELECT</td>
            <td>Displays data</td>
        </tr>

        <tr>
            <td>TRUNCATE</td>
            <td>Removes all rows</td>
        </tr>

        <tr>
            <td>DROP TABLE</td>
            <td>Deletes table completely</td>
        </tr>
    </table>

    <hr>

    <h2>Conclusion</h2>

    <p>
        This project teaches the foundation of SQL:
    </p>

    <ul>
        <li>Database creation</li>
        <li>Table creation</li>
        <li>Data insertion</li>
        <li>Data retrieval</li>
        <li>Data deletion</li>
    </ul>

    <p>
        These are the most important beginner concepts in SQL and database management.
    </p>
