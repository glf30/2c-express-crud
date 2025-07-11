# Assignment 2C. Express-CRUD

---

## Goals

- Create a server using the Express module
- Create an API that serves data based on the URL request
- Allow users to `C`reate, `R`ead, `U`pdate, and `D`elete data that exists on the server

---

![Sandwich Builder](https://i.imgur.com/Q1q6Ngd.jpg)

You are on a team for a company called Sandwich King! They plan on placing snack-machine style sandwich builders all around the city, and need an API for available ingredients to select from. Here is the original data set:

```js
const ingredients = [
  { type: "bread", items: ["white", "wheat", "sourdough", "rye", "multigrain"] },
  { type: "meat", items: ["turkey", "ham", "roast beef", "chicken", "bacon", "salami"] },
  { type: "cheese", items: ["cheddar", "swiss", "provolone", "mozzarella", "pepper jack", "Muenster"] },
  { type: "veggies", items: ["lettuce", "tomato", "onion", "cucumber", "bell pepper", "spinach", "avocado"] },
  { type: "condiments", items: ["mayonnaise", "mustard", "ketchup", "relish", "hot sauce", "ranch dressing"] }
];
```

Things such as "Bread", "Cheese", "Condiments" are all Ingredient Types. Things like "Cheddar", "Salami", "Ketchup" are the ingredients.

Your task is to create a server with routes to perform the following actions:

- `R`ead all available ingredients for all ingredient types
- `R`ead all available ingredients for ONE ingredient type (Hint: Use Query Parameters or Dynamic Parameters)
- `C`reate a new ingredient (Hint: Use Dynamic Parameters for the ingredient type and the request body to accept the new data)
- `U`pdate the ingredients list for one ingredient type, i.e., replace the ingredients list with a new list (Hint: Use Dynamic Parameters for the ingredient type and the request body to accept the new list)
- `D`elete an ingredient (Hint: Use Dynamic Parameters to know which ingredient to remove, and optionally a Query Parameter or second Dynamic Parameter to narrow down which ingredient type it's in)
