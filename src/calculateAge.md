# `calculateAge()`

![A screenshot of the titular code snippet](../snapshots/calculateAge.png)

## Overview

Calculates the age based on a given birth date.

### Dependencies

None

### Code

```js
const calculateAge = (birthDate) => {
  // initialize a new date object
  const currentDate = new Date();
  // calculate the difference in years between the two dates
  const yearDifference = currentDate.getFullYear() - birthDate.getFullYear();
  // calculate the difference in months between the two dates
  const monthDifference = currentDate.getMonth() - birthDate.getMonth();
  // calculate the difference in days between the two dates
  const dayDifference = currentDate.getDate() - birthDate.getDate();

  // return yearDifference - 1 if all other values are 0
  // otherwise, just return yearDifference
  return monthDifference < 0 || (monthDifference === 0 && dayDifference < 0)
    ? yearDifference - 1
    : yearDifference;
};
```
