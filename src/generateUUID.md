# `generateUUID()`

## Overview

Generates a universally unique identifier (UUID).

### Code

```js
const generateUUID = () => {
  return "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, function (c) {
    const r = (Math.random() * 16) | 0,
      v = c === "x" ? r : (r & 0x3) | 0x8;
    return v.toString(16);
  });
};

const uniqueId = uuid();
console.log(uniqueId);
```
