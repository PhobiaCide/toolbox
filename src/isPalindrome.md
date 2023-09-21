# `isPalindrome()`

## Overview

Checks if a string is a palindrome.

### Code

```js
function isPalindrome(str) {
  let reversedStr = str.split("").reverse().join("");
  return str === reversedStr;
}
```
