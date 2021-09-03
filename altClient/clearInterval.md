---
title: 'alt.clearInterval'
description: 'Clears a timer set with the setInterval function.'
prefix: '[Client]'
---

# alt.clearInterval

Used to stop an interval from executing the logic inside of it.

See [alt.setInterval](setInterval.md) for more information.

### Declaration

```typescript
alt.clearInterval(id: number): void
```

### Usage

```js
alt.clearInterval(someTimeoutValue);
```

### Real World Example

```js
const someTimeoutValue = alt.setTimeout(() => {
    alt.log('Client Says Hello!');
}, 5000);

alt.clearInterval(someTimeoutValue);
```

_These examples assume you have imported `alt` from `alt-client`._