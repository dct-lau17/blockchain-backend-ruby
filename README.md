## Blockchain Ticketing APP (Back-end)

[![Build Status](https://travis-ci.org/bilfar/blockchain-backend-ruby.svg?branch=master)](https://travis-ci.org/bilfar/blockchain-backend-ruby)
[![Maintainability](https://api.codeclimate.com/v1/badges/f89421f12fd5fbc684ac/maintainability)](https://codeclimate.com/github/bilfar/blockchain-backend-ruby/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/f89421f12fd5fbc684ac/test_coverage)](https://codeclimate.com/github/bilfar/blockchain-backend-ruby/test_coverage)

This repository represents the back-end 'blockchain' element to our project, while the Javascript/React front-end repository [can be found here](https://github.com/dct-lau17/blockchain-ticketing-app-1).

A blockchain-based ticketing app that allows users to purchase concert tickets and stores the validated transactions on a blockchain network. Created as part of our final project for the Makers Academy bootcamp during August 2018.

This repository hosts the back-end blockchain model and a 'miners' page. The back-end creates a new transaction object, and adds the transaction to a list of unverified transactions; then it returns a transaction hash to the user. A Miner can create a new block by hashing the unverified transactions into a new block object and stores it in the blockchain.

[Check out our project log](https://hackmd.io/ZMK-5YXeS6u6zb0THM5F7g)


### Initial MVP
* Project setup ( Trello, Github, Travis CI, Heroku, Simplecov, Linter)
* A simple app that allows a user to see available concert tickets and make a purchase.
* A 'dummy' blockchain built on Ruby that sends ticket transactions to a Postgres database.

### Final product
[**Watch our Ticketchain demonstration video here**](https://vimeo.com/287794015) (turn on Closed-Captions)  
* User can enter details(via frontend application)
* User can select a concert ticket from the songKick API
* A new transaction hash is created in the backend and stored as an unverified transaction
* The transaction can be verified and stored into a block inside a blockchain when a 'Miner' mines a block.
* During the mining process a block is created with a unique hash value based on the previous block's hash and a 'nonce' calculation to replicate the proof of work concept.
* The miner is rewarded a fix sum of 'coins' for mining this block

### User stories for miner and ticket-seller
```
As a miner,
So that I can be rewarded for using my computer processor power,
I want to be able to verify the transactions and store it to the blockchain.
```
```
As a ticket-seller,
So that I can be sure that my transaction is recorded publicly,
I want my transaction to be recorded on a blockchain.
```

## Technologies used
| Technologies Used | Test Suites |
| -------- | ----------------- |
| Ruby, Sinatra     | Rspec, Capybara   |

## To run application

Our Ruby back-end server needs to be run in conjunction with the web front-end. Please download or clone our repository, and navigate to the root directory. The following commands will install project dependencies and host our miner on http://localhost:9292. Transactions that are made on the front-end will appear as an unverified-transaction within the miner, this can be added to the blockchain by clicking mine.

```
> bundle install
> rackup
```

### To run tests
```
> rspec
```

## Learning Outcomes
[can be found here](https://github.com/dct-lau17/blockchain-ticketing-app-1)

## Future/Further Improvements
[can be found here](https://github.com/dct-lau17/blockchain-ticketing-app-1)

## Authors/Credits
* [Ben Luke Smith-Gordon](https://github.com/Ben-893)
* [Daniel Lau](https://github.com/dct-lau17)
* [Fred H](https://github.com/archmagos)
* [Jeff Hung](https://github.com/jeff1108)
* [Nabil Far](https://github.com/bilfar)
