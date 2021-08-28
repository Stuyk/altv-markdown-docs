---
title: 'alt.clearEveryTick'
description: 'Clears a timer set with the everyTick function.'
prefix: '[Client]'
---

# alt.clearEveryTick

Used to clear an everyTick event that calls a function very quickly.

## Usage
```js
alt.clearEveryTick(someEveryTick);
```

## Example Usage

```js
const someEveryTick = alt.everyTick(() => {
    console.log('Lots of Logging');
});

alt.clearEveryTick(someEveryTick);
```
