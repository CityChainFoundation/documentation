# How to easily run the City Chain block indexer

The block indexer is based on the Nako indexer by CoinVault.

Repo:  [https://github.com/CityChainFoundation/city-block-indexer](https://github.com/CityChainFoundation/city-block-indexer)

To run the block indexer from pre-compiled binaries, simply download the [docker-compose.yml](https://github.com/CityChainFoundation/city-chain/blob/master/Docker/BlockExplorerNako/docker-compose.yml) and run the following docker-compose file on a server with Docker:

```
docker-compose up
```

This should start up 3 images:

city-nako - Which runs the indexer, exposes an API on port 9019.

city-client - Which runs the daemon, exposes the RPC API on port 5000 and P2P port 4333 (expose this publicly to make the node a public full node).

city-mongo - Which runs the MongoDB instance that stores the blockchain information.
