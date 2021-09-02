---
title: 'alt.emitClient'
description: 'Emits specified event to specific client.'
prefix: '[Server]'
---

# alt.emitClient

Used to emit an event to a single player. They will receive this event on `client-side` from the `server`.

Useful for opening WebViews, showing notifications, or triggering pretty much anything to show up on client-side.


## Usage

```js
alt.emitClient(somePlayer, 'someCustomEvent', additional, args, can, go, here);
```

## Example Usage

```js
function someCallbackFunction(player) {
    alt.emitClient(player, 'customEventName', 'hello world');
}

alt.on('playerConnect', someCallbackFunction);
```

_These examples assume you have imported `alt` from `alt-server`._