# 🚀Challenge 06 - GoStack!

## Quick Start

- Install the dependencies.
- Config the database, through ormconfig.json.
- So type: yarn dev:server

## Backend challenge about Transactions!

The goal was to develop a Node.js backend using TypeScript, with Postegres database and a CSV importing option. Had been used the Docker to create a postgres container. It is a continuation and improviment from the others challenges.

- [x] Develop Database in Postgres;
- [x] Develop migrations;
- [x] Develop Models;
- [x] Develop Repositories;
- [x] Develop Services;
- [x] Develop Routes;
- [x] Pass Routes test;

### Functionalities:

- GET: List all transactions and a balance with the sum of incomes, outcomes, the account total, and the relation of each transaction with their category.

- POST: It creates transactions with a UUID. Requesting title, amount, type (income or result), the category, and not allowing to create any income transaction if the account total is insufficient.

- DELETE: With the transaction id, can delete the transacion.

- POST (/import): Route where a csv file can ben sendo through post and the transactions will be save on database.

### Tests

- [x] Should be able to create a new transaction;
- [x] Should create tags when inserting new transactions;
- [x] Should not create tags when they already exists;
- [x] Should be able to list the transactions;
- [x] Should not be able to create outcome transaction without a valid balance;
- [x] Should be able to delete a transaction;
- [x] Should be able to import transactions;
