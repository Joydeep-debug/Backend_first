## Movie Database Query Checklist

### Overview
This Node.js utility provides functions to query a movie database using Mongoose. It supports retrieving movies by title, fetching all movies, and searching movies by director name. The utility connects to the database through an initialization module.



### Goals
:ballot_box_with_check: Enable retrieval of a single movie by its title.
:ballot_box_with_check: Allow fetching all movies stored in the database.
:ballot_box_with_check: Allow fetching all movies directed by a specific director.
:ballot_box_with_check: Log the results of the database queries to the console.
:ballot_box_with_check: Gracefully handle and log errors during the database operations.


#### Functional Requirements
:ballot_box_with_check: Database Initialization
                        :ballot_box_with_check: Initialize and connect to the MongoDB database using `initializeDatabase()` from `./db/db.connect`.

:ballot_box_with_check: Model Utilization
                        :ballot_box_with_check: Use the `Movie` model from `./models/movie.models` to perform queries.

 :ballot_box_with_check: QueryFunction 
     1. `readMovieByTitle(movieTitle)`
        :ballot_box_with_check: If the movie is found, print the movie object to the console; else, handle errors gracefully.
     2. `readAllMovies()`
        :ballot_box_with_check: Fetch all movies; print them to the console.


     3. `readMovieByDirector(directorName)`
         :ballot_box_with_check: Query all movies by director; print the resulting array to the console.
     

### Error Handling
  :ballot_box_with_check: All database operations should be wrapped in try-catch blocks.
  :ballot_box_with_check: Errors should be logged or thrown appropriately to aid debugging.