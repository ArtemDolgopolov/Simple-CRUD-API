# Setup and Running

- `20 LTS` version of Node.js is preferable.
- Clone this repo:

    ```bash
    git clone https://github.com/ArtemDolgopolov/Simple-CRUD-API.git
    ```

- Switch to the develop branch:

   ```bash
    git checkout develop
    ```

- Move to folder:

    ```bash
    cd Simple-CRUD-API
    ```

- Install dependencies:

    ```bash
    npm install
    ```

- Create file `.env` with `PORT = number` excepting 3000.
- Start server:

    To run server in development mode:

    ```bash
    npm run start:dev
    ```

    To run server in production mode:

    ```bash
    npm run start:prod
    ```

    Also there are to commands to run server in horizontal scaling modes:

    ```bash
    npm run start:multi:dev
    ```

    or 

    ```bash
    npm run start:multi:prod
    ```

- Now you can send requests to the address: `http://localhost:{PORT}` (depending on port number).

- Command to start tests (app should run during testing!!!):

    ```bash
    npm run test
    ```

## API instructions

- **Get Users**

    Returns json data about users.

  - **URL**

    /api/users

  - **Method:**

    `GET`

----

- **Get User**

    Returns json data about selected user.

  - **URL**

    /api/users/{userId}

  - **Method:**

    `GET`

----

- **Create User**

    Creates a new user.

  - **URL**

    /api/users

    Example (for postman):

    ```
    {
      "username": "example_user",
      "age": 30,
      "hobbies": ["reading", "coding"]
    }
    ```

  - **Method:**

    `POST`

----

- **Update User**

    Updates selected user.

  - **URL**

    /api/users/{userId}

  - **Method:**

    `PUT`

----

- **Delete User**

    Deletes selected user.

  - **URL**

    /api/users/{userId}

  - **Method:**

    `DELETE`

----