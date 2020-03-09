<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# URL to this repo: https://bit.ly/2PhVNrP

# How to Create a Supply Chain Blockchain App

#### Lennart Frantzell, IBM Devloper Advocate San Francisco alf@us.ibm.com

#### David Nugent, IBM Developer Advocate, San Francisco

#### Grant Steinfeld, IBM Developer Advocate New York City

## We'll start here: [Sign up to a free IBM Cloud Account](https://ibm.biz/BdqXL6)

<img src="Signup.png">

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png">

### FYI: Satoshi Nakamoto's historik paper <i> "Bitcoin: A Peer-to-Peer Electronic Cash System" </i>  from Dec. 2008 https://bitcoin.org/bitcoin.pdf

<img src="https://github.com/LennartFr/20200227supplychain/blob/master/Screen%20Shot%202020-02-23%20at%207.56.59%20AM.png">

## Hyperledger Fabric – from The Linux Foundation – is the modular blockchain framework that has become the de facto standard for enterprise blockchain platforms.

### FYI: [Hyperledger Fabric documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.0/)

### FYI: [Hyperledger Fabric code](https://www.hyperledger.org/projects/fabric)

## In addition to the Hyperledger Fabric there is the cloud-based IBM Blockchain Platform:

### FYI: [IBM Blockchain Platform Component Overview](https://cloud.ibm.com/docs/services/blockchain?topic=blockchain-blockchain-component-overview)

### FYI: [Getting started with the IBM Blockchain Platform](https://cloud.ibm.com/docs/services/blockchain?topic=blockchain-get-started-ibp)

### FYI: <a href="https://cloud.ibm.com/docs/services/blockchain?topic=blockchain-ibp-v2-faq#ibp-v2-faq-vscode-tutorials">IBM Blockchain Platform FAQs</a>

### FYI: <a href="https://cloud.ibm.com/docs/services/blockchain?topic=blockchain-blockchain-component-overview">IBM Blockchain Platform Overview</a>

### FYI: [Blockchain Garage can help you get started with Blockchain](https://www.ibm.com/blockchain/garage)

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

## Food industry without Blockchain

<img src="FoodIndustry1.png">

<p>
 
## Food industry with Blockchain

<img src="FoodIndustry2.png">

<p>
<img src="Blockchain.png">
<p>
<img src="Transactions.png">
<p>
<img src="Ledger.png">
<p>
<img src="BP1.png">
<p>

<img src="BP2.png">


<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">


# Some Supply Chain Apps

<img src="Food. Trust1.png">

## FYI: <a href="https://www.ibm.com/blockchain/solutions/food-trust">IBM Food Trust</a>

<img src="TradeLens.png">

## FYI: <a href="https://www.tradelens.com">Trade Lens</a>

## FYI: <a href="https://www.ibm.com/blockchain/industries/supply-chain">IBM Blockchain for Supply Chain </a>

<img src="Bean2.png">

