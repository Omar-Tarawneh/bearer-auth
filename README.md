# bearer-auth

## Features & Notes

- Addetional layers of Encyption
- Tokens will be expired after 1 hour

## Deployment test And URLS

- Heroku main branch
  [oht-basic-auth](https://oht-bearer-auth.herokuapp.com/)

- Github Pull Request
  [Pull-Request](https://github.com/Omar-Tarawneh/bearer-auth/pull/1)

- Action
  [Action](https://github.com/Omar-Tarawneh/bearer-auth/actions)

## Setup

`.env`

- `PORT`: PORT NUMBER

- `MONGODB_URI`: `mongodb+srv://omar:0000@cluster0.vibfe.mongodb.net/myFirstDatabase?retryWrites=true&w=majority`

## Running the app

- `npm satrt`

- Endpoints:
- `/singup`

  - Returns Object

  ```javascript
  {
    "user": {
        "_id": "606b071ec90c2e0e29783059",
        "username": "omar"
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6Im9tYXIiLCJpYXQiOjE2MTc2MzMwMDcsImV4cCI6MTYxNzYzNjYwN30.diDiCIwjPTlECh-3rUpJUlhKBa-VP4zKLoLaT9AvJ_k"
  }
  ```

- `/signin`

  - Returns Object

  ```javascript
  {
    "user": {
        "_id": "606b071ec90c2e0e29783059",
        "username": "omar"
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6Im9tYXIiLCJpYXQiOjE2MTc2MzMwMDcsImV4cCI6MTYxNzYzNjYwN30.diDiCIwjPTlECh-3rUpJUlhKBa-VP4zKLoLaT9AvJ_k"
  }
  ```

- `/users`

  - Returns Object

    ```javascript
    ['omar', 'jack', 'ahmad'];
    ```

- `/sercret`

  - Returns Object

    `Welcome to the secret area!`

## Tests

- `npm test`

## UML

![uml](./img/Lab06.png)
