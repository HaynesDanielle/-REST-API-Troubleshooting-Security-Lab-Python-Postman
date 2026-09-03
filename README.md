# -REST-API-Troubleshooting-Security-Lab-Python-Postman
Identify and troubleshoot an API request that fails due to invalid authentication credentials.  
# Exercise: Invalid Authentication

## Objective

Identify and troubleshoot an API request that fails due to invalid authentication credentials.

## Request

```http
GET /users
{
  "error": "Unauthorized"
}
WARNING Unauthorized request to /users
<API_KEY>
HTTP 200 OK
