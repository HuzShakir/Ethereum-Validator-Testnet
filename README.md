# Ethereum-Validator-Testnet

As a validator, it stores a complete copy of the Ethereum blockchain and participates in the network as a validator, verifying transactions and adding new blocks to the blockchain.

### Steps to Follow:
* Create a jwt secret and store it in `./jwtsecret/jwt.hex`, this jwt token is used by execution and consensus client for message authentication.
* Import your wallet in `./validator` that would be `./validator/direct/account/all-accounts.keystore.json`
* Store your wallet password in `./validator/password.txt`
* Add the webhook url in `./config/alertmanager/config.yml`, alertmanager will notify on this webhook url if there is any alert.  
* Run the Ethereum validator by `docker compose up`


## Monitoring and Alerts

Grafana dashboard using Prometheus as a data source for metrics monitoring and visualisation, with alerts set up using Prometheus' alertmanager

#### Metrics for Execution Client


![image](https://github.com/HuzShakir/Ethereum-Validator-Testnet/assets/63386941/16e88548-dc29-4579-ae1b-44a9341d8086)

#### Metrics for Validator 

![image](https://github.com/HuzShakir/Ethereum-Validator-Testnet/assets/63386941/0adb9600-5932-4fd3-9468-d215a0998cc1)

#### Alerts sent from alertmanager to custom webhook

![image](https://github.com/HuzShakir/Ethereum-Validator-Testnet/assets/63386941/f25ab699-c639-47b6-9d47-91a9da91b4d2)
