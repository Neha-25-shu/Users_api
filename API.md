 API Documentation
-----------------
Base URL for all API endpoints : `http://127.0.0.1:8000/` <br />

i. User - Registration
Create/ Register a new user.

	Endpoint 	: /rest_auth/registration/
	Request Type 	: POST
	Request Params 	: username, email, password, password_2
	Non-mandatory params : invite_code

	Response Http status codes : HTTP_200_OK or HTTP_400_BAD_REQUEST
	
ii. User - Login
Obtain authentication token given the user credentials.

	Endpoint 	: /rest_auth/login/
	Request Type 	: POST
	Request Params 	: email (or username) and password
	
	Response 	: { "token": <token> }
	HTTP status code: HTTP_200_OK or HTTP_400_BAD_REQUEST
	
iii. User - Request for Password Reset
Receive an email with password reset link.

	Endpoint 	: http://127.0.0.1:8000/reset_password/
	Request Type 	: POST
	Request Params 	: email
	Request Sample : {"email": "some_email_id@gmail.com"}
	
	HTTP status code: HTTP_200_OK

iv. User - Password Change
    Change the password. Link as recieved from email by above request (iii).
	
	Endpoint 	: http://127.0.0.1:8000/reset_password_complete/<reset_code>/
	Request Type 	: POST
	Request Sample : {"new_password": "33441122", "new_password_2": "33441122"}
	
	HTTP status code: HTTP_200_OK or HTTP_400_BAD_REQUEST


