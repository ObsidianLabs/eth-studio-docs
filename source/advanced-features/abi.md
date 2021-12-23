## ABI Storage

When working with Code Inspector, Ethereum Studio relies on contract ABI to generate lists of methods, data types and event types. ABI Storage at the bottom is the place where these ABIs are stored. Upon successful deployment of contract, Ethereum Studio automatically stores contract ABI(s). Users may view the raw ABI data by moving the cursor onto the ABI record and click *Edit* (pencil) icon, or click *Delete* button to remove the ABI record.


![abi-1](abi-1.png)

In case when users need to access other contracts (an online contract, for example), he/she needs to add the contract ABI to ABI Storage. Click *New* button in the ABI Storage popup to start the process. For users' convenience, Ethereum Studio also reads ABI from all compiled contracts in the current project. Click *Select from the current project* and select to import ABI from the drop-down list.


![abi-2](abi-2.png)

### **Transaction History**

Ethereum Studio records every transaction pushed to the network. To view recent transactions, click *Transactions* tab to pull up the list of transactions. Users may single click on a transaction to pull up Transaction Details popup and review information such as Basics, Parameters, Tx and Receipt.




