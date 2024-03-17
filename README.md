# this is an updated version of:
https://github.com/TigerAtGit/VDapp_MiniProject.git
up to date (mars 2024)
- latest tls of node !
- this project will work in LOCAL envirement (using localhost) !

# it uses:
- Truffle
- Ganache
- Metamask
- Solidity
- Web3 JS
- React JS

# changes ?
- "commented"-out any references to infura.
- most uses of "img" has been left empty (src="") because those needs a database to store and call the images from.
- some files arn't being used (probably only "serviceWorker.js").
- updated the package.json dependencies.
- updated react components and removed all deprecated code.

# my opinion:
- the code work. youre welcome.
- there is/was a file named 'yarn.lock' and i don't know what it's being used for...
- the .env was holding this line 'SKIP_PREFLIGHT_CHECK=true', not sure if its necessary...

# commands used in this project:
```
npm i truffle -g
cd .\client\
npm i
cd ..
truffle compile
truffle migrate
cd .\client\
npm run start
```

# apps that needs installation:
- ganache
- metamask (i used the extension)

# guide ?
- in vscode, the extension "Truffle for VS Code v2.7.1" isn't going to work properly because it isn't up to date with node.js and npm. installing may help, just don't depend on it.
- used solc version "0.8.19" because anything later gave errors.
- ganache needs to be open and the project selected (ganache will look for 'truffle-config.js').
- add the ganache network inside metamask so the accounts that are going to be used when imported, will show 100eth each.
- the address for an admin is written inside the .sol file, so make sure it is changed to whatever address you're going to choose from ganache.
- the code is probably not "secure" enough.
- if you're going to install ganache from npm, make sure to install ganache and not ganache-cli(it's outdated).






### old README:

# VDapp (Decentralised Application for Voting)
It is an E-voting system using Blockchain. 

## Demo
https://user-images.githubusercontent.com/77017010/170699771-7d6a0109-a8f1-4db8-b122-0ae713db2596.mp4

## Need of Blockchain
Using blockchain, voting process can be made more secure, transparent, immutable, and reliable. A blockchain-based voting application does not concern itself with the security of its Internet connection, because any hacker with access to the terminal will not be able to affect other nodes. Voters can effectively submit their vote without revealing their identity or political preferences to the public. Officials can count votes with absolute certainty, knowing that each ID can be attributed to one vote, no fakes can be created, and that tampering is impossible.

## What we have developed?
A Decentralized Application (Dapp) running on the Ethereum blockchain and client side as a React JS application.
All the contract code is written in solidity language which is used to deploy contract in blockchain platform.
This application can be used by Election Commission (officials responsible for conducting Elections) as well as Voters. 
- The officials can control the election process by
  - Verifying the eligible voters
  - Adding the list of candidates that are standing for the election
  - Start or End voting phase (time during which the voters can cast their vote)
  - See or display the results of election.
- The voters can participate in the election process by
  - Registering themselves for the voting
  - Viewing the list of candidates
  - Casting their vote

### What we have used?
- Truffle
- Ganache
- Metamask
- Solidity
- Web3 JS
- React JS
