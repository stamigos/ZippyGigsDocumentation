# [Auth](authorization.md)

## [POST /api/v1/auth/signup/](authorization.md#post-apiv1authsignup)

Create a new user account with the provided data.

### Input Data

Field name | Type | Description
------------ | ------------- | ------------
`email` | **Required**  | Email-address the user should be signed up with.
`password` | **Required**  | Password for the new account.

### Response example
	{
		"data": {
		"created": "Sun, 16 Oct 2016 18:25:44 GMT", 
		"email": "fortest@example.com", 
		"id": 5, 
		"is_active": true, 
		"password": "7110eda4d09e062aa5e4a390b0a572ac0d2c0220", 
		"type": 3
		}, 
	  "error": null, 
	  "result": true
	}

## [POST /api/v1/auth/token/](authorization.md#post-apiv1authtoken)

Check the credentials and return the token if the credentials are valid and authenticated.

### Input Data

Field name | Type | Description
------------ | ------------- | ------------
`email` | **Required**  | Email of the user to login.
`password` | **Required**  | Password of the user to login.

### Response example
	{
	  "data": {
	    "token": "eyJhbGciOiJIUzI1NiIsImV4cCI6MTQ3NjYzMjY3NiwiaWF0IjoxNDc2NjMyMDc2fQ.eyJpZCI6NX0.aVM2-39F_G6sdNnPXPHYFQV-lW-DiDwGRfInkcpBp8s"
	  }, 
	  "error": null, 
	  "result": true
	}

## [POST /api/v1/auth/profile/](authorization.md#post-apiv1authprofile)

Update profile info of the authenticated user.

### Input Data
Field name   | Type          | Description
------------ | ------------- | ------------
`first_name` | **Required**  | First name of the user.
`last_name`  | **Required**  | Last name of the user.
`address`	 | **Required**  | Address of the user.
`phone`		 | **Required**	 | Phone number of the user.
`alt_phone`  | **Required**  | Alternative phone number of the user.
`pay_pal`    | **Required**  | Pay pal card details of the user.
`type`		 | **Required**	 | Account type (number): Client - 1, Vendor - 2, Both types - 3
`zip_code`   | **Required**  | Zip code of the user.

### Response example
	{
	  "data": {
	    "address": "Kiev city, Petroskiy avenue, 30", 
	    "alt_phone": "+380987998903", 
	    "first_name": "Vasya", 
	    "last_name": "Vasylenko", 
	    "pay_pal": "4567890893443", 
	    "phone": "+380976778745"
	  }, 
	  "error": null, 
	  "result": true
	}





