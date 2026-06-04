

  <h1>SQL Commands – DDL DML DCL TCL DQL Interview Notes</h1>

  <h2>Introduction</h2>
  <p>
    SQL commands let you communicate with a database to define structures, manipulate data, control access, handle transactions, and retrieve information.
    Commands are grouped into five main categories: <strong>DDL</strong>, <strong>DML</strong>, <strong>DQL</strong>, <strong>DCL</strong>, and <strong>TCL</strong>.
  </p>

  <hr />

  <h2>DDL Data Definition Language</h2>
  <p>
    <strong>Purpose</strong> — Define or modify the structure of database objects such as databases and tables.
  </p>

  <h3>Common Commands</h3>
  <ul>
    <li><code>CREATE</code></li>
    <li><code>ALTER</code></li>
    <li><code>DROP</code></li>
    <li><code>TRUNCATE</code></li>
    <li><code>RENAME</code></li>
  </ul>

  <h3>Example</h3>
  <pre><code>CREATE TABLE student (
  id INT,
  name VARCHAR(50)
);</code></pre>

  <p class="summary"><strong>Key Point</strong> — DDL works on the database schema (structure), not on the data itself.</p>

  <hr />

  <h2>DML Data Manipulation Language</h2>
  <p>
    <strong>Purpose</strong> — Insert, update, and delete data stored in tables.
  </p>

  <h3>Common Commands</h3>
  <ul>
    <li><code>INSERT</code></li>
    <li><code>UPDATE</code></li>
    <li><code>DELETE</code></li>
  </ul>

  <h3>Example</h3>
  <pre><code>INSERT INTO student (id, name)
VALUES (1, 'Rahul');</code></pre>

  <p class="summary"><strong>Key Point</strong> — DML operates on table data; many DML changes can be rolled back within transactions.</p>

  <hr />

  <h2>DQL Data Query Language</h2>
  <p>
    <strong>Purpose</strong> — Retrieve data from the database.
  </p>

  <h3>Primary Command</h3>
  <ul>
    <li><code>SELECT</code></li>
  </ul>

  <h3>Example</h3>
  <pre><code>SELECT * FROM student;</code></pre>

  <p class="summary"><strong>Key Point</strong> — DQL is read-only and used for querying and reporting.</p>

  <hr />

  <h2>DCL Data Control Language</h2>
  <p>
    <strong>Purpose</strong> — Manage permissions and access control for database users.
  </p>

  <h3>Common Commands</h3>
  <ul>
    <li><code>GRANT</code></li>
    <li><code>REVOKE</code></li>
  </ul>

  <h3>Example</h3>
  <pre><code>GRANT SELECT ON student TO user1;</code></pre>

  <p class="summary"><strong>Key Point</strong> — DCL commands are used for security and permission management.</p>

  <hr />

  <h2>TCL Transaction Control Language</h2>
  <p>
    <strong>Purpose</strong> — Control transaction boundaries to ensure data integrity.
  </p>

  <h3>Common Commands</h3>
  <ul>
    <li><code>COMMIT</code></li>
    <li><code>ROLLBACK</code></li>
    <li><code>SAVEPOINT</code></li>
  </ul>

  <h3>Example</h3>
  <pre><code>COMMIT;</code></pre>

  <p class="summary"><strong>Key Point</strong> — TCL ensures atomicity and consistency of grouped operations.</p>

  <hr />

  <h2>Quick Summary Table</h2>
  <table class="quick-table">
    <tr>
      <th>Category</th>
      <th>Full Form</th>
      <th>Purpose</th>
      <th>Example Command</th>
    </tr>
    <tr>
      <td>DDL</td>
      <td>Data Definition Language</td>
      <td>Structure management</td>
      <td>CREATE</td>
    </tr>
    <tr>
      <td>DML</td>
      <td>Data Manipulation Language</td>
      <td>Data modification</td>
      <td>INSERT</td>
    </tr>
    <tr>
      <td>DQL</td>
      <td>Data Query Language</td>
      <td>Data retrieval</td>
      <td>SELECT</td>
    </tr>
    <tr>
      <td>DCL</td>
      <td>Data Control Language</td>
      <td>Permission control</td>
      <td>GRANT</td>
    </tr>
    <tr>
      <td>TCL</td>
      <td>Transaction Control Language</td>
      <td>Transaction control</td>
      <td>COMMIT</td>
    </tr>
  </table>

  <hr />

  <h2>Interview Questions Practice</h2>

  <h3>Basic Level</h3>
  <ol>
    <li>What are the main SQL command types?</li>
    <li>Which command is used to create a table?</li>
    <li>What is the difference between DDL and DML?</li>
  </ol>

  <h3>Intermediate Level</h3>
  <ol>
    <li>What is the use of the <code>SELECT</code> command?</li>
    <li>What is the difference between <code>DELETE</code> and <code>TRUNCATE</code>?</li>
    <li>What is a transaction in SQL?</li>
  </ol>

  <h3>Advanced Level</h3>
  <ol>
    <li>What is the difference between <code>COMMIT</code> and <code>ROLLBACK</code>?</li>
    <li>What are DCL commands used for?</li>
    <li>Explain why SQL is called a query language.</li>
  </ol>

  <hr />

  <h2>Key Points to Remember</h2>
  <ul>
    <li>SQL commands are grouped into five categories.</li>
    <li><strong>DDL</strong> manages structure; <strong>DML</strong> manipulates data; <strong>DQL</strong> retrieves data.</li>
    <li><strong>DCL</strong> controls permissions; <strong>TCL</strong> manages transactions.</li>
    <li>Understand differences and real-world use cases for interview readiness.</li>
  </ul>

  <hr />

  <h2>Final Note</h2>
  <p>
    Interviewers often ask for differences between commands, example scenarios, and how transactions and permissions are handled in real systems. Practice writing short SQL snippets for each category and explaining when and why you would use them.
  </p>
