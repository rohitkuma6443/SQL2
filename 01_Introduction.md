  <h1>Introduction</h1>
  <p>
    This tutorial introduces the fundamental concepts of databases, Database Management Systems (DBMS), 
    Relational Database Management Systems (RDBMS), MySQL, and SQL. It explains how data is stored, organized, 
    and managed in modern applications, providing a foundation for learning MySQL and database technologies.
  </p>

  <h2>What is a Database?</h2>
  <p>
    A database is an organized collection of data that can be easily accessed, managed, and updated.
  </p>

  <h3>Example</h3>
  <p>Consider a school maintaining student information such as:</p>
  <ul>
    <li>Student ID</li>
    <li>Name</li>
    <li>Class</li>
    <li>Contact Number</li>
  </ul>
  <p>
    Instead of storing this information in separate files, all records can be stored in a database in a structured format.
  </p>

  <h3>Characteristics of a Database</h3>
  <ul>
    <li>Organized storage of data</li>
    <li>Easy retrieval of information</li>
    <li>Efficient data management</li>
    <li>Reduced duplication of data</li>
    <li>Improved security and consistency</li>
  </ul>

  <h2>What is DBMS?</h2>
  <p>
    DBMS (Database Management System) is software used to create, manage, and maintain databases.
  </p>

  <h3>A DBMS provides tools for:</h3>
  <ul>
    <li>Creating databases</li>
    <li>Storing data</li>
    <li>Retrieving data</li>
    <li>Updating records</li>
    <li>Deleting records</li>
    <li>Managing user access</li>
  </ul>

  <h3>Common Functions of DBMS:</h3>
  <ul>
    <li>Data Storage</li>
    <li>Data Retrieval</li>
    <li>Data Modification</li>
    <li>Data Security</li>
    <li>Backup and Recovery</li>
  </ul>

  <h3>Examples of DBMS:</h3>
  <ul>
    <li>MySQL</li>
    <li>Oracle Database</li>
    <li>Microsoft SQL Server</li>
    <li>PostgreSQL</li>
    <li>SQLite</li>
  </ul>

  <h2>What is RDBMS?</h2>
  <p>
    RDBMS (Relational Database Management System) is a type of DBMS that stores data in the form of tables.
  </p>

  <h3>Each table consists of:</h3>
  <ul>
    <li><strong>Rows (Records)</strong> → Individual data entries</li>
    <li><strong>Columns (Fields)</strong> → Attributes of the data</li>
  </ul>

  <h3>Example: Student Table</h3>
  <table border="1" cellpadding="5">
    <tr>
      <th>Student_ID</th>
      <th>Name</th>
      <th>Class</th>
    </tr>
    <tr>
      <td>101</td>
      <td>Rahul</td>
      <td>10</td>
    </tr>
    <tr>
      <td>102</td>
      <td>Priya</td>
      <td>10</td>
    </tr>
    <tr>
      <td>103</td>
      <td>Amit</td>
      <td>9</td>
    </tr>
  </table>

  <h3>Features of RDBMS:</h3>
  <ul>
    <li>Data stored in tables</li>
    <li>Relationships between tables</li>
    <li>Reduced data redundancy</li>
    <li>Better data integrity</li>
    <li>Support for SQL queries</li>
  </ul>

  <h2>Difference Between DBMS and RDBMS</h2>
  <table border="1" cellpadding="5">
    <tr>
      <th>DBMS</th>
      <th>RDBMS</th>
    </tr>
    <tr>
      <td>Stores data as files or simple structures</td>
      <td>Stores data in tables</td>
    </tr>
    <tr>
      <td>Limited relationships between data</td>
      <td>Supports relationships between tables</td>
    </tr>
    <tr>
      <td>Suitable for small applications</td>
      <td>Suitable for large-scale applications</td>
    </tr>
    <tr>
      <td>Less efficient for complex queries</td>
      <td>Highly efficient for complex queries</td>
    </tr>
  </table>

  <h2>What is MySQL?</h2>
  <p>
    MySQL is one of the most popular Relational Database Management Systems (RDBMS) in the world.
  </p>

  <h3>It is widely used in:</h3>
  <ul>
    <li>Web Development</li>
    <li>Enterprise Applications</li>
    <li>E-commerce Platforms</li>
    <li>Content Management Systems</li>
    <li>Data Storage Solutions</li>
  </ul>

  <h3>Why MySQL is Popular:</h3>
  <ul>
    <li>Open-source</li>
    <li>Fast and reliable</li>
    <li>Easy to learn</li>
    <li>Supports large databases</li>
    <li>Widely used in industry</li>
  </ul>

  <h2>What is SQL?</h2>
  <p>
    SQL (Structured Query Language) is the standard language used to communicate with databases.
  </p>

  <h3>SQL helps users:</h3>
  <ul>
    <li>Create databases and tables</li>
    <li>Insert data</li>
    <li>Retrieve data</li>
    <li>Update records</li>
    <li>Delete records</li>
    <li>Manage permissions</li>
  </ul>

  <h3>Example SQL Query:</h3>
  <pre><code>SELECT * FROM Students;</code></pre>
  <p>This query retrieves all records from the Students table.</p>

  <h2>Types of Databases</h2>
  <p>Many database systems are available, including:</p>
  <h3>Relational Databases</h3>
  <ul>
    <li>MySQL</li>
    <li>PostgreSQL</li>
    <li>Oracle</li>
    <li>SQL Server</li>
  </ul>

  <h3>Non-Relational (NoSQL) Databases</h3>
  <ul>
    <li>MongoDB</li>
    <li>Cassandra</li>
    <li>Redis</li>
  </ul>

</body>
</html>
