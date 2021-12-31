# Install Desktop Client

## Download

Download Ethereum Studio installation package in Github Ethereum Studio Latest Release([https://github.com/ObsidianLabs/EthereumStudio/releases](https://github.com/ObsidianLabs/EthereumStudio/releases)) according to the computer system type ( .dmg for macOS, .AppImage for Linux, .exe for Windows ).

 

## Install Dependencies

Starting Ethereum Studio requires several image dependencies, including Docker, Ethereum Node and Ethereum Truffle. All three docker files are necessary to run the Ehereum Studio desktop clients. The modules are installed in docker client like this:

 

 

If there is any missing dependency in Docker, one can install it through the "Welcome" page. One can install the available versions in the "Geth in Docker" list. It is the same for "Truffle in Docker", too.

 

 

 

After all the dependencies are installed, one can click the "Get Started", and the Project interface will be there. 

 

 

 

### Docker

[Docker](https://www.docker.com/) is used to start the Ethereum Node and building projects in Ethereum Studio. If Docker is not installed yet, users can click the *Install Docker* button to visit the official Docker website and download and install it.

 

Docker can not wake up automatically through the Ethereum Studio desktop client. One has to open Docker before starting the desktop client. Otherwise, an error report would remind "Docker has not been installed".

 

### Geth

[Geth in Docker](https://github.com/ethereum/go-ethereum) is the Ethereum node image. Ethereum Studio uses the image to run the Ethereum node and build projects. One can install the Geth image through the "Install" button and select the required version. The latest version is always recommended as the beginner's default version.

 

### Truffle

[Truffle in Docker](https://github.com/trufflesuite/truffle) is an Ethereum version of Truffle used to create and build projects. One can install the Truffle image through the "Install" button and select the required version. The latest version is always recommended as the beginner's default version.

 

When all the dependencies are correctly installed, the grey *Skip* button will change into a violet *Get Started* button. Click the button to enter the main interface of Ethereum Studio.

 
## Contrast with Web Client

### Create a New Project

It is a bit different in creating an ERC20 project in the Ethereum Studio Desktop client. The "Project name" is "testTransfer" and the "Project location" is automatically settled as "C:\Users\Administrator\Ethereum Studio\testTransfer" in the Windows system. The "Project location" must be empty documentation. On the web client will save projects automatically in the cloud.

 

 

In the Ethereum Studio desktop client, one can set "Template" as "Basics - ERC20, ERC721 & ERC 1155" to save time importing basic projects in the later development process. Besides, there is Truffle framework "Metacoin" to choose from while in the web client, there are only three types to choose from -- "Empty Project", "Coin", and "ERC20 Token". The "Open Zeppelin Version" is the latest automatically, and one can select other versions.

 

 

In the Ethereum Studio desktop client, one can select three different frameworks as the development environment. The frameworks to be chosen are "Truffle", "Hardhat", "Waffle", and "Dockerized Truffle". Besides, there are also three types of "Npm client", which are "npm", "yarn", and "cnpm" while one can not choose in the web client.

 

Those frameworks and tools will be automatically used in the command line when one tries to build or deploy projects. The default framework version is the same asset during the install process of Docker, and it will be introduced later.

 

### Build contracts

In the Ethereum Studio desktop client, one can build a Solidity file through "Right Click", the file name. In contrast, one can only build in the web client by clicking the "hammer" icon.

 

 

 

### Keypair Manager with MetaMask

In the Ethereum Studio web client, one can automatically wake up the Browser extension of MetaMask. After logging in to the MetaMask account, the Explorer will be linked to the account. One can check the detailed information about it. But one still needs to import the mnemonic in the Keypair Manager to use it in the later deploying. 

In the Ethereum Studio desktop client, one can only import a MetaMask account through mnemonic in Keypair Manager. The browser extension is invalid in the desktop client.

 

### Development and Custom Network

In the Ethereum Studio desktop client, one can select "Network" as "Development" to set a local instance. At the same time, there is no such choice in the web client.
