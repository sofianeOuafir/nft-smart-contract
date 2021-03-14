# nft-smart-contract

How I did it:

## 1. Install Truffle

`npm install -g truffle`

## 2. Create a directory

`mkdir first-nft-smart-contract`

## 3. cd in it

`cd first-nft-smart-contract`

## 4. initialize the project

`truffle unbox react`

And leave only the scaffolding for a blank new project:

Remove all contracts in the "/contracts" folder, except the Migrations.sol file.

Remove all the tests in the "/tests" folder.

Remove all migrations except the 01_intial_migration.js.

## GET ERC 721 Contract from openzeppelin package

`npm install --save @openzeppelin/contracts@v3.0.0`

## Add a "MyToken.sol" file to the "/contracts" folder

```
pragma solidity >= 0.6.0;

import "@openzeppelin/contracts/token/ERC721/ERC721.sol";

contract MyToken is ERC721 {
  constructor() ERC721("MyTokenName", "MyTokenSymbol") public {
  }
}
```

