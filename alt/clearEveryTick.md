---
title: 'alt.clearEveryTick'
description: 'Clears a timer set with the everyTick function.'
prefix: '[Server]'
---

# alt.clearEveryTick

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
