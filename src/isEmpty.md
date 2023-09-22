# `isEmpty()`

## Overview

Checks if an object or array is empty.

### At A Glance

![A screenshot of the titular code snippet](../snapshots/isEmpty.png)

### Code

```js
const isEmpty = (obj) =>
  Array.isArray(obj) ? obj.length === 0 : Object.keys(obj).length === 0;
```
