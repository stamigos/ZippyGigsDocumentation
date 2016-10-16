# [Vendors](vendors.md)
## [GET /api/v1/client/vendors/](vendors.md#get-apiv1clientvendor)
Retrive all vendors
### Input data
Field name   | Type          | Description
------------ | ------------- | ------------
`token`      | **Required**  | User authentication token for Authorization header.

### Query parameters
Field name   | Description
------------ | ---------------
`job_type`   | Vendor's job type (Number).
`status`	 | Vendor status (1 - Available or 2 - Not Available)
`radius`	 | Search radius (in miles)


### Response example
	{
	  "data": [
	    {
	      "address": null, 
	      "alt_phone": null, 
	      "avatar": null, 
	      "avatar_url": null, 
	      "created": "Sun, 16 Oct 2016 18:25:32 GMT", 
	      "email": "test@example.com", 
	      "first_name": "test", 
	      "id": 1, 
	      "is_active": true, 
	      "job_types": [
	        {
	          "id": 1, 
	          "title": "Websites design"
	        }
	      ], 
	      "last_name": "last_name", 
	      "lat": "50.45626", 
	      "lng": "30.47729", 
	      "pay_pal": null, 
	      "phone": null, 
	      "type": 3, 
	      "vendor_description": null, 
	      "vendor_status": null, 
	      "zip_code": "04116"
	    }
	    	...
	    {
	      "address": null, 
	      "alt_phone": null, 
	      "avatar": null, 
	      "avatar_url": null, 
	      "created": "Sun, 16 Oct 2016 18:25:33 GMT", 
	      "email": "test3@example.com", 
	      "first_name": "test3", 
	      "id": 4, 
	      "is_active": true, 
	      "job_types": [
	        {
	          "id": 4, 
	          "title": "Babysitter"
	        }
	      ], 
	      "last_name": "last_name3", 
	      "lat": "50.44590", 
	      "lng": "30.49741", 
	      "pay_pal": null, 
	      "phone": null, 
	      "type": 2, 
	      "vendor_description": null, 
	      "vendor_status": 2, 
	      "zip_code": "01032"
	    }
	  ], 
	  "error": null, 
	  "result": true
	}