# `getRandomNumber()`

## Overview

Generates a pseudo random number within a given range.

### Code

![A screenshot of the titular code snippet](../snapshots/getRandomNumber.png)

```js
const getRandomNumber = (min, max) =>
  Math.floor(Math.random() * (max - min + 1)) + min;
```
