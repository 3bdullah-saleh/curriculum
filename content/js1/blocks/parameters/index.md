+++
title = 'Parametrising a function'
headless = true
time = 5
facilitation = false
emoji= '🗄️'
[objectives]
    1='Define a _parameter_'
    2='Identify the value assigned to a parameter when a function is invoked'
    3='Differentiate between parameters and arguments'
    4='Invoke a given function with an appropriate argument to produce some target output'
    5='Give examples of how functionality can be generalised'
    6='Assess and explain whether a function can reference a given variable or not'
    7='Propose clear and meaningful parameter names for a function'
+++

To make this function reusable for any number, we need to handle inputs. We do this using a **parameter**.

{{<note type="definition" title="Definition: parameter">}}
A parameter is a special kind of variable whose value is defined by the caller.
{{</note>}}

`num` is still a variable - but as a **parameter** we don't assign `num` a value inside the function's body.
We pass an input to the function, and the value of that input is assigned to the `num` parameter when the function is called. This happens automatically.

We can add a parameter `num` to our function:

```js {linenos=table,hl_lines=[1] ,linenostart=1}
function convertToPercentage(num) {
  // now num is a parameter of convertToPercentage
  const percentage = `${num * 100}%`;
  return percentage;
}

const output1 = convertToPercentage(0.5);
const output2 = convertToPercentage(0.231);
```

In the example above, we're calling `convertToPercentage` twice: first time with an **input** of `0.5` and the second time with an **input** of `0.231`.
Instead of using the word **input** we can use the word **argument**, which has the same meaning.

> We're calling `convertToPercentage` twice, first time with an **argument** of `0.5` and the second time with an **argument** of `0.231`.

{{<note type="definition" title="Definition: argument">}}
An **argument** means an **input**
{{</note>}}

We can think of a function as a "box". We pass **arguments** to it, the function's code is executed and we get a return value after the function has finished executing. We can visualise this as follows:

```mermaid

flowchart LR
    A[argument] --> B{function}
    B --> C[return]
```

We could visualise what happens when `makeGreeting` is passed a specific **argument**:

```mermaid

flowchart LR
    A[0.231] --> B{convertToPercentage}
    B --> C[23.1%]
```

This time we have a difference in that we have defined a parameter `num` in the function declaration inside parentheses after the function name `convertToPercentage`. In our current mental model, a function call means going to `convertToPercentage` and running the code inside the function.

<iframe width="800" height="450" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=function%20convertToPercentage%28num%29%20%7B%0A%20%20const%20percentage%20%3D%20%60%24%7Bnum%20*%20100%7D%25%60%3B%0A%20%20return%20percentage%3B%0A%7D%0A%0Aconst%20output1%20%3D%20convertToPercentage%280.5%29%3B%0Aconst%20output2%20%3D%20convertToPercentage%280.23%29%3B&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

{{<note type="activity" title="exercise">}}
Use the interactive widget to see what happens when the code above is executed. Pay special attention the lines where `convertToPercentage` is called.
{{</note>}}
