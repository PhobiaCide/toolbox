# `isValidEmail()`

## Overview

Validates if a given string is a valid email address.

### Code

```js
const isValidEmail = (email) => {
  const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return regex.test(email);
};
```
