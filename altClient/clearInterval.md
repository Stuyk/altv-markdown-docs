---
title: 'alt.clearInterval'
description: 'Clears a timer set with the setInterval function.'
prefix: '[Client]'
---

# alt.clearInterval

Used to stop an interval from executing the logic inside of it.

### Usage

```js
alt.clearInterval(someTimeoutValue);
```

### Example Usage

```js
const someTimeoutValue = alt.setTimeout(() => {
    alt.log('Client Says Hello!');
}, 5000);

alt.clearInterval(someTimeoutValue);
```