## FYI: <a href="https://www.ibm.com/thought-leadership/blockchainbean/">Blockchain Bean</a>

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# Developing Supply Chain Apps

 1. [Check Pre-requisites 2.0](https://hyperledger-fabric.readthedocs.io/en/release-2.0/prereqs.html)
 2. Download Visual Studio Code: https://code.visualstudio.com/updates/v1_39. Sept 2019 version 1.39.x Be sure to change Setttings/Update:Mode to manual  
 3. Download the IBM Blockchain Platform Extension for VS Code: https://bit.ly/2RS2R02 
 4. Trouble-shoot installation: https://github.com/IBMDeveloperNYC/coffee-supply-chain-blockchain/blob/master/TROUBLE-SHOOTING.md 

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# Hands-on Blockchain

>

Follow tutorials

### Tutorial 1 Local Smart Contract Development

<img src="VSCode.png">

Follow the typical workflow from generating a new default smart contract project, deploying code to the Local Fabric environment, and testing out your transactions via an application gateway.

<img src="LocalFabric.png">

1. CA = Certificate Authority

2. MSP = Membership Service Provider



1. Create a new default smart contract project
The extension can generate a smart contract skeleton in your chosen Hyperledger Fabric supported programming language. This means you start with a basic but useful smart contract rather than a blank-sheet.
<p>
For the purposes of this tutorial, we'll use TypeScript as the main example language. Java examples are also shown.
<p>
In VS Code, every command can be executed from the Command Palette (press Ctrl+Shift+P, or Cmd+Shift+P on MacOS). All of this extension's commands start with IBM Blockchain Platform:. In the tutorial steps, we'll explain where to click in the UI, but look out for comment-boxes like this one if you want to know the Command Palette alternatives.
<p>
In the left sidebar, click on the IBM Blockchain Platform icon (it looks like a square, and will probably be at the bottom of the set of icons if this was the latest extension you installed)
<p>
Mouse-over the SMART CONTRACTS panel, click the ... menu, and select Create New Project from the dropdown.
<p>
Command Palette alternative: Create New Project
<p>
For this tutorial, choose the Default Contract option. The Private Data Contract will be covered in a future tutorial.
<p>
Choose a smart contract language. JavaScript, TypeScript, Java and Go are all available. This tutorial will be easiest to follow if you choose TypeScript or Java (please remember to expand the Java sections if you choose Java).
<p>
The extension will ask you if you want to name the asset in the generated contract. This will default to MyAsset, but you're welcome to change it. What do you intend to use your blockchain for? This will determine what type of asset you create, update and read from the ledger: Radish? Pineapple? Penguin? Pick whatever you like! For this tutorial, we'll stick with MyAsset.
<p>
Pro Tip: If you decide to change the name of your asset, remember to swap out MyAsset for whatever you named it in future steps!
<p>
Choose a location to save the project. Click Browse, then click New Folder, and name the project what you want e.g. demoContract.
<p>
Pro Tip: Avoid using spaces when naming the project!
<p>
Click Create and then select the new folder you just created and click Save.
<p>
Finally, select Add to workspace from the list of options.

<p>
 The extension will generate you a skeleton contract based on your selected language and asset name. Once it's done, you can navigate to the Explorer view (most-likely the top icon in the left sidebar, which looks like a "document" icon) and open the src/my-asset-contract.ts (alternatively, Java contracts are in src/main/java directory, but being a Java developer you might already have guessed that). Congratulations, you've got yourself a smart contract project.






### Tutorial 2

Create a cloud blockchain deployment

After developing a smart contract against the local runtime, you'll need somewhere more permanent to deploy for further dev, proof of concept, or production use. IBM Blockchain Platform includes an offering on IBM Cloud for creating and operating a suitable runtime environment for such purposes. Its full name is "IBM Blockchain Platform on IBM Cloud", but for the sake of brevity we'll refer to it from here on out as "the cloud service". In this tutorial you will learn how to get a cloud environment set up using the cloud service.

### Tutorial 3

Deploying and transacting with IBM Cloud

Important: You will need a smart contract package and a suitable cloud environment to follow this tutorial. Follow parts 1 and 2 of this series first for instructions.


<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# Appendix

### 1.1 <a href="https://github.com/IBMDeveloperNYC/coffee-supply-chain-blockchain"> Installing Visual Studio Code </a>

### 1.2 <a href="https://cloud.ibm.com/docs/services/blockchain/howto?topic=blockchain-develop-vscode">Developing smart contracts with Visual Studio Code extension </a>

### 1.3 IBM Blockchain 101: https://ibm.co/36U1QZM
 
### 1.4 Blockchain code patterns: https://ibm.co/2GROsL0
  
### 1.5 https://github.com/Grant-Steinfeld/coffee-supply-chain-blockchain

### 1.6 Youtube Video: <a href="https://youtu.be/5b7awLi93-E">Create a simple Coffee Bean Supply Chain Blockchain on Hyperledger Fabric</a>

### 1.7 <a href="https://developer.ibm.com/patterns/coffee-supply-chain-network-hyperledger-fabric-blockchain-2/">Create a fair trade supply chain network Use Hyperledger Fabric and IBM Blockchain Platform to increase efficiency in the supply chain of a coffee retailer></a>
