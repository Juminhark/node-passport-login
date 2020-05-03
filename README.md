# node-passport-login

- [`Traversy Media - Node.js With Passport Authentication`](https://www.youtube.com/watch?v=6FOq4cUdH8k&t=92s)

build a complete authentication app with login, register and access control using Node.js, Express, Passport, Mongoose and more.

## Init

```sh
npm init -y
```

## Dependencies

```sh
// dependencies
npm i mongoose dotenv express bcryptjs passport-local ejs express-ejs-layouts connect-flash express-session

// Devdependencies
npm i -D nodemon
```

```ts
// package.json

"main": "app.js",
"scripts": {
    "start": "node app.js",
    "dev": "nodemon app.js"
 }
```

## [bcryptjs](https://www.youtube.com/watch?v=W-ZARauLKc8)

- 암호를 hash함수를 통해 바꿔주는 역활을한다.

- 단방향 hash 함수 : 한쪽으로 바꾸는 건 쉽지만 역방향을 유추하기 힘들다.(암호화)

- user 정보를 admin이 저장할때 암호와 같이 치명적인 정보를 hash함수로 바꾼 정보를 저장.

- user가 admin에게 암호를 요구할경우 admin은 user에게 나머지 정보를 제공받아 user를 확인하고 새로운 암호를 저장하도록 유도.
