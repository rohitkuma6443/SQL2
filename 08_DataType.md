```html id="8q4n2x"
<h1>MySQL Datatypes Notes</h1>

<h3>Topics Covered</h3>

<ul>
    <li>Introduction to Datatypes</li>
    <li>Why Datatypes are Important</li>
    <li>Numeric Datatypes</li>
    <li>String Datatypes</li>
    <li>Date and Time Datatypes</li>
    <li>Choosing Correct Datatypes</li>
    <li>Create Table Example</li>
</ul>

<hr>

<h2>1. What are Datatypes in MySQL?</h2>

<p>
Datatypes in MySQL define the type of value that can be stored inside a table column.
</p>

<p>
Each column in a database table must have a datatype.
</p>

<hr>

<h2>2. Why Datatypes are Important?</h2>

<ul>
    <li>Helps organize data properly.</li>
    <li>Improves database performance.</li>
    <li>Saves storage space.</li>
    <li>Prevents invalid data entry.</li>
    <li>Makes searching and calculations faster.</li>
</ul>

<hr>

<h2>3. Example of Datatypes</h2>

<table border="1">

<tr>
    <th>Column Name</th>
    <th>Datatype</th>
    <th>Reason</th>
</tr>

<tr>
    <td>ID</td>
    <td>INT</td>
    <td>Stores numeric values</td>
</tr>

<tr>
    <td>Name</td>
    <td>VARCHAR(100)</td>
    <td>Stores text values</td>
</tr>

<tr>
    <td>Salary</td>
    <td>DECIMAL(10,2)</td>
    <td>Stores decimal numbers</td>
</tr>

<tr>
    <td>DateOfBirth</td>
    <td>DATE</td>
    <td>Stores date values</td>
</tr>

</table>

<hr>

<h2>4. Categories of Datatypes</h2>

<ul>
    <li>Numeric Datatypes</li>
    <li>String Datatypes</li>
    <li>Date and Time Datatypes</li>
</ul>

<hr>

<h2>5. Numeric Datatypes</h2>

<p>
Numeric datatypes are used to store numbers.
</p>

<table border="1">

<tr>
    <th>Datatype</th>
    <th>Description</th>
</tr>

<tr>
    <td>INT</td>
    <td>Stores whole numbers</td>
</tr>

<tr>
    <td>BIGINT</td>
    <td>Stores very large integers</td>
</tr>

<tr>
    <td>DECIMAL</td>
    <td>Stores exact decimal values</td>
</tr>

<tr>
    <td>FLOAT</td>
    <td>Stores floating point numbers</td>
</tr>

</table>

<hr>

<h2>6. String Datatypes</h2>

<p>
String datatypes are used to store text values.
</p>

<table border="1">

<tr>
    <th>Datatype</th>
    <th>Description</th>
</tr>

<tr>
    <td>CHAR</td>
    <td>Stores fixed-length text</td>
</tr>

<tr>
    <td>VARCHAR</td>
    <td>Stores variable-length text</td>
</tr>

<tr>
    <td>TEXT</td>
    <td>Stores large text data</td>
</tr>

</table>

<hr>

<h2>7. Difference Between CHAR and VARCHAR</h2>

<table border="1">

<tr>
    <th>CHAR</th>
    <th>VARCHAR</th>
</tr>

<tr>
    <td>Fixed length</td>
    <td>Variable length</td>
</tr>

<tr>
    <td>Faster</td>
    <td>Saves storage space</td>
</tr>

<tr>
    <td>Wastes extra space</td>
    <td>Uses only required space</td>
</tr>

</table>

<hr>

<h2>8. Date and Time Datatypes</h2>

<p>
These datatypes are used to store date and time values.
</p>

<table border="1">

<tr>
    <th>Datatype</th>
    <th>Description</th>
</tr>

<tr>
    <td>DATE</td>
    <td>Stores date (YYYY-MM-DD)</td>
</tr>

<tr>
    <td>TIME</td>
    <td>Stores time values</td>
</tr>

<tr>
    <td>DATETIME</td>
    <td>Stores both date and time</td>
</tr>

<tr>
    <td>TIMESTAMP</td>
    <td>Stores timestamp values</td>
</tr>

</table>

<hr>

<h2>9. Create Table Example Using Datatypes</h2>

<pre>
create table Employee(

    ID int primary key,
    Name varchar(100),
    Salary decimal(10,2),
    JoiningDate date,
    LoginTime time

);
</pre>

<hr>

<h2>10. Explanation of Table Columns</h2>

<table border="1">

<tr>
    <th>Column</th>
    <th>Datatype</th>
    <th>Purpose</th>
</tr>

<tr>
    <td>ID</td>
    <td>INT</td>
    <td>Stores employee ID</td>
</tr>

<tr>
    <td>Name</td>
    <td>VARCHAR(100)</td>
    <td>Stores employee name</td>
</tr>

<tr>
    <td>Salary</td>
    <td>DECIMAL(10,2)</td>
    <td>Stores salary with decimal values</td>
</tr>

<tr>
    <td>JoiningDate</td>
    <td>DATE</td>
    <td>Stores joining date</td>
</tr>

<tr>
    <td>LoginTime</td>
    <td>TIME</td>
    <td>Stores login time</td>
</tr>

</table>

<hr>

<h2>11. Choosing the Correct Datatype</h2>

<ul>
    <li>Choose datatype based on data type.</li>
    <li>Select proper size to save memory.</li>
    <li>Use numeric datatypes for calculations.</li>
    <li>Use string datatypes for names and text.</li>
    <li>Use date/time datatypes for date-related data.</li>
</ul>

<hr>

<h2>12. Important Notes</h2>

<ul>
    <li>Wrong datatype selection can reduce performance.</li>
    <li>Correct datatype improves speed and storage efficiency.</li>
    <li>Large databases require careful datatype planning.</li>
</ul>

<hr>

<h2>13. Most Commonly Used Datatypes</h2>

<table border="1">

<tr>
    <th>Datatype</th>
    <th>Usage</th>
</tr>

<tr>
    <td>INT</td>
    <td>Whole numbers</td>
</tr>

<tr>
    <td>VARCHAR</td>
    <td>Text values</td>
</tr>

<tr>
    <td>DECIMAL</td>
    <td>Decimal numbers</td>
</tr>

<tr>
    <td>DATE</td>
    <td>Date values</td>
</tr>

<tr>
    <td>DATETIME</td>
    <td>Date and time</td>
</tr>

</table>

<hr>

<h2>Conclusion</h2>

<ul>
    <li>Datatypes define what type of data can be stored.</li>
    <li>Different datatypes are used for different purposes.</li>
    <li>Choosing the correct datatype improves database performance.</li>
    <li>Datatypes help maintain data accuracy and efficiency.</li>
</ul>
```
