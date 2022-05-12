# Public endpoints

Osmosis supports the following  RPC protocols:

- URI over HTTP
- JSON-RPC 2.0 over HTTP
- JSON-RPC 2.0 over websockets (might be deprecated in the future).

Anyone can setup their node with endpoints to communicate with the Osmosis blockchain, for convenience there are also some public endpoints available for querying the chain. These are recommended for development and testing purposes. For maximun control and reliability it's recommended to run your own node. 

## Official endpoints

- [https://rpc.dev-osmosis.zone/](https://rpc.dev-osmosis.zone/)

### URI over HTTP Example

```sh
curl https://rpc.dev-osmosis.zone/abci_info?
```
or simply open this url on your browswer [https://rpc.dev-osmosis.zone/abci_info?](https://rpc.dev-osmosis.zone/abci_info?)

### JSON-RPC 2.0 over HTTP Example

```sh
curl --header "Content-Type: application/json" --request POST --data '{"method": "block", "params": ["4261881"], "id": 1}' https://rpc.dev-osmosis.zone:443
```


## Chain Registry

This repo contains a chain.json and assetlist.json for a number of cosmos-sdk based chains. A chain.json contains data that makes it easy to start running or interacting with a node. 
- [Chain Registry](https://github.com/cosmos/chain-registry) : `https://github.com/cosmos/chain-registry`


## Other providers

- [DataHub](https://datahub.figment.io) : `https://datahub.figment.io`