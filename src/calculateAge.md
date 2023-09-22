# `calculateAge()`

## Overview

Calculates the age based on a given birth date.

### Code

<img src="../snapshots/calculateAge.png" style="box-sizing:border-box;border:1px solid ck;border-radius:40px;outline-width:4px;outline-color:#113;outline-style:outset;outline-offset:-26px;">

![A screenshot of the titular code snippet in my development environment.](../snapshots/calculateAge.png)

```js
const calculateAge = (birthDate) => {
  const currentDate = new Date();
  const yearDifference = currentDate.getFullYear() - birthDate.getFullYear();
  const monthDifference = currentDate.getMonth() - birthDate.getMonth();
  const dayDifference = currentDate.getDate() - birthDate.getDate();

  return monthDifference < 0 || (monthDifference === 0 && dayDifference < 0)
    ? yearDifference - 1
    : yearDifference;
};
```
