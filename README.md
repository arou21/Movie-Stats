Movie Comparison App
This project is a movie comparison app that allows you to search for movies and compare their details side by side. It uses the Open Movie Database (OMDb) API to fetch movie data and displays it in a user-friendly format.

Features
Search for movies using a search term.
View search results with movie title and release year.
Compare two selected movies side by side based on various statistics such as awards, box office revenue, Metascore, IMDb rating, and IMDb votes.
Highlight the higher value in the comparison with a warning color.
How it Works
The main functionality of the app is implemented in the index.js file. Here's a breakdown of the key parts of the code:

autoCompleteConfig: This is a configuration object that contains methods to render search results, format the input value, and fetch movie data using the OMDb API.

createAutoComplete: This function is used to create an autocomplete widget for movie search. It takes the autoCompleteConfig as well as the root element where the autocomplete should be attached and an onOptionSelect callback to handle movie selection.

onMovieSelect: This asynchronous function is called when a movie is selected from the autocomplete search results. It fetches detailed information about the selected movie using the OMDb API and updates the summary element with the movie details. It also stores the selected movie information based on the side of comparison (left or right).

runComparison: This function compares the movie statistics of the selected movies and highlights the higher value with a warning color.

movieTemplate: This function generates an HTML template for displaying detailed movie information, such as movie title, genre, plot, awards, box office revenue, Metascore, IMDb rating, and IMDb votes.

Getting Started
Clone this repository to your local machine using the following command:

bash
Copy code
git clone https://github.com/arou21/Maze.git
Open the index.html file in your web browser to view the movie comparison app.

Enter the name of a movie in the search box to see the autocomplete results.

Select two movies from the autocomplete results to compare their details side by side.

Dependencies
Materialize CSS: The CSS framework used for styling the app.

axios: A popular JavaScript library for making HTTP requests, used to fetch data from the OMDb API.

License
This project is licensed under the MIT License. Feel free to use and modify it as needed.
