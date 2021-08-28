---
title: 'alt.emit'
description: 'Used to emit from one resource to another or the same resource.'
prefix: '[Client]'
---

# alt.emit

`alt.emit` will emit an event across multiple resources or a single resource. An event being a similar to calling a function by the name given in its first parameter.

## Usage
```js
alt.emit('customEventName', 'hello', 'world');
```

## Example

```js
alt.on('customEventName', (arg1, arg2) => {
    console.log(`${arg1} ${arg2}`);
    // Prints 'hello world'
});

alt.emit('customEventName', 'hello', 'world');
```
