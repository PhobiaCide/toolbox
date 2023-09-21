# `isPalindrome()`

## Overview

Checks if a string is a palindrome.

### At A Glance

![A screenshot of the titular code snippet](../snapshots/isPalindrome.png)

### Code

```js
function isPalindrome(str) {
  let reversedStr = str.split("").reverse().join("");
  return str === reversedStr;
}
```
