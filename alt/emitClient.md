---
title: 'alt.emitClient'
description: 'Emits specified event to specific client.'
prefix: '[Server]'
---

# alt.emitClient

Used to emit an event to a single player. They will receive this event on `client-side` from the `server`.

Useful for opening WebViews, showing notifications, or triggering pretty much anything to show up on client-side.

### Declaration

```typescript
alt.emitClient(player: Player, eventName: string, ...args: any[]): void
```

### Usage

```js
alt.emitClient(somePlayer, 'someCustomEvent', additional, args, can, go, here);
```

### Example Usage

```js
function someCallbackFunction(player) {
    alt.emitClient(player, 'customEventName', 'hello world');
}

alt.on('playerConnect', someCallbackFunction);
```

### Optional Usage #1

This iteration of the emit will emit it to *all* players.

```js
 alt.emitClient(null, 'customEventName', 'hello world')
```

### Optional Usage #2

This iteration of the emit will emit it to players who are passed from a list.

```js
const validPlayers = alt.Player.all.filter(player => player.name === 'johnny');

 alt.emitClient(validPlayers, 'customEventName', 'hello world')
```


_These examples assume you have imported `alt` from `alt-server`._