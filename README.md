# Algorand Royalty Smart Contract
This contract is deployed alongside and Algorand Standard Asset(ASA) which is to be sold as and NFT to collect royalty from subsequent sales of the ASA.

# Algorand ASA's as NFT's
An angorand ASA with the total parameter of 1 and decimal parameter of 0.

# Royalty for NFT Sales
Royalty is a really big reason to sell your creative work digitally over a Blockchain. Using smart contracts is a way to ensure that creators get their royalty on subsequent sales of their work in a guaranteed manner.

# Sale Flow
- Seller sets up the NFT for sale on our App which is a stateful smart contract.
- Buyer pays the specified amount to the the App. (Note: not directly to the seller)
- On recipt of the payment the NFT is transfered to the buyer
- The App remits the sale amount minus the royalty fee to the seller. 
- The royalty is collected on the App an can be redeamed by the creator at any time.

# PyTEAL
This contract is written in PyTEAL which is one of the supported languages to write TEAL smart contracts.

# Dev environment
- We assume you have an [algorand node](https://developer.algorand.org/docs/run-a-node/setup/install/) running or the [algorand sandbox](https://github.com/algorand/sandbox).
- [PyTEAL installed](https://pyteal.readthedocs.io/en/stable/installation.html)
- Nodejs configured for your system
- From the node folder run `npm install` or `yarn install`
- Alternatively you can globaly install the requirements `npm install -g typescript algosdk ts-node`
- For the test deployment we will use the algorand node and for the production deployment we could set up a node on the mainnet but we will be using [purestake.io](https://purestake.io).

# Understanding Teal
Teal is a DSL which we can implement in python. Although teal and python code cant be mixed.
We create chains of teal instruction in Python using the Seq Teal type which is a chain of TEAL instructions. 
In TEAL functions are called subroutines. Teal compiles the teal instructions into a Approval program and a Clear program. ... To be continued soon.

 
