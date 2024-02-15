# `getRandomNumber()`

![A screenshot of the titular code snippet](../snapshots/getRandomNumber.png)

## Overview

Generates a pseudo random number within a given range.

### Dependencies

None

### Code

```js
const getRandomNumber = (min, max) =>
  Math.floor(Math.random() * (max - min + 1)) + min;
```
