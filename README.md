# RAGEMP Client Natives

[![NPM version][npm-image]][npm-url]

This is a util package providing hash lists of GTA V's natives to use on
the client side of RAGE MP scripts.

## Install
```shell
npm install --save natives-ragemp
```

## Example
A little example to show you how to get infinite ammo:
```js
const NATIVES = require('natives-ragemp');

const weaponHash = NATIVES.WEAPON.GET_SELECTED_PED_WEAPON(player.handle);
mp.game.graphics.notify(`Result: ${weaponHash}`);
NATIVES.WEAPON.SET_PED_INFINITE_AMMO(player.handle, true, weaponHash);
```

## Roadmap
Only JS for now, I'll probably do a TypeScript one based on the work of
CocaColaBear or Pet-Platoon.

[npm-url]: https://www.npmjs.com/package/natives-ragemp
[npm-image]: https://img.shields.io/npm/v/natives-ragemp.svg
