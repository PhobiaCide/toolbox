# `truncateString()`

## Overview

Truncates a string to a specified maximum length and adds ellipses if necessary.

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
