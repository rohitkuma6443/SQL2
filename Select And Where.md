```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>Video 8 MySQL SELECT Query Notes</title>
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <style>
    body { font-family: Arial, sans-serif; line-height: 1.6; padding: 24px; max-width: 900px; margin: auto; color: #111; }
    h1,h2,h3 { color: #0b5ed7; }
    pre { background:#f6f8fa; padding:12px; border-radius:6px; overflow:auto; }
    table { border-collapse: collapse; width:100%; margin:12px 0; }
    table, th, td { border:1px solid #dfe3e8; }
    th, td { padding:8px 10px; text-align:left; }
    .note { background:#fff8e6; padding:10px; border-left:4px solid #f0ad4e; margin:12px 0; }
    ul { margin:8px 0 16px 20px; }
  </style>
</head>
<body>

  <h1>Video 8: MySQL SELECT Query – How to Read Data from MySQL Database?</h1>

  <h2>Introduction</h2>
  <p>
    The <code>SELECT</code> statement is used to retrieve data from a MySQL database. It is the most commonly used SQL command for reading and analyzing data stored in tables.
  </p>

  <hr />

  <h2>Sample Table student</h2>

  <h3>Table Structure</h3>
  <table>
    <tr>
      <th>Column</th>
      <th>Data Type</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>id</td>
      <td>INT</td>
      <td>Student ID</td>
    </tr>
    <tr>
      <td>name</td>
      <td>VARCHAR(50)</td>
      <td>Student Name</td>
    </tr>
    <tr>
      <td>city</td>
      <td>VARCHAR(50)</td>
      <td>City</td>
    </tr>
    <tr>
      <td>age</td>
      <td>INT</td>
      <td>Age</td>
    </tr>
    <tr>
      <td>marks</td>
      <td>INT</td>
      <td>Marks</td>
    </tr>
  </table>

  <h3>Sample Data</h3>
  <table>
    <tr>
      <th>id</th>
      <th>name</th>
      <th>city</th>
      <th>age</th>
      <th>marks</th>
    </tr>
    <tr>
      <td>101</td>
      <td>Rahul</td>
      <td>Mumbai</td>
      <td>20</td>
      <td>85</td>
    </tr>
    <tr>
      <td>102</td>
      <td>Priya</td>
      <td>Delhi</td>
      <td>21</td>
      <td>92</td>
    </tr>
    <tr>
      <td>103</td>
      <td>Amit</td>
      <td>Mumbai</td>
      <td>19</td>
      <td>78</td>
    </tr>
    <tr>
      <td>104</td>
      <td>Sneha</td>
      <td>Pune</td>
      <td>22</td>
      <td>88</td>
    </tr>
    <tr>
      <td>105</td>
      <td>Rohan</td>
      <td>Delhi</td>
      <td>20</td>
      <td>95</td>
    </tr>
  </table>

  <hr />

  <h2>SELECT Query Read All Data</h2>

  <h3>Syntax</h3>
  <pre><code>SELECT * FROM table_name;</code></pre>

  <h3>Example</h3>
  <pre><code>SELECT * FROM student;</code></pre>

  <p><strong>Result:</strong> Retrieves all rows and all columns from the table.</p>

  <hr />

  <h2>SELECT Specific Columns</h2>

  <h3>Syntax</h3>
  <pre><code>SELECT column1, column2 FROM table_name;</code></pre>

  <h3>Example</h3>
  <pre><code>SELECT name, city FROM student;</code></pre>

  <p><strong>Result:</strong> Retrieves only the selected columns.</p>

  <hr />

  <h2>WHERE Clause Filtering Data</h2>

  <h3>Syntax</h3>
  <pre><code>SELECT column_name
FROM table_name
WHERE condition;</code></pre>

  <h3>Example Filter by City</h3>
  <pre><code>SELECT * FROM student
WHERE city = 'Mumbai';</code></pre>

  <h3>Example Filter by ID</h3>
  <pre><code>SELECT * FROM student
WHERE id = 103;</code></pre>

  <p class="note"><strong>Note:</strong> Use the <code>WHERE</code> clause to return only rows that meet the specified condition.</p>

  <hr />

  <h2>Key Points</h2>
  <ul>
    <li><strong>SELECT</strong> is used to read data from tables.</li>
    <li><strong>*</strong> means all columns.</li>
    <li>Select specific columns for better performance and clarity.</li>
    <li><strong>WHERE</strong> filters rows based on conditions.</li>
    <li><strong>SELECT</strong> is the most frequently used SQL command.</li>
  </ul>

  <h3>Best Practice</h3>
  <p>Avoid using <code>SELECT *</code> in production queries. Prefer selecting only required columns.</p>
  <pre><code>-- Avoid
SELECT * FROM student;

-- Prefer
SELECT name, city
FROM student
WHERE city = 'Delhi';</code></pre>

  <hr />

  <h2>Exercises Practice</h2>

  <ol>
    <li><strong>Exercise 1</strong> — Write a query to display all data from the <code>student</code> table.</li>
    <li><strong>Exercise 2</strong> — Write a query to display only <code>name</code> and <code>city</code> from the <code>student</code> table.</li>
    <li><strong>Exercise 3</strong> — Write a query to display students whose <code>city</code> is <strong>Mumbai</strong>.</li>
    <li><strong>Exercise 4</strong> — Write a query to find the student whose <code>id = 105</code>.</li>
    <li><strong>Exercise 5</strong> — Write a query to display students whose <code>marks</code> are greater than 85.</li>
    <li><strong>Exercise 6</strong> — Write a query to display <code>name</code> and <code>marks</code> of students from <strong>Delhi</strong>.</li>
    <li><strong>Exercise 7</strong> — Write a query to display all students from the <code>student</code> table using proper SELECT syntax.</li>
  </ol>

  <hr />

  <h2>Summary</h2>
  <p>
    The <code>SELECT</code> statement retrieves data from MySQL tables. Use <code>SELECT *</code> to read all data, select specific columns for efficiency, and apply <code>WHERE</code> to filter results. Mastering <code>SELECT</code> is essential for working with databases.
  </p>

</body>
</html>
```
