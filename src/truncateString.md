# `truncateString()`

## Overview

Truncates a string to a specified maximum length and adds ellipses if necessary.

### Code

![A screenshot of the titular code snippet](../snapshots/truncateString.png)

```js
const truncateString = (str, maxLength) =>
  str.length <= maxLength ? str : str.slice(0, maxLength) + "...";
```
