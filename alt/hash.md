---
title: 'alt.hash'
description: 'Creates a hash using Jenkins one-at-a-time algorithm.'
prefix: '[Server]'
---

# alt.hash

Performs a `joaat` hash on a string. Fancy way of saying a hash algorithm that GTA:V uses.

Returns a `string`.

## Usage

```js
alt.hash('washington');
```


## Example Usage

```js
const hash = alt.hash('washington');
alt.log(hash);
```

_These examples assume you have imported `alt` from `alt-server`._