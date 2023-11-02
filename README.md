# module5
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Web App</title>
    <script>
        // Modified code to send the user to a random category
        function redirectToRandomCategory() {
            // Get a list of available categories (customize this list as needed)
            var categories = ["Lunch", "Dinner", "Sushi", "Appetizers", "Desserts"];

            // Generate a random index to select a category
            var randomIndex = Math.floor(Math.random() * categories.length);

            // Get the random category short_name
            var randomCategory = categories[randomIndex];

            // Redirect the user to the random category (simulate the behavior)
            alert("Redirecting to: " + randomCategory);
        }
    </script>
</head>
<body>
    <div id="menu-tile">
        <a href="#">Menu</a>
    </div>
    <div id="specials-tile">
        <!-- Add an event listener to the Specials tile -->
        <a href="#" onclick="redirectToRandomCategory()">Specials</a>
    </div>
    <div id="map-tile">
        <a href="#">Map</a>
    </div>
</body>
</html>


   


