# `isValidEmail()`

## Overview

Validates if a given string is a valid email address.

### At A Glance

![A screenshot of the titular code snippet](../snapshots/isValidEmail.png)

### Code

```js
const isValidEmail = (email) => {
  const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return regex.test(email);
};
```
