# Network

## Development

When building an Ethereum application with smart contracts, users will want to run it on a local network to see how it works before deploying it. Similar to how you create a local server on your computer for web development, you can create a local blockchain instance to test your app. This network allows for much faster iteration than a public testnet(for instance, you don't need to acquire ETH from a testnet faucet).

### Geth Version Manager

Click "Geth Version Manager" to set a specific version of Geth. Before login, one had installed the Docker image of Geth, so there is a default version.

![Nw-1](Nw-1.png)

One can install a Geth version different to the default version as development requires.

![Nw-2](Nw-2.png)

Geth is installed through Docker image. One has to start Docker before installing.

![Nw-3](Nw-3.png)

After installing Geth, one can check the created version in "Geth Version Manager". There will be a blue number icon beside the "Geth Version Manager" button indicating how many versions are in the manager.

If one wants to remove the installed Geth, double-click the "trash can" icon. After the first click, the icon will turn red, and one can click it again to delete Geth.

![Nw-4](Nw-4.png)

### New Instance

Click "New Instance", there will popup a "New Instance (dev)" window.

![Nw-5](Nw-5.png)

One can set "Instance name" in the window and change the Geth version if there are different versions. Besides, one can also set "Miner" as the target account. Then click the "Create" button on the bottom right to get an instance.

![Nw-6](Nw-6.png)

After successfully creating a new instance with the target Geth version, the instance will be on the panel. Click "Start" to run the development network. One can create an etheruem network and connect to it. This ethereum network requires no test ETH.

![Nw-7](Nw-7.png)

### Node Panel

Click the green "Start" button on the instance will start it. Information will run on the node panel, and the development network is prepared. One can deploy a contract instantly and cost nothing in the development network, so it is easy and friendly to test smart contracts on the private network. You can try it!

![Nw-8](Nw-8.png)


## Ethereum Mainnet and Testnet

### Mainnet

A mainnet is an independent blockchain running its network with its technology and protocol. It is a live blockchain where its cryptocurrencies or tokens are in use, compared to a testnet or projects running on top of other popular networks such as Ethereum.

 

Ethereum Mainnet is the primary public Ethereum production blockchain, where actual-value transactions occur on the distributed ledger. Ethereum mainnet uses real ETH as currency to transfer assets and pay gas fees and tips. There are many different Ethereum testnets, and each testnet uses its own test ETH as currency, respectively. One may deploy and test contracts on at least one testnet before the final release on the mainnet.

 

### Testnets

In addition to Mainnet, there are public testnets. These are networks used by protocol developers or smart contract developers to test both protocol upgrades and potential smart contracts in a production-like environment before deployment to Mainnet. Think of this as an analog to production versus staging servers.

 

It's generally essential to test any contract code you write on a testnet before deploying to the Mainnet. Suppose you're building a dapp that integrates with existing smart contracts. In that case, most projects have copies deployed to testnets that you can interact with it.

 

Most testnets use a proof-of-authority consensus mechanism. This means a small number of nodes are chosen to validate transactions and create new blocks – staking their identity in the process. It's hard to incentivize mining on a proof-of-work testnet which can leave it vulnerable.

 

#### Ropsten

A proof-of-work testnet for those running Geth, Besu and all other Ethereum clients. This means it's the best like-for-like representation of Ethereum. Ropsten started in November 2016 and it can be used with all clients.

 

#### Rinkeby

A proof-of-authority(clique) testnet for those running Geth, Besu, Nethermind, and OpenEthereum client. Rinkeby started in April 2017 and is immune to spam attacks (as Trusted parties control ether supply).

 

#### Gorli

A proof-of-authority testnet that works across clients. Gorli started in November 2018. Gorli doesn't fully reproduce the current production environment as it uses PoA.

 

#### Kovan

A proof-of-authority testnet for those running OpenEthereum clients. Kovan started in March 2017 and is immune to spam attacks. Kovan doesn't fully reproduce the current production environment as it uses PoA.

 

## Custom Network

In the Ethereum network, there are private networks and public networks. The Ethereum Studio can set "Custom Network" to connect the target network. Connecting to a network, one can join the network of other nodes instead of establishing a network by oneself. Especially, one can use a company's network service like Infura **Link(**[https://infura.io/docs](https://infura.io/docs)**)**.


![Nw-9](Nw-9.png)


### New Connection

In the "Custom Network" panel, click the "gear" icon, and there will popup a window named "Custom Network".

![Nw-10](Nw-10.png)

Click the "New Connection" button, and there will jump out a window for one to add more network connections. Since each connection represents a node from one of the public or private networks, there will usually be a lot of different connections for one to connect.

![Nw-11](Nw-10.png)

In the "New Custom Network Connection" window, one can input the name and URL of node RPC. In this picture, there is a node of Ropsten network from Infura. Infura is a Web3 backend and Infrastructure-as-a-Service (IaaS) provider that offers blockchain developers a range of services and tools. One can use Infura as a fundamental infrastructure of Ethereum projects. Besides, one can join other Geth nodes with the node parameters.

![Nw-12](Nw-12.png)

After clicking "Check Network," a "Network info" will be added below the original panel. The panel shows detailed network information to be joined with "URL of node RPC". One can check the information and join the network by clicking the "Add Network" button.

![Nw-13](Nw-13.png)

After adding a network, click the green "Connect" button, and there will be a "Blocks" panel showing the "Block Number", "Block Time", and "Difficulty" in real-time.

![Nw-14](Nw-14.png)

![Nw-15](Nw-15.png)
