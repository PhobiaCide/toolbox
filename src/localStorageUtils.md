# `localStorageUtils()`

![A screenshot of the titular code snippet](../snapshots/localStorageUtils.png)

## Overview

An object containing utility functions to simplify interactions with the browser's localStorage.

### Dependencies

None

### Code

```js
const localStorageUtils = {
  getItem: (key) => localStorage.getItem(key),
  setItem: (key, value) => localStorage.setItem(key, value),
  removeItem: (key) => localStorage.removeItem(key),
  clear: () => localStorage.clear()
};
```
