---
title: 'alt.clearInterval'
description: 'Clears a timer set with the setInterval function.'
prefix: '[Server]'
---

# alt.clearInterval

Used to stop an interval from executing the logic inside of it.

See [alt.setInterval](setInterval.md) for more information.

## Usage

```js
alt.clearInterval(someTimeoutValue);
```

## Example Usage

```js
const someTimeoutValue = alt.setTimeout(() => {
    alt.log('Client Says Hello!');
}, 5000);

alt.clearInterval(someTimeoutValue);
```

_These examples assume you have imported `alt` from `alt-server`._