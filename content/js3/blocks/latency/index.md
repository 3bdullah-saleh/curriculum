+++
title = '🗓️ Latency'
headless = true
time = 5
facilitation = false
emoji= '🧩'
[objectives]
  1='Define latency'
+++

```mermaid
graph LR
    fetch[(🐕 fetch)] --> |sends a| Request{📤 Request}
    Request --> |has a latency| TimeProblem[🗓️ Time Problem]
```

Once we are taking our data on a journey over a network, we introduce the problem of latency. Latency is the time taken for a request to traverse the network.

> 💡 Network latency is travel time.

Why is latency a problem? Because it means we need to **wait** for our data. But if we stopped our program to wait for data, then we wouldn't be able to do anything else. We need to handle this time problem. Programming often involves time problems, and latency is just one of them.
