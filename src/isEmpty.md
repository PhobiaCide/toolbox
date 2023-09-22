# `isEmpty()`

## Overview

Checks if an object or array is empty.

### Code

![A screenshot of the titular code snippet](../snapshots/isEmpty.png)

```js
const isEmpty = (obj) =>
  Array.isArray(obj) ? obj.length === 0 : Object.keys(obj).length === 0;
```
