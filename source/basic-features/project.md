# Project

In the upper left corner "Project" panel, one can create a new project, open projects and check all the local and remote projects.

## Create Project

Click "Create Project", one can create a new project in either local or cloud under one's account. The created projects will show in both desktop and web clients in real-time. Creating a project and editing it all function is solely the Ethereum Studio without other development tools like Visual Studio Code.

 

 

In the "Create a New Project" panel, one can input the "Project name", and the "Project location" will automatically generate a document path following "C:\Users\Administrator\Ethereum Studio". 

 

 

Users can change the path in any other documents they want. Click the "Choose" button on the left of the default path, and one will see all documents on the whole computer. One can choose another existing document as the new project location. Besides, one can create a new document as the new project location. Be careful that the new project location must be an empty file in any way.

 

 

 

### Empty Template

In "Template", one can choose "Empty Project" and click "Create Project" to generate a default empty project with contracts "Main.sol". The only "Main.sol" contract has no content but Main's empty contract file. One can use this contract as a minimum viable product to build smart contracts from scratch by oneself. This template is the most general document structure in the Ethereum Studio.

 

 

### Coin Template

In "Template", one can choose "Coin" and click "Create Project" to generate a default empty project with contracts "Coin.sol". This template is a primary contract with variables and functions that could help users have a basic understanding of smart contracts and help users build coin-related contracts. Please remember that a definition of coin functions creates this contract and does not follow any principles.

 

 

 

### ERC20 Template

In "Template", one can choose "ERC20 token" and click "Create Project" to generate an ERC20 project with several contracts, including "ERC20.sol". The "ERC20.sol" contract follows the ERC20 standard, so it has all functions the ERC20 standard required. Some "IERC20" contracts are interfaces of the ERC20 contract. Using the interfaces would reduce setting parameters and provide reliable third-party essential functions for users to call. This template has more standard required contracts than "Coin Template" and generates ERC20 standard related contracts and interfaces local.

 

 

### Basic Open Zeppelin Template

In "Template", one can choose "Basics - ERC20, ERC721 & ERC1155(v3.1+)" and click "Create Project" to generate a project with three ERC standard contracts including "GLDToken.sol", "GameItem.sol" and "GameItems.sol". Those three smart contracts inherited ERC20, ERC721 and ERC1155 standards, respectively. All three projects import ERC standards through Open Zeppelin online. Those contracts realized only constructor function but basic parameters settled. One can use those smart contracts to understand how the ERC20 tokens and NFTs are minted by oneself. The "Basic OpenZeppline Template" will use contracts online with other templates. Users only need to import ERC standard contracts through code. There are no specific ERC standard contracts and interfaces in projects, which will leave projects clean and simple. One will focus on core contracts of projects.

 

 

### Metacoin Template

In "Template", one can choose "Metacoin" with default framework "Dockerized Truffle" and click "Create Project" to generate a project with several contracts including "ConvertLib.sol", "MetaCoin.sol" and "Migrations.sol". In this project, ???

 

Only "Dockerized Truffle" can be selected in this framework since ???

 

 

 

## Frameworks Introduction

### Open Zeppelin

Open Zeppelin provides a complete suite of security products to build, manage, and inspect all aspects of software development and operations for Ethereum projects. 

 

In the Ethereum Studio, one can import Open Zeppelin contracts through the template. Detailed information about Open Zeppelin can be referred to **as Link (**[https://docs.openzeppelin.com/openzeppelin/](https://docs.openzeppelin.com/openzeppelin/)**)**.

 

### Hardhat 

Hardhat is a development environment to compile, deploy, test, and debug Ethereum software. It helps developers manage and automate the recurring tasks inherent to the process of building smart contracts and dApps and quickly introduces more functionality around this workflow. This framework means compiling, running and testing smart contracts at the very core.

 

In the Ethereum Studio, one can use Hardhat as a development framework. Developers can choose it during the creation of projects. One can also use this framework during the development process by the command line in the Ethereum Studio. Detailed information about Hardhat can be referred to **Link (**[https://hardhat.org/getting-started/](https://hardhat.org/getting-started/)**)**.

 

### Truffle

Truffle is a development environment, testing framework and asset pipeline for blockchains using the Ethereum Virtual Machine (EVM). With Truffle, users get a built-in smart contract compilation, linking, deployment and binary management. Truffle also has network management for deploying to any number of public & private networks.

 

In the Ethereum Studio, one can use Hardhat as a development framework. Developers can choose it during the creation of projects. One can also use this framework during the development process by the command line in the Ethereum Studio. Detailed information about Hardhat can be referred to **Link (**[https://trufflesuite.com/docs/truffle/](https://trufflesuite.com/docs/truffle/)**)**.

 

Dockerized Truffle used only Truffle in Docker image without other dependencies like Node.js and Npm in local. The other two Frameworks, Hardhat and Waffle, require Node.js and Npm.

 

### Waffle

Waffle is a library for writing and testing smart contracts. Sweeter, simpler and faster than Truffle. In Waffle, "Simpler" means minimalistic, few dependencies; "Sweeter" means nice syntax, easy to extend; "Faster" means to focus on the speed of tests execution. Waffle uses a set of chai matches, and it can import contracts from npm modules easily. There is also a fast compilation with native and dockerized solidity contracts. It provides fixtures that help write fast and maintainable test suites.

 

In the Ethereum Studio, one can use Waffle as a development framework. Developers can choose it during the creation of projects. One can also use this framework during the development process by the command line in the Ethereum Studio. Detailed information about Waffle can be referred to **Link (**[https://ethereum-waffle.readthedocs.io/en/latest/](https://ethereum-waffle.readthedocs.io/en/latest/)**)**.

 

## Open Project

Click "Open Project", one can check the location of the current project or try to open an existed project in the system anywhere.



## Local Projects and Remote Projects

In the "Local Projects" and "Remote Projects" of the "File" panel, one can see all the projects in local and cloud under one's account. One can quickly change a project through the panel, and this would be helpful for muti-project developers.
