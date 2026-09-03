# -REST-API-Troubleshooting-Security-Lab-Python-Postman
Identify and troubleshoot an API request that fails due to invalid authentication credentials.  
# Exercise: Invalid Authentication

## Objective

Identify and troubleshoot an API request that fails due to invalid authentication credentials.

## Request

```http
GET /users
Problem
The request was made using an incorrect API key in the X-API-Key header.

HTTP Response
Status: 401 Unauthorized
{
  "error": "Unauthorized"
}
Log Evidence
WARNING Unauthorized request to /users
Root Cause
The API key supplied in the X-API-Key header was invalid.

Resolution
Replace the invalid API key with the correct API key:
<API_KEY>
Successful Result
After supplying the correct API key, the request succeeded with:
HTTP 200 OK
The API returned the expected users JSON response.

Summary
The 401 Unauthorized response was caused by an invalid API key. Updating the X-API-Key header with the correct credential resolved the authentication failure. I identified the authentication failure from the 401 status, confirmed the cause using the server log, determined that the X-API-Key was invalid, corrected the credential, and verified the fix with a successful 200 response.
