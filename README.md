# BlockchainCode

1.	Pre-Requisites  
Docker
 Installation
Git Clone
https://github.com/abhishekpatwa/BlockchainCode.git

2.	Create .env file at the root directory with following content. 
INFURA_TOKEN= < Infura Project Token >
CONTRACT_ADDRESS= < Address of Contract deployed>
OWNER_ADDRESS= < Metamask Account ID >
PRIVATE_KEY= < Private from Metamask Account >

Note:- Kindly replace the above values correctly. For reference refer dotenv file

3.	Creating Docker Image   
docker build -t nciabhishekpatwa/blockchaintokendeployment:tagname  .

4.	Run Docker image  
docker run nciabhishekpatwa/blockchaintokendeployment:tagname 

5.	Trouble Shooting 
Invalid address error.
Kindly make following chnages in distribute.js file.
change .split('\r\n'); to .split('\n'); on line number 19.
