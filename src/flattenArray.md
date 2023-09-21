# `flattenArray()`

## Overview

Flattens a nested array into a single-level array.

### Code

```js
function flattenArray(arr) {
  return arr.reduce(
    (acc, val) =>
      Array.isArray(val) ? acc.concat(flattenArray(val)) : acc.concat(val),
    []
  );
}
```
