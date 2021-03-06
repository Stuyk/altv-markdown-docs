---
title: 'vehicle.getArmoredWindowHealth'
description: 'Used to get the current damage health of a specific window.'
prefix: '[Server]'
---

# getArmoredWindowHealth

Used to `get` the current health of a specific window id.

```js
{
    VEH_EXT_WINDSCREEN: 0,
    VEH_EXT_WINDSCREEN_R: 1,
    VEH_EXT_WINDOW_LF: 2,
    VEH_EXT_WINDOW_RF: 3,
    VEH_EXT_WINDOW_LR: 4,
    VEH_EXT_WINDOW_RR: 5,
    VEH_EXT_WINDOW_LM: 6,
    VEH_EXT_WINDOW_RM: 7
}
```

_LF = Left Front,  RF = Right Front, etc._

Returns a `number`.

### Declaration

```typescript
vehicle.getArmoredWindowHealth(window: number): number;
```

### Usage

```js
const windowHealth = vehicle.getArmoredWindowHealth();
```

### Real World Example

May be more useful to see it on a vehicle with armored windows.

```js
const vehicle = new alt.Vehicle('riot', 0, 0, 0, 0, 0, 0);
const windowHealth = vehicle.getArmoredWindowHealth(0);
```

_These examples assume you have vehicle created or available on `server-side`_