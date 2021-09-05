---
title: 'vehicle.setWheelDetached'
description: 'Used to set if a wheel is detached or not.'
prefix: '[Server]'
---

# setWheelDetached

Used to `set` if a wheel is detached or not.

### Declaration

```typescript
vehicle.setWheelDetached(wheel: number, isDamaged: boolean): void;
```

### Usage

```js
vehicle.setWheelDetached(0, false);
```

### Real World Example

```js
const vehicle = new alt.Vehicle('dloader', 0, 0, 0, 0, 0, 0);
vehicle.setWheelDetached(2, true);
```

_These examples assume you have imported `alt` from `alt-server`._