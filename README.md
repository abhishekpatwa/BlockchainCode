# BlockchainCode

1.	Pre-Requisites  <br/>
Docker
 Installation 
Git Clone
https://github.com/abhishekpatwa/BlockchainCode.git

2.	Create .env file at the root directory with following content. <br/>  
INFURA_TOKEN= < Infura Project Token >   <br/>
CONTRACT_ADDRESS= < Address of Contract deployed>   <br/>
OWNER_ADDRESS= < Metamask Account ID >  <br/> 
PRIVATE_KEY= < Private from Metamask Account > <br/>

Note:- Kindly replace the above values correctly. For reference refer dotenv file <br/>

3.	Creating Docker Image <br/>
docker build -t nciabhishekpatwa/blockchaintokendeployment:tagname  .

4.	Run Docker image <br/>
docker run nciabhishekpatwa/blockchaintokendeployment:tagname 

5.	Trouble Shooting <br/>
Invalid address error.
Kindly make following chnages in distribute.js file.
change .split('\r\n'); to .split('\n'); on line number 19.
