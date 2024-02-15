# `capitalize()`

![A screenshot of the titular code snippet](../snapshots/capitalize.png)

## Overview

Converts the first character of a string to uppercase.

### Dependencies

None

### Code

```js
const capitalize = (string) => string.charAt(0).toUpperCase() + string.slice(1);
```
