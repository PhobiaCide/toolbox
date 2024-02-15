# `isValidEmail()`

![A screenshot of the titular code snippet](../snapshots/isValidEmail.png)

## Overview

Validates if a given string is a valid email address.

### Dependencies

None

### Code

```js
const isValidEmail = (email) => /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
```
