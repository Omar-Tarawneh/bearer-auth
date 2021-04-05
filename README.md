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
        "username": "omar",
        "password": "$2b$10$zsfYlAFYH8.8kT6h1heWE.b/QP1xopvf7kNGoiFLiZrKY2rE.enKC",
        "__v": 0
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6Im9tYXIiLCJpYXQiOjE2MTc2MjY5MTZ9.9rDmdWFJ-j6x37tRgLKJP13I7TBgs8bk-jIT3uWCrDo"
  }
  ```

- `/signin`

  - Returns Object

  ```javascript
  {
    "user": {
        "username": "omar",
        "password": "$2b$10$zsfYlAFYH8.8kT6h1heWE.b/QP1xopvf7kNGoiFLiZrKY2rE.enKC",
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6Im9tYXIiLCJpYXQiOjE2MTc2MjY5MTZ9.9rDmdWFJ-j6x37tRgLKJP13I7TBgs8bk-jIT3uWCrDo"
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
