<h1 aling="center">CatellaTech DAO BACKEND 👷‍♂️⛓</h1>

  <a href="https://github.com/maurodesouza/profile-readme-generator/blob/master/LICENSE.md" target="_blank">
    <img alt="Badge showing project license type" src="https://img.shields.io/github/license/maurodesouza/profile-readme-generator?color=f85149">
  </a>

  <a href="#" target="_blank">
    <img src="https://img.shields.io/badge/Solidity-%5E8.0.4-363636?style=flat-square" alt="Badge showing the solidity version"/>
  </a>

  <a href="#" target="_blank">
    <img src="https://img.shields.io/badge/hardhat-2.8.4-f8fc03?style=flat-square" alt="Badge showing the hardhat version"/>
  </a>

  <a href="https://github.com/gab0071" target="_blank">
    <img alt="Author" src="https://img.shields.io/badge/made%20by-CatellaTech-blueviolet?style=flat-square">
  </a>
 

  <br>
  <br>

In summary, this Ethereum smart contract is an implementation of a decentralized autonomous organization (DAO). The DAO is designed to allow participants to make proposals and vote on them to make decisions about the organization. The contract has several functions that allow users to create proposals, vote on existing proposals, execute approved proposals, and check various information about proposals and votes. The contract uses two interfaces: `IFakeNFTMarketplace` and `ICryptoDevsNFT`, which allow the contract to interact with a fake non-fungible token (NFT) marketplace and a specific NFT called `"CryptoDevsNFT"`. The contract also has several modifiers that restrict certain functions to only be called by certain types of users or in certain circumstances.

<h2> Requirements ⬇</h2>

- Anyone with a `CryptoDevs` NFT can create a proposal to purchase a different NFT from an NFT marketplace
- Everyone with a `CryptoDevs` NFT can vote for or against the active proposals
- Each NFT counts as one vote for each proposal
- Voter cannot vote multiple times on the same proposal with the same NFT
- If majority of the voters vote for the proposal by the deadline, the NFT purchase is automatically executed

You can see the smart contract on Etherscan: <a href="https://goerli.etherscan.io/address/0x63da3d1b4a128ed40a13175901176c8944324def">Project</a>.

<hr>
<h2> Installing / Getting started </h2>

```bash
# Clone this project
$ git clone https://github.com/gab0071/DAO-BACKEND

# Access
$ cd DAO-BACKEND

# Install dependencies
$ npm install

``` 

<h2>Commands</h2>

- $ ` npx hardhat compile `
- $ ` npx hardhat run scripts/deploy.js `
- $ `npx hardhat verify --constructor-args args.js DEPLOYED_CONTRACT_ADDRESS --network goerli`

In the folder `constants/index.js`: 

```javascript
// Replace the value with your NFT contract address
const CRYPTODEVS_NFT_CONTRACT_ADDRESS =
  "YOUR_CRYPTODEVS_NFT_CONTRACT_ADDRESS_HERE";
module.exports = { CRYPTODEVS_NFT_CONTRACT_ADDRESS };
```

<h2> Technologies / Built With </h2>

- Solidity
- Metamask
- <a href="https://www.npmjs.com/package/@openzeppelin/contracts"> OpenZeppelin </a>
- <a href="https://hardhat.org/">Hardhat Framework</a>
- <a href="https://hardhat.org/hardhat-runner/plugins/nomiclabs-hardhat-etherscan">Etherscan</a>

<h2>License</h2>

<p>This project is under license from MIT. For more details, see the LICENSE file.</p>

<h2>Contributing</h2>
Contributions are always welcome! Open a PR or an issue!

<br>
<br>

<p align="center">
<br/>
  Made with ❤️ by <b>catellaTech</b>.
<p/>