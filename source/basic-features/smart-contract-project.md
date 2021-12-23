## **Smart Contract Project**

### **Create New Project**

Click *Project* tag to switch to Project Manager. Then click *New* button on the top-right corner to open create project popup. Select whether user wishes to create a local or cloud project, then key in a project name and select the template which will be the base of your project. Ethereum Studio currently offers the following templates:

- **Coin**: A simple coin contract template；
- **ERC20 Token**: An ERC-20 token contract template；
- **[Open Zeppelin] Basics**: A set of templates based on [Open Zeppelin](https://openzeppelin.com/), which includes ERC-20, ERC-721(NFT), ERC-777 and ERC-1155 contract;
- **[Truffle] Metacoin**：Contract templates created by Ethereum Truffle. Ethereum Studio currently does not support deploying Metacoin contracts.

![smart-contract-project-1](smart-contract-project-1.png)

Ethereum Studio supports to create and manage projects out of three common frameworks [Truffle](https://www.trufflesuite.com/truffle), [Hardhat](https://hardhat.org/) and [Waffle](https://ethereum-waffle.readthedocs.io/).

Right now, let's create a new project named `my-project` with Basics template from Open Zeppelin and Truffle framework. Click *Create Project* to start the process.

We'll stick to this project later in this tutorial as we demo a complete cycle of smart contract development.

### **Project Editor**

When the project is successfully created, users will be redirected to Project Editor. Project Editor has a few useful built-in widgets, including file explorer on the left with a toolbar above it, code editor to the right and log viewer in the lower half.

![smart-contract-project-2](smart-contract-project-2.png)

Click the *Project Settings* (gear-shape) icon on the toolbar to open project settings page. Users may view or change project basics, compiler/linter settings, among others.

![smart-contract-project-3](smart-contract-project-3.png)

Ethereum Studio's project editor has a built-in linter, which automatically checks codes and flag for potential warnings or errors. Project editor will indicate an exclamation mark on the line that has warnings and a red cross mark on the line that has errors.

![smart-contract-project-4](smart-contract-project-4.png)

### **Compile smart contracts**

Click *Build* (hammer-shaped) button on the toolbar to start compiling the current project. Users may view progress in the log viewer in the lower half of the editor. Outputs will be stored as `*.json` files in `build/contracts` folder under the current project path. Refer to [solc documentation](https://docs.soliditylang.org/en/latest/using-the-compiler.html#output-description) for more details about compiled outputs.

![smart-contract-project-5](smart-contract-project-5.png)

Users may also trigger compilation of a specific `.sol` contract by a right-click on the file, then select *Compile* from the drop-down menu.

### **Deploy smart contracts**

Click *Deploy* (docker whale) button on the toolbox to open the contract deployment popup. Users may proceed with deployment by filling out all necessary parameters:

- Compiled Contract: The [compiled contract](https://docs.soliditylang.org/en/latest/using-the-compiler.html#output-description) to be deployed in `.json` format. There might be multiple contracts in a single project, choose the proper contract from the drop-down list. Here, we'll be deploying `GLDToken.json` this time;
- Constructor Parameters: Required parameters to construct functions. Ethereum Studio automatically generates parameter form from data structures predefined in the contract, so that users only need to fill the form. Here, click on the initialSupply column and type in 1000;
- Signer: Keypair to sign the deployment transaction. This must be a keypair stored in Keypair Manager. Here, we pick `my-keypair-1` from the drop-down list;
- Gas Limit, Gas Price: Transaction fees for this deployment transaction. Users may leave them blank for Ethereum Studio to estimate on its own or manually override them with your estimates.

Users may also trigger deployment of a specific `.json` output by a right-click on the file, and select *Deploy* from the drop-down menu.

![smart-contract-project-6](smart-contract-project-6.png)

In the above example, the `GLDToken` contract will distribute all 1,000 initial tokens to the signer address `my-keypair-1` upon its receipt of successful deployment. Click *Estimate & Deploy* button, Ethereum Studio will estimate the transaction fee and fill corresponding sections in the form. Hit *Re-estimate* button to redo it. Finally, click the violet *Deploy* button to send the deployment transaction. Sometimes, transaction fees might be underestimated which leads to a failed deployment with insufficient transaction fee error. In that case, manually override with a higher Gas Limit and Gas Price and retry deployment.

Deployment transaction(s) may take some time to be processed by the Ethereum network. Usually, a transaction details popup will show up after 10 - 20 seconds. Users may click on tabs to view Parameters, Tx, Receipt and ABI information of the transaction. This popup can be recalled anytime from [Transaction History](https://github.com/ObsidianLabs/EthereumStudio/blob/master/README.md#Transaction-History).

![smart-contract-project-7](smart-contract-project-7.png)

### **Invoke smart contract**

After the contract is deployed, click the contract address in the Transaction Details popup and user will be redirected to Contract Inspector. Users may also click *Contract* tab to switch to Contract Inspector and type in the address to open a contract. Ethereum Studio's contract inspector allows users to open and debug multiple contracts at the same time.

Contract Inspector is mainly divided into three parts:

- Write methods on the left: Invoke write methods in the contract by selecting from the violet drop-down list;
- Read data in the middle: Read data as predefined data types in the contract by selecting from the violet drop-down list;
- Query event logs on the right: Query event logs as defined in the contract by selecting from the violet drop-down list.

![smart-contract-project-8](smart-contract-project-8.png)

Ethereum Studio automatically stores contract ABI after deployment and generates above lists of write methods, data retrieval, event query and their corresponding parameter forms. For more information on ABI, please refer to [ABI Storage](https://github.com/ObsidianLabs/EthereumStudio/blob/master/README.md#abi-storage).

Now, let's open the `GLDToken` contract we deployed moments ago to demo how to access the contract with Contract Inspector.

First, select *transfer* method from the drop-down list on the left column. *Transfer* method moves a specified amount of tokens from one address to another. We need to populate the parameter form to complete the transaction:

- Select `my-keypair-2` from the drop-down list as the recipient (manual key-in address is also accepted) and type in 100 for amount as we wish to transfer 100 token in this example;
- Leave all forms in the Gas section to Ethereum Studio to estimate.
- Select `my-keypair-1` from the drop-down list in the Signer column. This also designates `my-keypair-1` as the sender in this transaction.

Then click *Execute* (Play) button next to *transfer* to push and execute the transaction. Moments later, Ethereum Network will prompt messages stating transaction status and fee information.

![smart-contract-project-9](smart-contract-project-9.png)

Let's proceed by verifying the outcome of last transaction. Select *balanceOf* from the drop-down list of data types, then select `my-keypair-2` from the drop-down list in the account column. And finally hit *Execute* (Play) button to read the data. The result will be shown below, which in our example, is 100. This verifies that the above transfer transaction of 100 tokens to `my-keypair-2` has been successfully carried out.

![smart-contract-project-10](smart-contract-project-10.png)

Finally, we pick *Transfer* from the drop-down list of contract events and click *Get event logs*(Play) button to query all transfer-related events. Results are shown below in the Event Logs section. Ethereum Studio supports a customized range for events query, but can only return maximum 10,000 queries when connecting to local nodes or testnets, and by default the most recent 10,000 records. Therefore, users should keep the custom range within the aforementioned number. When connecting to Ethereum mainnet, the maximum number of event log queries goes down to 1,000.


