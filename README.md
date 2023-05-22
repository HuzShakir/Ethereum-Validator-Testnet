# Ethereum-Validator-Testnet

As a validator, it stores a complete copy of the Ethereum blockchain and participates in the network as a validator, verifying transactions and adding new blocks to the blockchain.

Steps to Follow:
* Create a jwt secret and store it in `./jwtsecret/jwt.hex`, this jwt token is used by execution and consensus client for message authentication.
* Import your wallet in `./validator` that would be `./validator/direct/account/all-accounts.keystore.json`
* Store your wallet password in `./validator/password.txt`
* Run the validator by `docker compose up`


## Prometheus

Metrics for Validator 
![image](https://github.com/HuzShakir/Ethereum-Validator-Testnet/assets/63386941/0adb9600-5932-4fd3-9468-d215a0998cc1)

Metrics for Execution Client
![image](https://github.com/HuzShakir/Ethereum-Validator-Testnet/assets/63386941/16e88548-dc29-4579-ae1b-44a9341d8086)
