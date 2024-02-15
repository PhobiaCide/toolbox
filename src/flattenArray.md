# `flattenArray()`

![A screenshot of the titular code snippet](../snapshots/flattenArray.png)

## Overview

Flattens a nested array into a single-level array.

### Dependencies

None

### Code

```js
const flattenArray = (arr) =>
  arr.reduce(
    (acc, val) =>
      Array.isArray(val) ? acc.concat(flattenArray(val)) : acc.concat(val),
    []
  );
```
