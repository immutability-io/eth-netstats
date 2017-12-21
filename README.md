Ethereum Network Stats
============

This is a visual interface for tracking ethereum network status. It uses WebSockets to receive stats from running nodes and output them through an angular interface. It is the front-end implementation for [eth-net-intelligence-api](https://github.com/immutability-io/eth-net-intelligence-api).

## Part of the Immutability tutorial
The intent of this repo is to provide a Docker image for use with the Immutability tutorial. As such, only the Docker aspects of running this tool will be described.

## Installation

```sh
$ docker pull immutability/ethstats
$ docker run -d -p 3000:3000  --network ethereum --name=ethstats --network-alias=ethstats -e WS_SECRET=$WS_SECRET immutability/ethstats
```

Note: the `WS_SECRET` environment variable needs to be the same one used for  [eth-net-intelligence-api](https://github.com/immutability-io/eth-net-intelligence-api).

## Usage

If everything was configured properly, see the interface at http://localhost:3000
