**Log Event**
----
  Returns information about the created event.

* **URL**

  `/event`

* **Method:**

  `POST`
  
*  **URL Params**

   **Required:**
 
   `key=[api key]`

* **Data Params**

  **Required:**

  `name=[string]`

  **Optional:**

  `description=[string]`

  `additional=[string]`

* **Success Response:**

  * **Status Code:** `200 OK` <br />
    **Content:** `{ id: 1 }`
 
* **Error Response:**

  * **Status Code:** `401 Unauthorized` <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`

* **Sample Call:**

  ```
    curl https://api.foilr.com/event \
     -u APIKEY: \
     -d "name=begin deploy" \
     -d "description=Starting deploy"
  ```