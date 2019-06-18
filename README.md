This repository hosts `Spend Testnet`, an implementation of the Cosmos Hub.

**Note**: Requires [Go 1.12+](https://golang.org/dl/)

## Cosmos Hub Mainnet

To run a full-node for the mainnet of the Cosmos Hub

sudo apt-get update -y

### Install GO

sudo snap install go --classic

### Install Cosmos SDK & Spend
git clone https://github.com/cosmos/gaia
cd gaia/
make build-linux

### Add the builds to alliases
echo alias spend=$(pwd)/build/./spend >> ~/.bash_aliases

echo alias spendcli=$(pwd)/build/./spendcli >> ~/.bash_aliases

## Usage 

Use spend start to start the daemon (Run spend --help to list all comands)

spend start

Copy the genesis to your config folder
There is a spendcli and spend daemon configuration folders located at ./spend 

cp genesis/genesis.json ~/.spend/config

Use spendcli to interact with the blockchain

## Disambiguation

This Cosmos-SDK project is not related to the [React-Cosmos](https://github.com/react-cosmos/react-cosmos) project (yet). Many thanks to Evan Coury and Ovidiu (@skidding) for this Github organization name. As per our agreement, this disambiguation notice will stay here.


