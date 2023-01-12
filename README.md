# Stateless Smart Contract Demo
This repository contains sample codes to compile a stateless smart contract into a contract account or delegated signature without using Algo Builder.

## Setup instructions

### Install packages
```
yarn install
```

### Update environement variables
1. Copy `.env.example` to `.env`.
2. Update Algorand Sandbox credentials in `.env` file.
3. Run `source .env` in the project directory

### Update receiver address
In `stateless_sc.py`, update receiver's address to `ACC2_ADDR`'s in the env file

### Compile contract
```
make stateless_sc
```

### Stateless smart contract to contract account
```
node js/contract_account.js
```

### Stateless smart contract to delegated signature
```
node js/delegate.js
```