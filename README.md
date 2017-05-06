# From this branch forward, we will be building our Reddit application.
### In this lesson, we will be building the backend API. While this is not strictly necessary (since Reddit provides its own open JSON API), this will allow us to demonstrate the relevant principles of express and Node, while avoiding the usage and creation of a far more complex backend.

### Let's get started with packages, servers and Express.
```
npm i --save-dev express nodemon
```

Nodemon is a package that allows you to watch your project for changes, and it will automagically reload for you. Since we will be editing frequently, killing and restarting your server again and again will get very old, very fast.

### You will also need some helper modules:
```
npm i --save-dev body-parser cookie-parser multer http-status-codes
```

### Create your simplest server.
Start with the server in `src/index.js`, which builds on the project we built in the first session.


### Exercise:
Build a server API that does the following:
- Accepts a GET request on the '/' index route, and returns the Reddit JSON for that same route.
- Generalize this function so that it can retrieve the JSON for any reddit path
  - Reddit paths are /, r/<subreddit>
  - Each one can also have top, new, hot
