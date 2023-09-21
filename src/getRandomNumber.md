# `getRandomNumber()`

## Overview

Generates a pseudo random number within a given range.

### At A Glance

![A screenshot of the titular code snippet](../snapshots/getRandomNumber.png)

### Code

```js
const getRandomNumber = (min, max) =>
  Math.floor(Math.random() * (max - min + 1)) + min;
```
