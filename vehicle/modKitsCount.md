---
title: 'vehicle.modKitsCount'
description: 'Used to get the modKit that is applied to the vehicle.'
prefix: '[Server]'
---

# modKitsCount

Used to `get` the total modKits available for a vehicle.

Returns a `number`.

### Declaration

```typescript
vehicle.modKitsCount: number;
```

### Usage

```js
const count = vehicle.modKitsCount;
```

### Real World Example

```js
const vehicle = new alt.Vehicle('elegy', 0, 0, 0, 0, 0, 0);

if (vehicle.modKitsCount >= 1) {
    vehicle.modKit = 1;
}
```

_These examples assume you have imported `alt` from `alt-server`._