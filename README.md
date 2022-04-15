# BlockchainCode

Pre-Requisites
Docker
Installation
Git Clone
https://github.com/abhishekpatwa/BlockchainCode.git

Create .env file at the root directory with following content.
INFURA_TOKEN= < Infura Project Token >
CONTRACT_ADDRESS= < Address of Contract deployed>
OWNER_ADDRESS= < Metamask Account ID >
PRIVATE_KEY= < Private from Metamask Account >

Note:- Kindly replace the above values correctly. For reference refer dotenv file

Creating Docker Image
docker build -t nciabhishekpatwa/blockchaintokendeployment:tagname  .

Run Docker image
docker run nciabhishekpatwa/blockchaintokendeployment:tagname 

Trouble Shooting
Invalid address error.
Kindly make following chnages in distribute.js file.
change .split('\r\n'); to .split('\n'); on line number 19.
