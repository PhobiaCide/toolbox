# `isPalindrome()`

![A screenshot of the titular code snippet](../snapshots/isPalindrome.png)

## Overview

Checks if a string is a palindrome.

### Dependencies

None

### Code

```js
const isPalindrome = (str) => str === str.split("").reverse().join("");
```
