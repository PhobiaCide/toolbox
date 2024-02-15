# `truncateString()`

## Overview

Truncates a string to a specified maximum length and adds ellipses if necessary.

![A screenshot of the titular code snippet](../snapshots/truncateString.png)

### Code

```js
const truncateString = (str, maxLength) =>
  // if the length of `str` is less than `maxLength`
  str.length <= maxLength
    // then, 
    ? str
    // else, slice it for `maxLength` and append '...'
    : str.slice(0, maxLength) + "...";
```
