+++
title = '❓❓❓ Multiple parameters'
headless = true
time = 30
facilitation = false
emoji= '🧩'
[objectives]
    1='Describe how to extend a strategy for one item to multiple items'
+++

We can now take on another test case: when there are multiple query parameters in the url string.
In the case where the query string has multiple parameters, then each key-value pair is separated by a `&` (ampersand)
symbol

```js
test("given a query string with multiple key-value pairs, returns them in object form", function () {
  const input = "fruit=apple&city=london";
  const currentOutput = parseQueryString(input);
  const targetOutput = { fruit: "apple", from: "y" };

  expect(currentOutput).toStrictEqual(targetOutput);
});
```

### 🧭 Strategy

We've already worked out how to update the query params object given a single key-value pair in the query string.
So our strategy will be to break the query string part into an array of key-value pairs👍

> 💡 Key insight: If we can do it for **one pair**, we can try doing it for a **list of pairs** too.

Our strategy will consist of breaking the query string into an array and then iterating through it to update the query object on each iteration.

Let's start with the first sub-goal.

> 🎯 Sub-goal 1: split the query string into an array of key-value pairs

We can take the `"to=x&from=y"` string and split it by the `"&"` character.

```js {linenos=table,hl_lines=[4] ,linenostart=1}
function parseQueryString(queryString) {
  // suppose queryString has a value of "to=x&from=y"
  const queryParams = {}; // 'to=x&from=y'
  const keyValuePairs = encodedParams.split("&"); // ['to=x', from=y']
}
```

> 🎯 Sub-goal 2: iterate through the key-value pairs and update the query params object

Once we've got an array we can iterate through the key-value pairs and update the `queryParams` object each time.

```js {linenos=table,hl_lines=["6-9"] ,linenostart=1}
function parseQueryString(queryString) {
  // assume queryString has a value of 'to=x&from=y'
  const queryParams = {};
  const keyValuePairs = queryString.split("&"); // ['to=x', from=y']

  for (const pair of keyValuePairs) {
    const [key, value] = pair.split("=");
    queryParams[key] = value;
  }

  return queryParams;
}
```
