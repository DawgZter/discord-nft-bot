# discord-nft-bot

A [discord.js](https://discord.js.org/) bot that listens to messages in channels and replies with items from an nft collection.

Originally developed for [@dutchtide](https://twitter.com/dutchtide)'s [𝕄𝕚𝕕𝕟𝕚𝕘𝕙𝕥 夏季 𝔹𝕣𝕖𝕖𝕫𝕖](https://opensea.io/collection/midnightbreeze) collection.

An OpenSea API key is needed - [request one here](https://docs.opensea.io/reference/request-an-api-key).

## Supported syntax:

- `#1234`
- `#ensname.eth`
- `#openseaUsername`
- `#random`

Example reply:

![Example bot reply](./example.png)

Example console output:

```
------------------------------------------------------------
Logged in as Dutchtide Listen Bot#8486!
Listening for messages...
------------------------------------------------------------
Message from ryanio in #🌴🎐view-the-breeze🎐🌴:
> #random
Fetching #2248...
Replied with #2248
------------------------------------------------------------
```

Provided metadata fields:

- Owner
- Last sale
- Listed for
- Highest offer

You can add properties of the specific nft by formatting `asset.traits` and adding to the `fields` array.

## Setup

### Env

Please define these env variables for the repostitory to work as intended.

#### APIs

- `DISCORD_TOKEN`
- `OPENSEA_API_TOKEN`
- `INFURA_PROJECT_ID`

#### Project specific

- `TOKEN_NAME`
- `TOKEN_ADDRESS`
- `MIN_TOKEN_ID`
- `MAX_TOKEN_ID`

### Bot

To get your `DISCORD_TOKEN`, create a bot at [https://discord.com/developers/applications](https://discord.com/developers/applications), set up the bot and permissions (Read/Write messages), and have it join your server.

The `DISCORD_TOKEN` looks like this: `OTE5MzY5ODIyNzEyNzc5NzUz.YBuz2g.x1rGh4zx_XlSNj43oreukvlwsfw`
