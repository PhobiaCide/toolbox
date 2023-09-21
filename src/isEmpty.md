# `isEmpty()`

## Overview

Checks if an object or array is empty.

### At A Glance

![A screenshot of the titular code snippet](../snapshots/isEmpty.png)

### Code

```js
function isEmpty(obj) {
  if (Array.isArray(obj)) {
    return obj.length === 0;
  } else {
    return Object.keys(obj).length === 0;
  }
}
```
