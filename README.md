# Python-interactive-data-visualization
Python script is a simple Streamlit web application for data visualization with a login section

**#Libraries Used**

**streamlit**: A popular Python library for creating web applications with minimal code.
pandas: Used for data manipulation and analysis.
numpy: Provides support for large, multi-dimensional arrays and matrices.
plotly.express: Used for creating interactive plots and visualizations.
sqlite3: Python interface to SQLite, a lightweight relational database management system.

**Security Functions:**
make_hashes: Hashes a password using SHA-256 for secure storage.
check_hashes: Compares a password with its hashed version to verify login credentials.

**Database Management:**
Connects to an SQLite database named 'data.db'.
Creates a table named 'userstable' to store user credentials.
Defines functions for adding users to the table, retrieving user data, and viewing all users.

**Main Function:**
The main function sets up a simple menu using Streamlit's sidebar.
The "Home" option displays a public view using the plotly.express library, specifically scatter and bar plots with sample data from the Iris and Tips datasets.
The "Login" option allows users to input a username and password. If the credentials are correct, the script displays interactive plots using plotly.express.

**Web Application Flow:**
Users enter their credentials in the login section.
The script checks the credentials against the stored hashed passwords in the SQLite database.
If the login is successful, the web application displays interactive data visualizations.

**Note:**
The script uses sample data from plotly.express for demonstration purposes.
It's important to enhance security measures for a production environment (e.g., using secure password storage, user authentication tokens, HTTPS).
