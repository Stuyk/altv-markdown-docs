---
title: 'alt.clearNextTick'
description: 'Clears a timer set with the function.'
prefix: '[Server]'
---

# alt.clearNextTick

Used to clear a nextTick event before it is ran. The logic inside of the nextTick event is never executed if cleared in time.

## Usage

```js
alt.clearNextTick(someNextTick);
```


## Example Usage

```js
const someNextTick = alt.everyTick(() => {
    console.log('hello world');
});

alt.clearNextTick(someNextTick);
```
