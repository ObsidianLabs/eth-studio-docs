# Project

In the upper left corner "Project" panel, one can create a new project, open projects and check all the local and remote projects.

## Create Project

Click "Create Project", one can create a new project in either local or cloud under one's account. The created projects will show in both desktop and web clients in real-time. Creating a project and editing it all function is solely the Ethereum Studio without other development tools like Visual Studio Code.

![Pr-1](/pic/Pr-1.png)

In the "Create a New Project" panel, one can input the "Project name", and the "Project location" will automatically generate a document path following "C:\Users\Administrator\Ethereum Studio".

![Pr-2](/pic/Pr-2.png)

Users can change the path in any other documents they want. Click the "Choose" button on the left of the default path, and one will see all documents on the whole computer. One can choose another existing document as the new project location. Besides, one can create a new document as the new project location. Be careful that the new project location must be an empty file in any way.

![Pr-3](/pic/Pr-3.png)

### Frameworks
Simple introduction
### Npm Clients


### Empty Template

In "Template", one can choose "Empty Project" and click "Create Project" to generate a default empty project with contracts "Main.sol". The only "Main.sol" contract has no content but Main's empty contract file. One can use this contract as a minimum viable product to build smart contracts from scratch by oneself. This template is the most general document structure in the Ethereum Studio.

![Pr-4](/pic/Pr-4.png)

### Coin Template

In "Template", one can choose "Coin" and click "Create Project" to generate a default empty project with contracts "Coin.sol". This template is a primary contract with variables and functions that could help users have a basic understanding of smart contracts and help users build coin-related contracts. Please remember that a definition of coin functions creates this contract and does not follow any principles.

![Pr-5](/pic/Pr-5.png)

### ERC20 Template

In "Template", one can choose "ERC20 token" and click "Create Project" to generate an ERC20 project with several contracts, including "ERC20.sol". The "ERC20.sol" contract follows the ERC20 standard, so it has all functions the ERC20 standard required. Some "IERC20" contracts are interfaces of the ERC20 contract. Using the interfaces would reduce setting parameters and provide reliable third-party essential functions for users to call. This template has more standard required contracts than "Coin Template" and generates ERC20 standard related contracts and interfaces local.

![Pr-6](/pic/Pr-6.png)

### Basic Open Zeppelin Template

In "Template", one can choose "Basics - ERC20, ERC721 & ERC1155(v3.1+)" and click "Create Project" to generate a project with three ERC standard contracts including "GLDToken.sol", "GameItem.sol" and "GameItems.sol". Those three smart contracts inherited ERC20, ERC721 and ERC1155 standards, respectively. All three projects import ERC standards through Open Zeppelin online. Those contracts realized only constructor function but basic parameters settled. One can use those smart contracts to understand how the ERC20 tokens and NFTs are minted by oneself. The "Basic OpenZeppline Template" will use contracts online with other templates. Users only need to import ERC standard contracts through code. There are no specific ERC standard contracts and interfaces in projects, which will leave projects clean and simple. One will focus on core contracts of projects.

![Pr-7](/pic/Pr-7.png)

### Metacoin Template

In "Template", one can choose "Metacoin" with default framework "Dockerized Truffle" and click "Create Project" to generate a project with several contracts including "ConvertLib.sol", "MetaCoin.sol" and "Migrations.sol". In this project, ???

Only "Dockerized Truffle" can be selected in this framework since ???

![Pr-8](/pic/Pr-8.png)


## Open Project

Click "Open Project", one can check the location of the current project or try to open an existed project in the system anywhere.


![Pr-9](/pic/Pr-9.png)

![Pr-10](/pic/Pr-10.png)


## Local Projects and Cloud Projects

In the "Local Projects" and "Remote Projects" of the "File" panel, one can see all the projects in local and cloud under one's account. One can quickly change a project through the panel, and this would be helpful for muti-project developers.

![Pr-11](/pic/Pr-11.png)


## Delete Project

