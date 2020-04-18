# simple-crud-go-postgres

BaseUrl: http://localhost:8080

## **Create New User**
Return json of new user

-   **URL**

    /api/newuser

-   **Method:**

    `POST`

-   **URL Params**

    None

-   **Data Params**

      **Required:**

      `name=[string]`\
      `age=[integer]`\
      `location=[string]`\

-   **Success Response:**

    -   **Code:** 201 <br />
        **Content:**
        ```json
        {"id":2,"message":"User created successfully"}
        ```


## **Get All Users**
Return array of users object

-   **URL**

    /api/newuser

-   **Method:**

    `GET`

-   **Success Response:**

    -   **Code:** 200 <br />
        **Content:**
        ```
        [{"id":1,"name":"Edycakra","location":"Bandung","age":29},{"id":3,"name":"dUMMY","location":"Jakarta","age":0}]
        ```

## **Get One User**
Return json of one user

-   **URL**

    /api/user/:id

-   **Method:**

    `GET`

-   **URL Params**

    **Required:**

    `id=[integer]`

-   **Success Response:**

    -   **Code:** 200 <br />
        **Content:**
        ```json
        {"id":1,"name":"Edycakra","location":"Jakarta","age":28}
        ```

## **Update One User**
Return json of update status

-   **URL**

    /api/newuser/:id

-   **Method:**

    `PUT`

-   **URL Params**

    **Required:**

    `id=[integer]`

-   **Data Params**

      **Required:**

      `name=[string]`\
      `age=[integer]`\
      `location=[string]`\

-   **Success Response:**

    -   **Code:** 200 <br />
        **Content:**
        ```json
        {"id":2,"message":"User updated successfully. Total rows/record affected 1"}
        ```

## **Delete One User**
Return json of delete status

-   **URL**

    /api/newuser/:id

-   **Method:**

    `DELETE`

-   **URL Params**

    **Required:**

    `id=[integer]`

-   **Data Params**

      **Required:**

      `name=[string]`\
      `age=[integer]`\
      `location=[string]`\

-   **Success Response:**

    -   **Code:** 200 <br />
        **Content:**
        ```json
        {"id":2,"message":"User updated successfully. Total rows/record affected 1"}
        ```