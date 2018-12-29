TCS hiring Challenge/ Angular UI/UX
For Solution Page View: https://dhiraj2018.github.io/TCS-Hiring-Challenge/tcscustomerform/
Problem Statement:
The below scenario is used to create a Customer details and display the details in same page. In the start up of the project, it need to display Customer Registration form, which contain following attributes; customerName, customerAge, customerMobileNumber. The fields need to be validated during the registration. The customerId is an auto generated one and prefix with the letter ”C”. After successful registration the details need to be populated in a table beneath to the form. The customer listing need to be in the descending order of customerId.

 
•	The customer.service.ts need to be modified to declare a Customer array and should be returned from the class using the methods getCustomers specified in the class.
•	Create a form (in customerregistration.component.html) with following attributes and validations;
•	The form design should be model driven one.
•	The error messages displayed can be template based.
•	While designing the form please make sure that the model driven form attributes should be same as customer model attribute.

 
 
Diagram1 : Customer Registration Screen
 
 
 
Following validations need to apply for the Customer Registration form;

 
Attribute Name	Control	Validation
customerName	TextBox	Mandatory Field. Alphabets only.(required and pattern should be used)
Error Messages:
1) Customer Name is Required
2) Customer Name contains alphabets only
customerAge	TextBox	Mandatory Field. It should be accept only numeric attributes. The value should be between 20-50.(required, pattern, min & max should be used)
Error Messages:
1) Customer Age is Required
2) Customer Age is not a Number
3) Customer Age between 20-50 only
customerMobile	TextBox	Mandatory Field. 10digit number only and starts with 7, 8 or 9. (required and pattern should be used)
Error Messages:
1) Customer Mobile Number is Required
2) Customer Mobile Number not valid
Register	Button	Register button will enable only when we provide the value of all attributes.

 
•	Should display one error message inside the span nearby each input control when validation fails based on the input given. (error messages can be displayed when user touched the input controls and moves out)
•	The customer.service.ts should be loaded inside the Component using dependency injection.
 
Diagram2 : Mandatory validation in Customer Registration Screen
 
Diagram3 : Numeric validation for Customer Age

 
 
Diagram4 : Age & Phone number validation for Customer Registration

 
•	Create one method registerCustomer() in customer.service.ts.
•	The method registerCustomer(), accepts Customer's name, age and mobile number. Stores them in an array of customers along with an auto-generatedcustomerId.
•	After successful registration, the newly added customer details need to be added in to the table beneath to the screen. The customer registration form also need to be reset.
•	The table below should be visible  based on the availability of customer details inside the array else hidden.
•	In the Customer List, the customerId need to preponed with the letter C ie; C-1, C-2 etc.
•	Also the Customer List, need to be listed in the descending order of Customer Id attribute.
 
Diagram5 : Listing screen after registration
 
•	The next customer created also need to be updated in to the list beneath to that. Also the list need to be sorted in the order of customerId descending.

 
 
Diagram6 : Customer Listing screen with three successful customer registration
 
 
Note :
•	Same table header and structure need to be used. Table order need to be maintained
•	The test data given above should be used for form Registration
•	Kindly use the basic template structure given in customerregistration.component.html.

 
Things to remember
•	Before proceeding the coding, install the required dependencies using the menu Run->Install
•	Once the coding is done, run the application in built in server available. To start the server go to Run -> Run Server.
•	After verifying the application, before submitting the implementation click on the Run Test button and ensure that every test cases are cleared.
•	If everything is fine Submit the code using the Submit button.
