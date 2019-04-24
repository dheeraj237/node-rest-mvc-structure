# node-rest-mvc-structure
Scalable REST API using the nodejs, express.js and MongoDB Using famous MVC Structure.

### Directory Structure
```
├── configs
│   ├── app.js
│   ├── config
│   │   ├── config.js
│   │   └── local.js
│   └── db.js
├── controllers
│   └── apis
│       └── user.js
├── models
│   └── user.js
├── package.json
├── package-lock.json
├── routes
│   ├── apis
│   │   ├── index.js
│   │   └── v1.js
│   └── index.js
├── server.js
└── services
    └── users
        └── user.js

9 directories, 13 files
```

### Testing
  install REST CLient Extension in VS COde and use `test.rest` file for testing REST Endpoint in IDE itself. please refer to [this](https://github.com/Huachao/vscode-restclient/blob/master/README.md)
  
### Customizations
  The db.js file is a simple js file which contains our MongoDB URL and a secret key and then exporting it so that we can use it in others file. 
  You will see that in the above file we are requiring the env file which is dependent on the environment like local, testing, staging or production. For a large application, It is always a good practice to keep keys based on the environment type. For this tutorial, we have a local file which you can modify according to your need.
  
  `local.js` file inside the config folder which export hostname and port inside the localConfig object.
