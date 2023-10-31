+++
title = '💽 Single datum'
headless = true
time = 30
facilitation = false
emoji= '🧩'
[objectives]
    1='Describe how to render a single item of data in the browser'
+++

To break down this problem, let's define a sub-goal:

> 🎯 Sub-goal: Render _any_ single datum in the user interface

We'll consider how to render a single datum before doing this for the whole list. We will start with an object like the one below:

```js
const show = {
  event: "Little Simz concert",
  date: "5th November",
  location: "02 Victoria Warehouse",
  city: "Manchester",
};
```

How can we **render** this data in the user interface?
