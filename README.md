# TodoList-Solidity-
Solidity Remix Ganache-GUI Truffle


### installing truffle <br>
npm install -g truffle@5.0.2

### create new truffle project <br>
truffle init

### create package.json file to install some dev dependencies <br>
npm install touch-cli -g <br>
touch package.json <br>
reference the content of the file "package.json"

### create TodoList.sol

### compile
truffle compile

### update the configration file(truffle-config.js) and connect to personal blockchain network(ganache)

 development: { <br>
     host: "127.0.0.1",     // Localhost (default: none) <br>
     port: 7545,            // Standard Ethereum port (default: none) <br>
     network_id: "5777",       // Any network (default: none) <br>
    }, <br>

 truffle migrate

 ### open truffle console

 truffle console

 ### get the instance of the deployed smart contract
 todoList = await TodoList.deployed()

 ### get the address of the deployed smart contract
 todoList.address

 ### get the taskCount of the todoList
 todoList.taskCount()

 ### or 
 taskCount = TodoList.taskCount()
 taskCount.toNumber()

 ### truffle migrate reset 
 truffle migrate --reset <br>

 todoList = await TodoList.deployed() <br>
 task = await todoList.tasks(1)  <br>
 task.content   <br>

 ### develop frontend

bs-config.json  <br> 
src/index.html  <br>
src/app.js      <br>

### run the client
npm run dev

