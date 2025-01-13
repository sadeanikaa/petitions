# SLPP – Shangri-La Petition Platform
**Key Requirements:**
- Register a minimum of two accounts.
- Create a petition on both accouunts.
- Sign a petition on both accounts.

**How to run the web application:**
1. Create a database named _petition_ in my SQL.
2. Update the database credentials in _src/main/resources/application.properties_ .
3. Then run the application.
4. Search http://localhost:8080 in your browser.

**How to navigate through the web application as a _Petitioner_:**
1. (http://localhost:8080) will display the Login page.
2. Enter your credentials if you already have an account (_Email and Password_) and select login.
3. You will then be redirected to the Petitioner Dashboard page (http://localhost:8080/dashboard).
4. If you do not have an account click the _Register_ hyperlink and you'll be redirected to the Register page (http://localhost:8080/register).
5. Enter your credentials (_Email, Full Name, DOB, Password and BioID_) and select register.
6. You will then be redirected to the Petitioner Dashboard page (http://localhost:8080/dashboard).

**How to navigte through the Petitioners Dashboard:**
1. Select _Dashboard_ in the navigation bar to be redirected to see an overview of the Total Petitions,Signed Petitions,Pending Petitions (http://localhost:8080/dashboard).
2. Select _Create Petitions_ in the navigation bar to be redirected to fill out a form to create a petition (http://localhost:8080/petitions/create).
3. Select _View Petitions_ in the navigation bar to be redirected to view and sign submitted petitions (http://localhost:8080/petitions/list).
4. Select Logout in the navigation bar to be redirected to logout of the petitoners account (http://localhost:8080/login?logout).

**How to navigate through the Create Petitions page:**
1. Fill out the petitions form to create a petition.
2. Ensure the fields _Title_ and _Content_ have an input.
3. Select the button _Submit Petition_ for the petition to be created and saved to the database.
4. You will then be redirect back to the dashboard page (http://localhost:8080/dashboard).
5. To view all petitions select the _View Petitions_ in the navigation bar.

**How to navigate through the View Petitions page:**
1. There will be a list of all the petitions submitted.
2. You will then scroll to find petitions that have the status _open_ and press the _sign_ button.

**How to navigate the web application as an Admin:**
1. On the main page (http://localhost:8080) select the hyperlink _Login as Admin_ under the login for to access the Admin Login.
2. Fill out the login form with the required credentials (Email: admin@petition.parliament.sr and Password: 2025%shangrila).
3. You will now have access to the Petitions Committee Dashboard/Admin Dashboard (http://localhost:8080/admin/dashboard).

**How to navigate through the Petitions Committee Dashboard:**
1. On the petitions committee dashboard page you are able to set a signature threshold by pressing the _Update_ button, and add a response to petitions that have met the threshold by pressing the button _Add Response_.
2. You will then be redirected to another page to add a response to the petition in the required field (http://localhost:8080/admin/petitions/10/response) and then press _Submit Response_ and you'll be redirected back to the petitions committee dashboard page.
3. The petition will then display the _Status_ and _Action_ as _Closed_.
