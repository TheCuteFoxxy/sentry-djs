<div align="center">
  <br />
  <p>
    <a href="https://sentrybot.xyz"><img src="https://sentrybot.xyz/assets/main.png" width="546" alt="sentry-djs" /></a>
  </p>
  <br />
  <p>
    <a href="https://www.npmjs.com/package/sentry-djs"><img src="https://img.shields.io/npm/v/sentry-djs" alt="NPM version" /></a>
    <a href="https://www.npmjs.com/package/sentry-djs"><img src="https://img.shields.io/npm/dt/sentry-djs" alt="NPM downloads" /></a>
    <a href="https://github.com/TheCuteFoxxy/sentry-djs/blob/master/LICENSE"><img src="https://img.shields.io/npm/l/sentry-djs" alt="License" /></a>
    <a href="https://discord.gg/e4S4PaK"><img src="https://img.shields.io/discord/763079551470665758?label=Discord" alt="Discord" /></a>
    <a href="https://sentrybot.xyz"><img src="https://img.shields.io/website?down_color=Red&down_message=Offline&up_color=Green&up_message=Online&url=https%3A%2F%2Fsentrybot.xyz" alt="Website" /></a>
  </p>
  <p>
    <a href="https://nodei.co/npm/sentry-djs/"><img src="https://nodei.co/npm/sentry-djs.png?downloads=true&downloadRank=true&stars=true"></a>
  </p>
</div>

## Table of contents

- [About](#about)
- [Installation](#installation)
  - [Optional packages](#optional-packages)
- [Example Usage](#example-usage)
- [Links](#links)
  - [Extensions](#extensions)
- [Help](#help)

## About

Sentry-Djs is a powerful [Node.js](https://nodejs.org) module that allows you to easily interact with the
[Discord API](https://discord.com/developers/docs/intro).

- Object-oriented
- Predictable abstractions
- Performant
- 100% coverage of the Discord API

## Installation

**Node.js 14.0.0 or newer is required.**  
Ignore any warnings about unmet peer dependencies, as they're all optional.

Without voice support: `npm install sentry-djs`  



### Optional packages

- [zlib-sync](https://www.npmjs.com/package/zlib-sync) for WebSocket data compression and inflation (`npm install zlib-sync`)
- [erlpack](https://github.com/discord/erlpack) for significantly faster WebSocket data (de)serialisation (`npm install discord/erlpack`)
- One of the following packages can be installed for faster voice packet encryption and decryption:
  - [sodium](https://www.npmjs.com/package/sodium) (`npm install sodium`)
  - [libsodium.js](https://www.npmjs.com/package/libsodium-wrappers) (`npm install libsodium-wrappers`)
- [bufferutil](https://www.npmjs.com/package/bufferutil) for a much faster WebSocket connection (`npm install bufferutil`)
- [utf-8-validate](https://www.npmjs.com/package/utf-8-validate) in combination with `bufferutil` for much faster WebSocket processing (`npm install utf-8-validate`)

## Example usage

```js
const Discord = require('sentry-djs');
const client = new Discord.Client();

client.on('ready', () => {
  console.log(`Logged in as ${client.user.tag}!`);
});

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('pong');
  }
});

client.login('token');
```

## Links

- [Website](https://sentrybot.xyz/)
- [Sentry-djs Discord server](https://discord.gg/e4S4PaK)
- [Discord API Discord server](https://discord.gg/discord-api)
- [GitHub](https://github.com/TheCuteFoxxy/sentry-djs)
- [NPM](https://www.npmjs.com/thecutefoxxy/sentry-djs)
- [Related libraries](https://discordapi.com/unofficial/libs.html)

### Extensions

- [RPC](https://www.npmjs.com/package/discord-rpc) ([source](https://github.com/discordjs/RPC))


## Help

If you don't understand something, you are experiencing problems, or you just need a gentle
nudge in the right direction, please don't hesitate to join our official [Sentry-djs Server](https://discord.gg/e4S4PaK).

## Disclaimer

Sentry-djs is a modified version of Discord.js to support preffered changes and flexibility between the v11 and v12 changes.
