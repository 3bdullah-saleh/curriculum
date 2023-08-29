+++
title = '➕ Summation'
headless = true
time = 20
facilitation = false
emoji= '🧩'
[objectives]
    1='Describe how to sum the numbers in a list'
+++

> 🎯 Sub-goal: compute the sum of an array of numbers.

To sum a list we can initialise a variable with a value of `0`.

We then need to **repeatedly** increment `count` for each item in the `list`.

```js
let total = 0;
const list = [1, 2, 3, 4, 5];

total += list[0]; // access a list element and add to total
total += list[1];
total += list[2];
total += list[3];
total += list[4];
```

However, this method doesn't work for any array.
If the number of items in `list` changes then we may have to change the number of statements updating the `total`.

{{<tabs name="Playing computer">}}

{{<tab name="🕹️ Playing computer">}}
Use the [Code Visualiser](https://pythontutor.com/render.html#mode=display) to **play computer** with the code above.
{{</tab>}}

{{</tabs>}}
