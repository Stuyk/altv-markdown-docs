---
title: 'alt.hasResource'
description: 'Returns whether the specified resource exists.'
prefix: '[Server]'
---

# alt.hasResource

Used to determine if a resource is currently loaded by the server.

Returns a `boolean`. (true / false)

## Usage

```js
alt.hasResource('someResource');
```

## Example Usage

```js
const resource = alt.hasResource('someResource');
if (resource) {
    alt.log('someResource exists');
}
```

_These examples assume you have imported `alt` from `alt-server`._