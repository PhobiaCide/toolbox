# `shuffleArray()`

![A screenshot of the titular code snippet](../snapshots/shuffleArray.png)

## Overview

Shuffles the elements of an array randomly.

### Dependencies

None

### Code

```js
const shuffleArray = (array) => {
  array.forEach((_, i, arr) => {
    const j = Math.floor(Math.random() * (i + 1));
    [arr[i], arr[j]] = [arr[j], arr[i]];
  });
  return array;
};
```
