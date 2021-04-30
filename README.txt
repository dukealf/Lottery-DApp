Decentralized Lottery App on the Ethereum Blockchain
By: Duke Alf

Overview:
The traditional lottery system is inherently unfair to players. Winnings are lost due to splitting pots, paying taxes, and fraud. This Dapp allows players to join a lottery for the cost of 1 ether. Each address can only enter the lottery once. The winner is randomly selected and receives the entire payout. No middle-man necessary. 

Process:
-the owner of the contract opens the lottery 
-players can enter the lottery by sending one ether
-the ether is pooled together
-the owner closes the lottery and calls a function to randomly select a winner
-the winner, players, and payout is visible to all
-the winning address receives the payout
-the owner can reset the lottery and the process can begin again

Contracts:
There is one Solidity contract called Lottery.sol. This contains all necessary information to successfully conduct the lottery. This can be found in the contracts folder. 

Demo:
I use a Jupyter Notebook to demonstrate functionality. Open the notebook lottery_demo.ipynb and run the cells in order while follwoing the comments. The blockchain I use to deploy and test the contract is eth-tester. This supports the PyEVM backend, which is a full Ethereum implementation in Python. I interact with PyEVM using Web3. Eth-tester will automatically be set to interact with PyEVM.

pip install web3[tester] installs Web3.py, eth-tester, and PyEVM

Sources: 
My references and other notes can be seen at the end of the Jupyter Notebook. 
