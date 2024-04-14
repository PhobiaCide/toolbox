# `validatePassword()`

## Overview

Validates if a password meets common security criteria.

![A screenshot of the titular code snippet](../snapshots/validatePassword.png)

### Code

#### Deprecated

```js
const validatePassword = (password) => {
  // Check if password is at least 8 characters long
  if (password.length < 8) {
    return false;
  }

  // Check if password contains at least one uppercase letter
  if (!/[A-Z]/.test(password)) {
    return false;
  }

  // Check if password contains at least one lowercase letter
  if (!/[a-z]/.test(password)) {
    return false;
  }

  // Check if password contains at least one digit
  if (!/\d/.test(password)) {
    return false;
  }

  // Check if password contains at least one special character
  if (!/[!@#$%^&*()_+\-=\[\]{};':"\\|,.<>\/?]/.test(password)) {
    return false;
  }

  // If all criteria are met, return true
  return true;
}
```
#### New Version

```js
/**
 * Validates a password against common criteria.
 * Checks if the password meets the following conditions:
 * - At least 8 characters long
 * - Contains at least one uppercase letter
 * - Contains at least one lowercase letter
 * - Contains at least one digit
 * - Contains at least one special character
 * @param {string} password - The password to validate.
 * @returns {boolean} True if the password meets all criteria, false otherwise.
 */
const validatePassword = (password) =>
  // Check if password is less than 8 characters long
  || password.length < 8
  // Or if password does not contain at least one uppercase letter
  || !/[A-Z]/.test(password)
  // Or if password does not contain at least one lowercase letter
  || !/[a-z]/.test(password)
  // Or if password does not contain at least one digit
  || !/\d/.test(password)
  // Or if password does not contain at least one special character
  || !/[!@#$%^&*()_+\-=\[\]{};':"\\|,.<>\/?]/.test(password)
  // If any of the conditions above are true, return false
  ? false
  // If none of the criteria are met, return true
  : true;
```
