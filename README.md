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
    "username": <YOUR_DB_LOGIN_NAME>,
    "password": <YOUR_DB_PASSWORD>,
    "database": "FlightsAndSearch",
    "host": "127.0.0.1",
    "dialect": "mysql"
  }
}

```
- Once you've added your db config as listed above, go to the src folder from your terminal and execute `npx sequelize db:create`
and execute `npx sequelize db:migrate`
```

## DB design
- Airplane table
- Flight
- Airport
- City

- A flight belongs to an Airplane but one airplane can be used in multiple flights
- A city has many airports but one airport belongs to a city
- One airport can have multiple flights but a flight belongs to one airport
