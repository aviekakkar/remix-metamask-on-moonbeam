🧑‍💻 [ECOSYSTEM CHALLENGE] Using Remix and MetaMask on Moonbeam

### Challenge description
This challenge combines a few different things, centered explicitly in MetaMask and Remix. This can be done using other tools, but we recommend these two as they provide the easiest path to victory :crown:.

The idea is to deploy an ERC20 token onto Moonbase Alpha, and send at least 5 tokens from one account (referred to as account01 from now on) to another (referred to as account02).

For the ERC20 token contract, the following address needs to be added as an approved spender (for a minimum of 5 ERC20 token, remember to account for the decimals :wink:): 0x12Cb274aAD8251C875c0bf6872b67d9983E53fDd

Another contract (referred to as checkContract) needs to be deployed, and will have 3 variables stored in it (these variables need to be made public, please use the exact names provided for the variables):

address1: the address of account01
address2: the address of account02
addressToken: the address of the deployed ERC20 token contract.
Funds for deployment can be requested from the Faucet set up in Moonbeam's Discord channel.

### Submission requirements
The submitted result is only the deployed address of checkContract. The contract must only hold these three variables and nothing more. The addresses needed to complete the challenge will be extracted from it.

The verification process will use the address of the checkContract to verify that the balance of _account01 and account02 is higher or equal than 5 ERC20 tokens. Also, the script will try to perform a token transfer from the approved spender to another address, and verify that the transaction went through successfully.

### Resources
In our Docs Website you will find lots of information available:

- MetaMask
- Remix
- Connect to Moonbase
- Moonbase Faucet
