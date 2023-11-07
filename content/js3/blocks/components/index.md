+++
title = '🃏 Components'
headless = true
time = 30
facilitation = false
emoji= '🧩'
[objectives]
    1='Implement components for a user interface'
+++

To build user interfaces, we decompose the interface into smaller {{<tooltip title="UI components">}}A **component** is a reusable, self-contained piece of the UI. Components are like lego blocks you can build websites with. Most websites are made by "composing" components in this way.{{</tooltip>}}. JavaScript functions enable us to reuse code: therefore we can implement UI components using JavaScript functions.

Let's consider our code thus far:

```js
const film = {
    title: "Killing of Flower Moon",
    director: "Martin Scoresese"
    times: ["15:35"],
    certificate: "15",
    duration: 112
};

const filmCard = document.createElement("section");
filmCard.innerHTML = `
<p>${film.title}</p>
`;
console.log(filmCard);
```

Our sub-goal is to be able to render _any_ film object in the user interface. To do this, we can wrap up this code to create a function.

```js
function createFilmCard(film) {
  const card = document.createElement("section");
  card.innerHTML = `
    <p>${film.title}</p>
`;
  return card;
}

const film1 = {
    title: "Killing of Flower Moon",
    director: "Martin Scoresese"
    times: ["15:35"],
    certificate: "15",
    duration: 112
};

document
  .querySelector("ul")
  .append(createShowCard(film1)); // append the film cards to the DOM

const film2 = {
    title: "Typist Artist Pirate King",
    directory: "Carol Morley"
    times: ["15:00", "20:00"],
    certificate: "12A",
    duration: 108
};

document
  .querySelector("ul")
  .append(createShowCard(film2)); // append the film cards to the DOM
```

{{<tabs>}}

{{<tab name="🔧 Implement">}}

Update the implementation of `createFilmCard` so it renders other film properties like `times` etc.

{{</tab>}}

{{<tab name="🧹 Refactor">}}

Refactor the `createFilmCard` function to use object destructuring in the parameters.

{{</tab>}}

{{</tabs>}}
