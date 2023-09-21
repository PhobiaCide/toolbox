# `getRandomNumber()`

## Overview

Generates a pseudo random number within a given range.

### Code

```js
const getRandomNumber = (min, max) =>
  Math.floor(Math.random() * (max - min + 1)) + min;
```
