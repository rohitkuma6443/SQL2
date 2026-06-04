<h1>Custom Installation of MySQL (Workbench + Documentation)</h1>

  <h2>Introduction</h2>
  <p>
    During the MySQL installation process, you can choose the <strong>Custom</strong> setup type to manually select the components you want to install. 
    If your goal is to install <strong>MySQL Workbench</strong> and <strong>MySQL Documentation</strong>, this option allows you to choose only the required components.
  </p>

  <hr>

  <h2>Step 1: Launch MySQL Installer</h2>
  <ol>
    <li>Open the MySQL Installer.</li>
    <li>Select <strong>Custom</strong> as the setup type.</li>
    <li>Click <strong>Next</strong> to proceed.</li>
  </ol>

  <hr>

  <h2>Step 2: Select Components</h2>
  <h3>MySQL Workbench</h3>
  <p>Navigate to:</p>
  <p><em>Applications → MySQL Workbench</em></p>
  <p>Move <strong>MySQL Workbench</strong> to the "Products to Be Installed" section.</p>

  <h3>MySQL Documentation</h3>
  <p>Navigate to:</p>
  <p><em>Documentation → MySQL Documentation</em></p>
  <p>Move <strong>MySQL Documentation</strong> to the installation list.</p>

  <hr>

  <h2>Recommended Additional Component</h2>
  <p>
    If you want to create and manage databases on your computer, you should also install:
  </p>
  <p><em>MySQL Servers → MySQL Server</em></p>
  <p>
    Without <strong>MySQL Server</strong>, Workbench can only connect to an existing MySQL database server and cannot store databases locally.
  </p>

  <h3>Recommended Selection</h3>
  <ul>
    <li>MySQL Server</li>
    <li>MySQL Workbench</li>
    <li>MySQL Documentation</li>
  </ul>

  <hr>

  <h2>Step 3: Install the Selected Components</h2>
  <ol>
    <li>Click <strong>Next</strong>.</li>
    <li>Review the selected products.</li>
    <li>Install any required prerequisites if prompted.</li>
    <li>Click <strong>Execute</strong> to begin the installation.</li>
  </ol>
  <p>Wait until all components are installed successfully.</p>

  <hr>

  <h2>Step 4: Configure MySQL Server</h2>
  <p>If MySQL Server is installed, complete the configuration wizard:</p>

  <h3>Configuration Settings</h3>
  <ul>
    <li>Server Type: <strong>Development Machine</strong></li>
    <li>Port Number: <strong>3306</strong></li>
    <li>Authentication Method: <strong>Strong Password Encryption</strong></li>
    <li>Root User: <strong>root</strong></li>
    <li>Set a secure root password</li>
  </ul>
  <p>Apply the configuration and finish the setup process.</p>

  <hr>

  <h2>Step 5: Verify the Installation</h2>
  <p>Open <strong>MySQL Workbench</strong> and create a connection using:</p>
  <ul>
    <li>Hostname: localhost</li>
    <li>Port: 3306</li>
    <li>Username: root</li>
    <li>Password: Your configured root password</li>
  </ul>
  <p>Test the connection and connect to the server.</p>

  <hr>

  <h2>Step 6: Run a Test Query</h2>
  <p>Execute the following query in MySQL Workbench:</p>
  <pre><code>SELECT VERSION();</code></pre>
  <p>If MySQL returns its version number, the installation has been completed successfully.</p>

  <hr>

  <h2>Conclusion</h2>
  <p>
    For beginners learning MySQL, the recommended custom installation includes:
  </p>
  <ul>
    <li>MySQL Server</li>
    <li>MySQL Workbench</li>
    <li>MySQL Documentation</li>
  </ul>

