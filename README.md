# NYT-Goodreads-Map

We will make a map showing the New York Times Bestselling authors for the "Combined Print & E-Book" category since its inception in February 2011.

It works in the following order:

1. ** nyt-bestseller-scrape.ipynb ** scrapes the NYT bestseller titles along with names of authors, book description, ranking, and how many weeks the book has been on the list.
2. ** scraping-goodreads-books.ipynb ** scrapes these books and author links from goodreads along with the rating of the book and the number of readers who reviewed the book.
3. ** scraping-goodreads-authors.ipynb ** goes to the author URLs we scraped in the previous version and gets the authors' place of birth
4. ** geolocating_authors.ipynb ** uses the Google Maps API to find the cooridnates of the authors' birthplaces to build our map
5. ** data_cleaning.ipnyb ** cleans the text of the columns
6. ** mapbox-data-prep.ipynb ** aggregates the data and prepares it for the map
7. The subfolder ** Maps Stuff ** contains the final data files and html to create the map 
