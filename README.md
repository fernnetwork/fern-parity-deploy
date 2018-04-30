# fern-parity-deploy

Parity deployment configurations for local development on a private PoA network. Initially generated using [parity-deploy](https://github.com/paritytech/parity-deploy).

Running the `docker-compose` command will launch a parity chain with the following configurations:
- 3 authority nodes, proof of authority chain
- An ethstats monitoring instance that can be accessed at http://localhost:3001
- An account `0x00Ea169ce7e0992960D3BdE6F5D539C955316432` with lots of eths to send around for testing. 

## Prerequisites
- docker & docker-compose

## Commands
Starting the services:
```
$ docker-compose up -d --build
```

Stopping the services:
```
$ docker-compose down
```

Deleting chain data:
```
$ rm -rf data
```
