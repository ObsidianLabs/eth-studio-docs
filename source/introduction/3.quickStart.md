# QuickStart
## Login web client

One can log in through two ways. First, click the "Login" icon on the bottom of "not logged in". Second, click the upper right corner and click the "Login" on the panel.

![Qk-1](/pic/Qk-1.png)

In the Ethereum Studio, users can log in through their Github accounts. Once logged, one can automatically log again through Github information. The Ethereum Studio will not keep users' accounts information for sure.

## Create an ERC20 project

After login, one can create the project by clicking the green button with "New".


![Qk-2](/pic/Qk-2.png)


Create an ERC20 project in Ethereum Studio. Let's set the "Project names "tokenTransfer" and the "Template" as "ERC20 Token". The project will be automatically saved in Ethereum Studio's cloud under one's account. Then click the purple button at the bottom left corner to create a project.

![Qk-3](/pic/Qk-3.png)

Then we can see the project is created and the ERC20 contracts have been generated successfully.

![Qk-4](/pic/Qk-4.png)

## Connect to MetaMask Account

We can see a MetaMask wallet popup in the web client to log in through users' passwords. Suppose one does not have a MetaMask account. Please refer to the **Link (**[https://metamask.zendesk.com/hc/en-us](https://metamask.zendesk.com/hc/en-us)**)**.


![Qk-5](/pic/Qk-5.png)

After linking to the MetaMask, one must copy the mnemonic into the Keypair Manager **for later deploying contracts.** By clicking the purple key icon on the bottom left corner, one can click the "Import" button and paste the mnemonic words, 12 English Words representing the private key. Finally, give this imported private key a name, and the Etereum Studio will save it under this account in the cloud.

## Request Ropsten Faucet

After choosing the "Network" and "Explorer", one can click the upper right "Faucet" icon and get the request page of testETH on the testnet. Let's choose Ropsten testnet and click the icon to turn to the request page in this example.


![Qk-6](/pic/Qk-6.png)

Click the upper right "Faucet" icon, and the page will jump to the Ropsten Faucet. One can copy the wallet address in MetaMask and paste it into the box. Then one clicks the button "Send me test Ether" and wait for a few minutes.


![Qk-7](/pic/Qk-7.png)

With all the requests finished, there will be 5 testETH in the wallet address on Ropsten test Network.


![Qk-8](/pic/Qk-8.png)

Back to the web client, one can also check that there is 5ETH on the selected test network, Ropsten.


![Qk-9](/pic/Qk-9.png)

## Build Contracts

One has three Solidity files in the "ERC20/contracts/" file in the left panel after successfully creating the project. One can select the contract and click the "Hammer" icon to build the contract.


![Qk-10](/pic/Qk-10.png)

Now the IDE only supports compiling all the contracts together. The single-file compilation will come soon in the later version.

![Qk-11](/pic/Qk-11.png)


## Deploy Contracts

After a successful compilation, one can deploy the ERC20 contract on the Ropsten testnet. Select the JSON file "ERC20.json".

![Qk-12](/pic/Qk-12.png)

Then set "name_" as "test", "symbol_" as "TEST" and totalSupply as "3000000000".

![Qk-13](/pic/Qk-13.png)

The signer can be selected as the keypair saved in Keypair Manager. If there is no choice, please check the **Link**.

![Qk-14](/pic/Qk-14.png)

One can set the "Tip" as one's own will, or it can be generated with "Gas Limit" and "Max Fee" together. Then click the bottom right button to "Estimate" the "Gas Limit", "Tip", and "Max Fee". There will be the estimated Gas Fee in real-time. If one supposes the Gas Fee is not reasonable, click the "Re-estimate".

![Qk-15](/pic/Qk-15.png)

After deploying successfully, there is a window with detailed transaction information. Now the contract is deployed at the address: 0xF30438E789b361Eca03B3C7AB8cB176e436C7259 and one can click the address to turn to the "Contract" interface.

![Qk-16](/pic/Qk-16.png)

## Check Balance and Transfer

Since one has 5 testETH prepared for "Gas Fee", one can choose the "transfer" function from the purple inverted triangle icon. Now, select the "recipient" as the target address and set the token amount to transfer as 1000. Then one can click the purple "Estimate" button to set "Parameters" and "Gas" automatically.

![Qk-17](/pic/Qk-17.png)

After all the parameters are settled, one can click the triangle icon beside "transfer" to execute a function.

![Qk-18](/pic/Qk-18.png)

After the "PUSHING" state, the contract is deployed successfully with the "CONFIRMED" state. If one wants to see the past transaction detail, select "Explorer" on the upper right panel.

![Qk-19](/pic/Qk-19.png)

After transferring the 1000 "TEST" token, one can click the upper right "Explorer" to see the balance of 4.997 testETH now. Since one has deployed and called a contract, the balance consumed by the "Gas Fee" and "Tip" will not be 5 testETH anymore.

![Qk-20](/pic/Qk-20.png)

Here is the most simple quickstart example of the Ethereum Studio. Please feel free to ask us any questions through **Link (**[https://github.com/ObsidianLabs/EthereumStudio/issues/new](https://github.com/ObsidianLabs/EthereumStudio/issues/new)**)**.