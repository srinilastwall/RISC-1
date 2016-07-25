![Lastwall Logo](lw-logo.jpg) 


# Integration Steps


## Add script to your login page


## Add API key



## Add Authorisation Token




## API Return Values

All Lastwall API calls will return one of the following status codes:

- **200** - OK: the API call was successful
- **400** - Error: the API call failed due to invalid input or caller error
- **401** - Authorization Error: the API call failed due to an API key authentication failure
- **500** - Fatal: the API call failed due to an internal Lastwall system error (not your fault)

For all successful API calls (code 200), the relevant response data will be returned as JSON in the message body. If there is no data to return, the result will be:

`{ "status": "OK" }`

For all failed API calls (codes 400, 401, or 500), the result will be:

`{ "status": "Error", "error": "(specific error message)" }`


