# cryptogrambot-docker

CryptoGramBot Docker

Current CryptoGramBot version : 0.3.313
`https://github.com/mehtadone/CryptoGramBot/releases`

CryptoGramBot `https://github.com/mehtadone/CryptoGramBot`

## Quick Guide

- Setup your Telegram bot. see `https://github.com/mehtadone/CryptoGramBot` or `https://www.youtube.com/watch?v=HPYl5FbXZ94`

- download the configure file from `https://github.com/mehtadone/CryptoGramBot/blob/master/CryptoGramBot/appsettings.json`

- Fill in your config in appsettings.json. Bot ID is WITHOUT Bot and choose whether you want enable each service (true or false). NOTE: Create a new API key at your exchange, do not use an existing API key. See for `https://github.com/mehtadone/CryptoGramBot` reference.

- To Run Container and replace <your path> with the full path where the appsettings.json file is.

```bash
docker run -d -p 5002:5002 -v <your path>/appsettings.json:/cryptogrambot/appsettings.json jakkie/cryptogrambot-docker
```

- After CryptoGramBot is running go to telegram and interact with the bot `https://github.com/mehtadone/CryptoGramBot#bot-commands`

## DIY Guide for building your docker container

### Installing the container

- Build the container from the repository.

```bash
docker build -t cryptogrambot .
```

- To build with a specific CryptoGramBot version. Just change the CryptoGramBot version to the version you want. To see which versions are available go to `https://github.com/mehtadone/CryptoGramBot/releases`

```bash
docker build -t cryptogrambot --build-arg CRYPTOGRAMBOT_VERSION=0.3.313 .
```

### Running with docker-compose

- To install docker compose see `https://docs.docker.com/compose/install/`

- To start docker-compose to run all the containers.

```bash
docker-compose up -d
```

Tip jar, support appreciated!

BTC: 1JvpPGe22ViBYNiNrA3nwtg71Jta5vqXAi

BCH: qzndnssc368k5h5ndg6h2d5pewmkycd50c9gxcpre6

LTC: LWRDbKva26cATarA2PoTXTpKVJwCRCzbNC

ETH: 0x13346b1DcF1f923bD357a1C8900C4475342e5255

ZEC: t1YgFzgYdRymwJcwTBaS1harBf1sPakgbZ4

DASH: XanACebtJkEZsfRaMahbnqCU4LPt42e3mE