# Welcome to Flight Services
## Project setup
- Clone the project on your local
- Execute `npm install` on the same path as of your root directory of thr downloaded project
- Create a `env file` in the root directory and add the following environment variable
    -PORT `3000`
- Inside the `src/config` folder create a new file `config.json` and then nd the following piece of json

```
{
  "development": {
    "username": "root",
    "password": null,
    "database": "FlightsAndSearch",
    "host": "127.0.0.1",
    "dialect": "mysql"
  }
}

```