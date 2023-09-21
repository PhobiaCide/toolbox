# `truncateString()`

## Overview

Truncates a string to a specified maximum length and adds ellipses if necessary.

### At A Glance

![A screenshot of the titular code snippet](../snapshots/truncateString.png)

### Code

```js
function truncateString(str, maxLength) {
  if (str.length <= maxLength) {
    return str;
  } else {
    return str.slice(0, maxLength) + "...";
  }
}
```
