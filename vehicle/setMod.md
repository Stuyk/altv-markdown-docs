---
title: 'vehicle.setMod'
description: 'Used to set a vehicle mod on a vehicle based on index.'
prefix: '[Server]'
---

# setMod

Used to `set` a vehicle mod on a vehicle based on index.


See [Vehicle Mods](../articles/tables/vehicle-mods.md) for more information.

### Declaration

```typescript
vehicle.setMod(modIndex: number, modValue: number): void;
```

### Usage

```js
vehicle.setMod(2, 1);
```

### Real World Example

```js
const vehicle = new alt.Vehicle('elegy', 0, 0, 0, 0, 0, 0);
vehicle.modKit = 1;
vehicle.setMod(2, 1);
```

_These examples assume you have imported `alt` from `alt-server`._