# Taco Town 🌮

A small Express + EJS website that shows how to make different tacos. Pick chicken, beef or fish and the page builds the full recipe from JSON data.

## Features
- Three taco buttons, built automatically from the JSON data
- Recipe card with price, filling, salsa (with a 1-3 chili heat meter) and toppings
- Each topping shows its quantity and ingredient chips
- Responsive layout that works on phones

## Tech
Node.js, Express, EJS, body-parser, plain CSS

## Run it
    npm install
    node index.js
Then open http://localhost:3000

## How it works
1. Each button submits a form (`POST /recipe`) with a `choice` such as `beef`.
2. The server finds the matching taco in the JSON data.
3. `views/index.ejs` loops through the data and renders the recipe card.

## Project structure
    taco-town/
    ├── index.js
    ├── recipe.json
    ├── views/index.ejs
    └── public/styles/main.css

## What I learned
Working with nested JSON, Express routes, form data and EJS templates.
