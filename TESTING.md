 # Testing 

## Automated Testing

### Validation Services

  * **HTML**: I have used [https://validator.w3.org/](https://validator.w3.org/) in order to validate the HTML code.

  * **CSS**: I have used [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/) in order to validate the CSS code.

  * **JavaScript**: I have used [https://jshint.com/](https://jshint.com/) in order to check the JavaScript code.

  * **Python** I used [PEP8 Online]: (http://pep8online.com/) to validate Python.

### Coverage
coverage.py was used to provide feedback during testing to check that enough of my code had been tested.

 I built 41 different tests to encompass most of my python views, forms, and models. Using the coverage.py test package.

 In some cases the tests were quite complicated and in these cases I have chosen to test manually since I was running out of time to present the project.

How to run coverage
  * Activate your virtual environment.
  * In the terminal enter the following command:
    * coverage html
    * Open the newly created htmlcov directory in the root of your project folder.
    * Open the index.html file inside it.
    * Run the file in the browser to see the output.

#### Stripe payment testing

My checkout app is using the stripe payment for the payment option. I tested this by using Stripes test card (4242 4242 4242 4242) I tested the forms and ensured all my validation worked as expected and my logic was performing as expected. The checkout app works from the Stripe API.

Card number - 4242424242424242

CVC - Any 3 digit number.

Expiry date - Any date in the future.


### Responsiveness

Chrome DevTools and physical devices were used throughout development for a number of purposes, one of which was to test the responsiveness and rendering across a range of sizes and devices. As issues were found they were either fixed at the time or noted and returned to later.

The site has been tested successfully on

Apple Macbook Air - Safari browser

Apple iPhone 6,7 &8S - Safari Browser

iPad Mini - Safari Browser

Desktop - Chrome v.74

Desktop - Firefox v.67

 * **REGISTER** 
I've created my own account, and 3 other accounts to confirm that the authentication and validation for creating account worked as expected.

* **LOG IN AND LOG OUT** * Logging To An Existing Account
The accounts created were tested by attempting log in and out. No issues found or expected. Using a non-existing user or incorrect password yield errors. Django messages confirmed
the user if attempts to log in/out were successful.

* **Add | View | Edit | Delete a Service**
I've created 3 services (loaded from the json file) and 1 test service created directly from the admin account in order to:
Show the application functionality.
Tested grid/list view btn and search database.
The data validation in the add service form is solid and only accepts input in the correct format.
    * Services has been modified in several ocassion to test the functionality of updating/deleting a service to the 2 database (local and for deployment) and for a user-friendly display. 
Tested edit and delete service buttons are available for the admin of the services, and hidden for non-site admin. 
To prevent admin from deleting aservice card by mistake modal checks were added. When the delete button is pressed, a modal asks the admin to confirm deletion. 
if the admin selects cancel, they are taken back to all the services tab.
     
**SEARCH**
- Search by inputting a clothing item into the search field and clicking the search button redirects to the correct search page with the filtered results.

**Navigation Bar**
- Correct links are displayed `Milestone Four`, `Clothing`, `All Products`, `Special Offers`, clicking the links redirect to the correct page.
