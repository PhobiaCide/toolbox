# `isValidEmail()`

## Overview

Validates if a given string is a valid email address.

### Code

![A screenshot of the titular code snippet](../snapshots/isValidEmail.png)

```js
const isValidEmail = (email) => /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
```
