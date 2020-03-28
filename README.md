### Restaurant Menu

In this exercise, your best friend is opening a restaurant and needs your help with the site, particularly showcasing the menu. Use the text messages from your friend to create and modify your menu object.

Copy and paste the below JS and follow the prompts (these appear as "text messages" from your friend). Create an HTML file and link this file using `<script src="">` tags.

let menuItem = {
  name: 'Kale Caesar Salad',
  nickName: 'All Hail Kale',
  referenceID: 'SLD001',
  description: 'Kale is king in this hearty, flavorful salad that pays homage to the traditional - but with a healthy twist',
  highInCalories: false,
  ingredients: ['Kale', 'Caesar dressing', 'Anchovy paste', 'Grilled corn', 'Parmesan cheese', 'Croutons'],
  numIngredients: function() {
    return this.ingredients.length;
  }
}
// START HERE
// TEXT 1: Howdy friend!  Thanks sooo much for doing this. I'm thinking this all out loud, so be
// patient with me.  Here's the work I attempted so far, but I need your help to get this right.
// It would be nice to track the year I added the dish to my menu. My salad was added in 2017.

// TEXT 2: Although we provide breakfast, lunch, and dinner, not all dishes are available around the clock.
// Please add something to track which menu the dish will be featured on. The Caesar salad is for
// lunch and dinner

// TEXT 3: Yikes! When I first did the menu, I broke dishes down to low and high in calories.  I don't
// like this anymore, so can you remove it and change it to the number of calories?
// The salad stands at 560 calories

// TEXT 4: Don't you think the nickname is stupid?  Remove it.  Sooo not needed.

// TEXT 5: OMG!  I forgot to add lemon juice to the list of ingredients.  Can you add this?

// **WILL PRINT key/value pairs for menuItem
console.log("\n\n******menuItem Object******");
Object.entries(menuItem).forEach(([key, value]) => {
  if (key != 'numIngredients')
    console.log(`${key}: ${value}`)
  });
console.log(`Number of ingredients = ${menuItem.numIngredients()}`);
