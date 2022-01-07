# Contract

In the "Contract" panel, there are three function panels from left to right. Each function panel represents "Write Functions", "View Functions" and "Events" respectively. One can interact with "Write Functions", mainly calling functions with assets. One can check the address status with "View Functions". Besides, one can set parameters and check related events in "Events".

![C-1](/pic/C-1.png)


## Write Functions

### Parameters

In "Parameters", one can set function required parameters. Usually, there are owner, receiver, amount and so on. Please remember that the unit here is "wei".

![C-2](/pic/C-2.png)


### Gas

If one wants to call functions, there would be some gas fee and tip to spend on the miner. Especially when the network is congested, the gas fee can be huge, so one should set a "Max Fee" in case of an unexpectedly high cost. One can click the purple "Estimate" button to get the real-time gas price of this contract on the specific network. If one supposes the gas price is not fair, one can click again, and the Ethereum Studio will change the number too.

![C-3](/pic/C-3.png)

### Authorization

In "Authorization", one can choose "Signer" to pay the gas fee and tip.

![C-4](/pic/C-4.png)

### Results

In "Results", there would be some direct results of the return value of functions. One can check if the function is calling successfully.

![C-5](/pic/C-5.png)



## View Functions

### Parameters


### Results





## Events

### Parameters

### Events Log

In the "Events Log", there is detailed information of events on the contract. For example, in the deployed ERC20 contract, there is an "Approval" and a "Transfer". Click the "Execute" triangle beside the "Approval" button, and one can check the latest event with its block number in the range. There are also event logs on the network.

![C-6](/pic/C-6.png)