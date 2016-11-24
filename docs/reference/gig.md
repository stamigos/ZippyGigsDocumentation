# [Gig](gig.md)
## [POST /api/v1/gig/](gig.md#post-apiv1gig)
Create gig
### Input data
Field name   | Type          | Description
------------ | ------------- | ------------
`token`      | **Required**  | User authentication token for Authorization header.
`type`       | **Required**  | Job type field
`description`| **Required**  | Description of gig
`price`      | **Required**  | Hourly rate
`account`    | **Required**  | Client account - gig creator
`vendor_id`  | Optional      | If set - gig related to particular vendor, if not set - to different vendors


### Response example
