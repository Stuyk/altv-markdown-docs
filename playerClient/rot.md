---
title: 'player.rot'
description: 'Get the rotation of a player.'
prefix: '[Client]'
---

# alt.Player.local.rot

Get the player's rotation.

**Syntax**

```js
readonly rot: { x: number, y: number, z: number };
```

### Real World Example

```js
const localPlayerRot = alt.Player.local.rot;
alt.log(JSON.stringify(localPlayerRot));
```

_alt.Player.local can also be a **player instance** from server_
