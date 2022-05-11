# Recruitment Python Django task

Hello,

This is the recruitment test for the position of Python Developer at Accent. Please read the instructions carefully and send us back the link with a solution.

### Specification

We’d like you to build a simple REST API for us - a basic movie database interacting with an external API. Here’s the full specification of endpoints that we’d like it to have:

* `POST /movies`:
  * The request body should contain only the movie title, and its presence should be validated.
  * Based on the passed title, other movie details should be fetched from http://www.omdbapi.com/ (or other similar, public movie database) - and saved to the application database.
  * Request response should include a complete movie object and all data fetched from external API.
* `GET /movies`:
  * Should fetch a list of all movies already present in the application database.
  * Additional filtering and sorting are optional, but some implementation is a bonus.
* `POST /comments`:
  * The request body should contain the ID of the movie already present in the database and the comment text body.
  * Comment should be saved to the application database and returned in the request-response.
* `GET /comments`:
  * Should fetch a list of all comments present in the application database.
  * Should allow filtering comments by associated movie, bypassing its ID.

### Rules & hints

* Your goal is to implement REST API in Django. However, you're free to use any third-party libraries and database of your choice - sharing your reasoning behind choosing them is welcome!
* At least basic tests of endpoints and their functionality are obligatory. Their exact scope and form are left up to you.
* The application's code should be kept in a public repository so that we can read it, pull it and build it ourselves. Remember to include a README file or at least introductory notes on application requirements and setup - we should be able to easily and quickly get it running.

**Good luck! If you have any questions feel free to ping us!**