# [Order](order.md)
## [GET /api/v1/order/get-orders/](order.md#get-apiv1orderget-orders)
Get orders for logged in user
### Input data
Field name   | Type          | Description
------------ | ------------- | ------------
`token`      | **Required**  | User authentication token for Authorization header.

### Query parameters
Field name   | Description
------------ | ---------------
`status`   | Order status (1 - Pending, 2 - Accepted, 3 - Rejected, 4 - Finished).
`page`	 | Page number

### Response example
	{
	  "data": {
	    "orders": [
	      {
	        "created": "Thu, 24 Nov 2016 10:22:59 GMT", 
	        "description": null, 
	        "gig": 3, 
	        "id": 6, 
	        "status": 2, 
	        "vendor": 1
	      }, 
	      {
	        "created": "Thu, 24 Nov 2016 10:22:59 GMT", 
	        "description": null, 
	        "gig": 2, 
	        "id": 3, 
	        "status": 2, 
	        "vendor": 1
	      }
	    ], 
	    "pagination": {
	      "current_page": 1, 
	      "next_page": 2, 
	      "pages": 2, 
	      "prev_page": null
	    }
	  }, 
	  "error": null, 
	  "result": true
	}

## [POST /api/v1/order/create-order/](order.md#post-apiv1ordercreate-order)
Create an order
### Input data
Field name   | Type          | Description
------------ | ------------- | ------------
`token`      | **Required**  | User authentication token for Authorization header.
`description`| **Required**  | Description of work that should be done by vendor.
`status_id`     | **Required**  | Order status (1 - Pending, 2 - Accepted, 3 - Rejected, 4 - Finished).

### Response example
