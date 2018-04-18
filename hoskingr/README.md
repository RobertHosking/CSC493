# Payvr ERC20 Token (YAP)

This repo contains the Ethereum smart contract that produces the tokens for Payvr.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

To trade ERC20 Tokens, you will need a Ether wallet that is ERC20 compatible.

We reccommend [Trust Wallet](https://trustwalletapp.com/) for iOS and Android.

To deploy this smart contract yourself, follow [this guide](https://medium.com/mercuryprotocol/dev-highlights-of-this-week-cb33e58c745f)
You will need to install the Go-Ethereum (Geth) framework and sync the Ethereum blockchain.

### Install and Deploy

Install the Geth framework:

```
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install ethereum
```
to begin syncing the Ethereum blockchain without performing verification on each block hash, run

```
geth --fast
```
Install a solC (solidity complier)

```
sudo add-apt-repository ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install solc
which solc
```

in the geth console type

```
admin.setSolc("path/to/solc")
```
now type

```
eth.getCompilers()
```
It should show that you have `['Solidity']` installed.

From here, follow [this guide](https://github.com/ethereum/go-ethereum/wiki/Contract-Tutorial#the-coin) using the contents of `coin.sol` as the smartcontract code.

## Built With

* [Ethereum](https://ethereum.org/) - The Blockchain hosting the smart contract
* [Solidity](http://solidity.readthedocs.io/en/v0.4.21/) - Smartcontract Programming Language used
* [Geth](https://github.com/ethereum/go-ethereum/wiki/geth) - Used to compile the Smart contract and interface with the Ethereum network

## Contributing

We welcome suggestions to our smart contract code.

## License

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

```
http://www.apache.org/licenses/LICENSE-2.0
```

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

