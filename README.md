# module5
// Original code to send the user to the "Specials" category
function redirectToSpecials() {
  $dc.loadMenuCategories("Specials");
}

// Modified code to send the user to a random category
function redirectToRandomCategory() {
  // Get a list of available categories (you may need to fetch this data)
  var categories = ["Lunch", "Dinner", "Sushi", "Appetizers", "Desserts"];

  // Generate a random index to select a category
  var randomIndex = Math.floor(Math.random() * categories.length);

  // Get the random category short_name
  var randomCategory = categories[randomIndex];

  // Redirect the user to the random category
  $dc.loadMenuCategories(randomCategory);
}

// Attach the modified click event handler to the Specials tile
document.getElementById("specials-tile").addEventListener("click", redirectToRandomCategory);

   


