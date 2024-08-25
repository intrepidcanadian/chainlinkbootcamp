Your assignment is as follows:

Using chainlink-local, write a test for this Github project.

Please note: During Exercise #3, we used Chainlink Local's Forked Mode with Foundry. For this homework, you should use Chainlink Local's Local Mode with Hardhat.

In the test, you must:

1. Create an instance of CCIPLocalSimulator.sol smart contract

2. Call the configuration() function to get Router contract address

3. Create instances of the following smart contracts:

3a. CrossChainNameServiceRegister.sol
3b. CrossChainNameServiceReceiver.sol
3c. CrossChainNameServiceLookup.sol

4. Call enableChain() function where needed

5. Call the register() function and provide both “alice.ccns” and Alice’s EOA address as function arguments.

6. Call the lookup() function and provide “alice.ccns” as a function argument. Then assert that the returned address is Alice’s EOA address.

7. Send a URL pointing to the public Github repository.

IMPORTANT: Do not provide private key or testnet rpc details. Use Hardhat Network only! If you need additional help, please refer to this Gitbook.

# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```
