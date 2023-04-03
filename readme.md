## Movie Ticketing System
This project is a simple movie ticketing system that allows users to view information about movies and purchase tickets.

## Features
Displays information about the first movie in the database, including its poster, title, description, runtime, and showtime.
Displays the number of available tickets for the first movie.
Allows users to purchase tickets for the first movie by clicking a button.
Updates the number of available tickets and displays a “SOLD OUT” message when all tickets have been sold.
Sends a PATCH request to the server to update the number of tickets sold for the first movie.
Usage
To use this project, you will need to have a local server running on port 3000 that serves data from the /films endpoint. The data should be an array of objects representing movies. Each object should have properties for id, poster, title, description, runtime, showtime, capacity, and tickets_sold.

Once you have the server set up, open the index.html file in your web browser. You should see information about the first movie in the database and be able to purchase tickets by clicking the “Buy Ticket” button.

## Code Explanation
The code uses an event listener to wait for the DOMContentLoaded event before calling the moviePlace function. This function uses the fetch() function to send a GET request to the /films endpoint of a local server running on port 3000. The response is then converted to a JSON object and used to update elements on the page with information about the first movie in the database.

An event listener is also added to the “Buy Ticket” button that listens for click events. When this button is clicked, the number of available tickets is decreased by one and updated on the page. If all tickets have been sold, a “SOLD OUT” message is displayed. A PATCH request is also sent to the server to update the number of tickets sold for the first movie.
## Author
Ronald Barasa ron-nieb