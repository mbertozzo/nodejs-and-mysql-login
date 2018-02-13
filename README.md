# Node.js and MySQL Login

This is a simple signup and/or signin app made with Node.js, Knex and MySQL, done with the purpose to test Node.js ability to interact with MySQL.

## Getting Started

You'll need a machine with Node.js (project tested with v. 8.0.9 and higher) and MySQL. 
Please note that the project uses Knex: in order to work it needs to be installed globally on your machine.

```
npm i knex -g
```

### Database set-up

The database connection details are stored in the *knexfile.js* file: please update the following lines with your credentials.

```
connection: {
    user: 'your_user',
    password: 'your_password',
    database: 'node_database'
  }
```

The *database* value must be the same as the database name you created in your MySQL.

Once ready, run the knex migration to create the table structure: open a terminal in your working folder and launch the command

```
knex migrate:latest
```

## Wrapping up and launching the server

Almost ready!

Just install all the dependencies with 

```
npm install
```

When everything is configured, open a terminal in your working folder and launch

```
node .
```

Your server will be available opening the browser at http://localhost:3000

___

*Thanks to Robert Tod for the tutorial about this code.*
