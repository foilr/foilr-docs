**Log Exception**
----
  Returns information about the created exception.

* **URL**

  `/exception`

* **Method:**

  `POST`
  
*  **URL Params**

   **Required:**
 
   `key=[api key]`

* **Data Params**

  **Required:**

  `exceptionType=[string]`

  **Optional:**

  `url=[string]`

  `statusCode=[integer]`

  `file=[string]`

  `lineNumber=[integer]`

  `message=[string]`

  `stacktrace=[string]`

  `username=[string]`

  `ipaddress=[string]`

  `useragent=[string]`

  `server=[string]`

  `additional=[string]`

* **Success Response:**

  * **Status Code:** `200 OK` <br />
    **Content:** `{ id: 1 }`
 
* **Error Response:**

  * **Status Code:** `401 Unauthorized` <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`

* **Sample Call:**

  ```
    curl https://api.foilr.com/exception \
     -u APIKEY: \
     -d "exceptionType=server" \
     -d "url=example.com/test"
  ```