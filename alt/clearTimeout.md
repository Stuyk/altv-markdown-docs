---
title: 'alt.ClearTimeout'
description: 'Clears a timer set with the setTimeout function.'
prefix: '[Server]'
---

# alt.clearTimeout

Used to clear a timeout early. If the timeout is cleared the code inside of the timeout is **never** executed.

## Usage

```js
alt.clearTimeout(someTimeoutValue);
```

## Example Usage

```js
const someTimeoutValue = alt.setTimeout(() => {
    alt.log('Client Says Hello!');
}, 5000);

alt.clearTimeout(someTimeoutValue);
```
