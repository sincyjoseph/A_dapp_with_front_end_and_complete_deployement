# A_dapp_with_front_end_and_complete_deployement


Steps:

1. download the folder dapp

2. open the folder in Visual studio code.

3. take the terminal and run the command => npm install

4. This will install all the dependencies(Here we use web3.js version 0.19.0 so use >>npm install web3@0.19.0 --save)

5. take another terminal and run this command => testrpc

6. install live server using VS code extension

7. run the smart contract in remix ide

8. Create your front end using html/css(To create a skeleton html file in vscode type ! and tab, here the folder contain the index.html file already)

9. copy the ABI of your contract from remix to inside your index.html file
                       
                       //Something similar to this code
                        [
                          {
                            "constant": false,
                            "inputs": [
                              {
                                "name": "_fName",
                                "type": "string"
                              },
                              {
                                "name": "_age",
                                "type": "uint256"
                              }
                            ],
                            "name": "setInstructor",
                            "outputs": [],
                            "payable": false,
                            "stateMutability": "nonpayable",
                            "type": "function"
                          },
                          {
                            "constant": true,
                            "inputs": [],
                            "name": "getInstructor",
                            "outputs": [
                              {
                                "name": "",
                                "type": "string"
                              },
                              {
                                "name": "",
                                "type": "uint256"
                              }
                            ],
                            "payable": false,
                            "stateMutability": "view",
                            "type": "function"
                          }
                        ]

10. copy the deployed contract address from remix ide and paste it in index.html

        var Coursetro = CoursetroContract.at('0x00fb966d6a31240661F7EF38d88298861BB5dB72');  //Deployed contract address from remix

11.Save all the file.

12.Open another terminal and run

          ganache-cli -p 8545       //if you are using the ganache-cli as your testnetwork, your HttpProvider: http://localhost:8545, http://localhost:8545 may vary depend on your network)
          
13. right click the index.html and run using live server.





