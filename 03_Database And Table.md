  <h2>What is a Database?</h2>
  <p>
    A <strong>database</strong> is an organized collection of data that allows easy storage, retrieval, and management of information.
  </p>

  <h3>Example</h3>
  <ul>
    <li>Student information</li>
    <li>Teacher information</li>
    <li>Course details</li>
  </ul>
  <p>A database contains one or more <strong>tables</strong>.</p>

  <hr>

  <h2>Creating a Database</h2>
  <h3>Syntax</h3>
  <pre><code>CREATE DATABASE database_name;</code></pre>

  <h3>Example</h3>
  <pre><code>CREATE DATABASE school;</code></pre>

  <hr>

  <h2>Viewing Databases</h2>
  <pre><code>SHOW DATABASES;</code></pre>

  <hr>

  <h2>Selecting a Database</h2>
  <pre><code>USE school;</code></pre>
  <p>After this command, all tables will be created inside the <strong>school</strong> database.</p>

  <hr>

  <h2>What is a Table?</h2>
  <p>
    A <strong>table</strong> is a collection of related data stored in rows and columns.
  </p>

  <h3>Example</h3>
  <table border="1" cellpadding="5">
    <tr>
      <th>Student_ID</th>
      <th>Name</th>
      <th>City</th>
    </tr>
    <tr>
      <td>101</td>
      <td>Rahul</td>
      <td>Mumbai</td>
    </tr>
    <tr>
      <td>102</td>
      <td>Priya</td>
      <td>Delhi</td>
    </tr>
  </table>

  <h3>Components</h3>
  <ul>
    <li><strong>Rows</strong> → Records</li>
    <li><strong>Columns</strong> → Fields</li>
    <li><strong>Data Types</strong> → Define the type of data stored</li>
  </ul>

  <hr>

  <h2>CREATE TABLE Statement</h2>
  <h3>Syntax</h3>
  <pre><code>CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
    column3 datatype
);</code></pre>

  <h3>Example</h3>
  <pre><code>CREATE TABLE student (
    student_id INT,
    student_name VARCHAR(50),
    city VARCHAR(50)
);</code></pre>

  <hr>

  <h2>Common Data Types</h2>
  <table border="1" cellpadding="5">
    <tr>
      <th>Data Type</th>
      <th>Purpose</th>
    </tr>
    <tr>
      <td>INT</td>
      <td>Whole numbers</td>
    </tr>
    <tr>
      <td>VARCHAR(n)</td>
      <td>Text values</td>
    </tr>
    <tr>
      <td>FLOAT</td>
      <td>Decimal numbers</td>
    </tr>
    <tr>
      <td>DATE</td>
      <td>Date values</td>
    </tr>
    <tr>
      <td>BOOLEAN</td>
      <td>True/False values</td>
    </tr>
  </table>

  <hr>

  <h2>Examples</h2>
  <h3>Example 1: Student Table</h3>
  <pre><code>CREATE TABLE student (
    student_id INT,
    student_name VARCHAR(50),
    city VARCHAR(50)
);</code></pre>

  <h3>Example 2: Customer Table</h3>
  <pre><code>CREATE TABLE customer (
    customer_id INT,
    customer_name VARCHAR(50),
    city VARCHAR(50)
);</code></pre>

  <h3>Example 3: Employee Table</h3>
  <pre><code>CREATE TABLE employee (
    emp_id INT,
    emp_name VARCHAR(100),
    department VARCHAR(50),
    salary FLOAT
);</code></pre>

  <h3>Example 4: Product Table</h3>
  <pre><code>CREATE TABLE product (
    product_id INT,
    product_name VARCHAR(100),
    price FLOAT,
    quantity INT
);</code></pre>

  <h3>Example 5: Book Table</h3>
  <pre><code>CREATE TABLE book (
    book_id INT,
    title VARCHAR(100),
    author VARCHAR(100)
);</code></pre>

  <hr>

  <h2>Viewing Tables</h2>
  <pre><code>SHOW TABLES;</code></pre>

  <h2>Describing a Table</h2>
  <pre><code>DESCRIBE student;</code></pre>
  <p>or</p>
  <pre><code>DESC student;</code></pre>

  <hr>

  <h2>Table with Constraints</h2>
  <pre><code>CREATE TABLE student (
    student_id INT PRIMARY KEY,
    student_name VARCHAR(50) NOT NULL,
    city VARCHAR(50)
);</code></pre>

  <h3>Constraints</h3>
  <ul>
    <li><strong>PRIMARY KEY</strong> → Unique value for each record.</li>
    <li><strong>NOT NULL</strong> → Prevents empty values.</li>
  </ul>

  <hr>

  <h1>Practice Exercises</h1>
  <h3>Exercise 1</h3>
  <p>Create a database named <code>college_db</code>.</p>

  <h3>Exercise 2</h3>
  <p>Create a table named <code>college</code> with:</p>
  <ul>
    <li>college_id</li>
    <li>college_name</li>
    <li>city</li>
  </ul>

  <h3>Exercise 3</h3>
  <p>Create a table named <code>teacher</code> with:</p>
  <ul>
    <li>teacher_id</li>
    <li>teacher_name</li>
    <li>subject</li>
  </ul>

  <h3>Exercise 4</h3>
  <p>Create a table named <code>hospital</code> with:</p>
  <ul>
    <li>patient_id</li>
    <li>patient_name</li>
    <li>disease</li>
    <li>age</li>
  </ul>

  <h3>Exercise 5</h3>
  <p>Create a table named <code>mobile</code> with:</p>
  <ul>
    <li>mobile_id</li>
    <li>brand</li>
    <li>model</li>
    <li>price</li>
  </ul>

  <hr>

  <h2>Important Commands Summary</h2>
  <h3>Create Database</h3>
  <pre><code>CREATE DATABASE database_name;</code></pre>

  <h3>Show Databases</h3>
  <pre><code>SHOW DATABASES;</code></pre>

  <h3>Select Database</h3>
  <pre><code>USE database_name;</code></pre>

  <h3>Create Table</h3>
  <pre><code>CREATE TABLE table_name (
    column_name datatype,
    column_name datatype
);</code></pre>

  <h3>Show Tables</h3>
  <pre><code>SHOW TABLES;</code></pre>

  <h3>Describe Table</h3>
  <pre><code>DESC table_name;</code></pre>

  <hr>

  <h2>Key Points to Remember</h2>
  <ol>
    <li>A database stores multiple tables.</li>
    <li>Create a database using <code>CREATE DATABASE</code>.</li>
    <li>Select a database using <code>USE</code>.</li>
    <li>Create tables using <code>CREATE TABLE</code>.</li>
    <li>Every column must have a data type.</li>
    <li>Use <code>SHOW DATABASES</code> and <code>SHOW TABLES</code> to verify creation.</li>
    <li>Use <code>DESC</code> to view table structure.</li>
    <li>Constraints such as <code>PRIMARY KEY</code> and <code>NOT NULL</code> help maintain data integrity.</li>
  </ol>
