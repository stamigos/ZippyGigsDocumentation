# [Client](vendors.md)
## [POST /api/v1/client/avatar/](client.md#post-apiv1clientimage)
Upload an avatar for authenticated user
### Input data
Field name   | Type          | Description
------------ | ------------- | ------------
`avatar`     | **Required**  | base64 encoded image file
`token`      | **Required**  | User authentication token for Authorization header.

### Response example
	{ 
	  "data": 
	    {
		   "url": "http://{domain}/api/v1/client/media/image.png"
		},
	  "error": null, 
	  "result": true
	}

## [GET /api/v1/client/job-types/](client.md#post-apiv1clientimage)
Get list of job types
### Input data
Field name   | Type          | Description
------------ | ------------- | ------------
`token`      | **Required**  | User authentication token for Authorization header.

### Response example
	{
	  "data": {
	    "job_types": [
	      {
	        "id": 1, 
	        "title": "Websites design"
	      }, 
	      {
	        "id": 2, 
	        "title": "Marketing"
	      }, 
	      {
	        "id": 3, 
	        "title": "Plumbing"
	      },

	      	...

	    ]
	  }, 
	  "error": null, 
	  "result": true
	}