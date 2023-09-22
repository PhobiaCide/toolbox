# `parseQueryString()`

## Overview

Parses the query string parameters from a URL and returns them as an object."

### Code

![A screenshot of the titular code snippet](../snapshots/parseQueryString.png)

```js
const parseQueryString = (url) => {
  const queryString = url.split("?")[1];
  const params = {};

  if (queryString) {
    const pairs = queryString.split("&");

    pairs.forEach((pair) => {
      const [key, value] = pair.split("=");
      params[key] = decodeURIComponent(value);
    });
  }

  return params;
};
```
