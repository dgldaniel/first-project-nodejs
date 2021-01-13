![Logo of the project](https://camo.githubusercontent.com/a869a2aaab296ef925343d7e76518cd213eb0a30/68747470733a2f2f73746f726167652e676f6f676c65617069732e636f6d2f676f6c64656e2d77696e642f626f6f7463616d702d676f737461636b2f6865616465722d6465736166696f732d6e65772e706e67)

# Nodejs Fundamentals

Stores incoming and outgoing financial transactions, which should allow the registration and listing of those transactions.

### Main Tools and concepts

- Typescript
- Express.js
- TypeORM
- Eslint
- Jest

---

## Requirements

For development, you will only need Node.js and a node global package, Yarn, installed in your environement.

### Node

- #### Node installation on Windows

  Just go on [official Node.js website](https://nodejs.org/) and download the installer.
  Also, be sure to have `git` available in your PATH, `npm` might need it (You can find git [here](https://git-scm.com/)).

- #### Node installation on Ubuntu

  You can install nodejs and npm easily with apt install, just run the following commands.

      $ sudo apt install nodejs
      $ sudo apt install npm

- #### Other Operating Systems
  You can find more information about the installation on the [official Node.js website](https://nodejs.org/) and the [official NPM website](https://npmjs.org/).

If the installation was successful, you should be able to run the following command.

    $ node --version
    v8.11.3

    $ npm --version
    6.1.0

If you need to update `npm`, you can make it using `npm`! Cool right? After running the following command, just open again the command line and be happy.

    $ npm install npm -g

###

### Yarn installation

After installing node, this project will need yarn too, so just run the following command.

      $ npm install -g yarn

---

## Install

    $ git clone https://github.com/dgldaniel/first-project-nodejs.git
    $ cd nodejs-fundamentals
    $ yarn

## Running the project

    $ yarn dev:server

[![Run in Insomnia}](https://insomnia.rest/images/run.svg)](https://insomnia.rest/run/?label=First-Project-Nodejs&uri=https%3A%2F%2Fraw.githubusercontent.com%2Fdgldaniel%2Ffirst-project-nodejs%2Fmaster%2Ffirst-project-nodejs-insomnia.json)

**Create a transaction** - **`POST /transactions`**:

Request example:

```json
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

**List transactions** - **`GET /transactions`**

## Running tests

    $ yarn test
