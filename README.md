# Movie Mania

Welcome to Movie Mania! This is a React project that allows you to explore, bookmark and watch different movies.

## Live Link

You can access the live version of this project [here](https://movie-mania-original.netlify.app/).

## Installation

To run this project locally, follow these steps:

1. Clone the repository.
2. Navigate to the `movie-mania` directory.
3. Install the dependencies by running the command `npm install`.
4. Start the development server with `npm run dev`.

# Server Setup

The server for this project is written in Python and uses Flask. Follow these steps to set it up:

1. Navigate to the `src` directory.
2. Create a virtual environment: `python3 -m venv venv`
3. Activate the virtual environment: `source venv/bin/activate` (on Unix or MacOS) or `.\venv\Scripts\activate` (on Windows)
4. Install the dependencies: `pip install -r requirements.txt`
5. Start the server: `python app.py`

The server will start on `localhost:5000` by default.

## API Endpoints

The server provides several API endpoints for interacting with the movie data:

- `PUT /movies/<id>`: Update a favorite movie. This endpoint requires a JSON body with the movie data, and it returns a message indicating whether the update was successful. See [`update_favorite`](src/routes.py) in [src/routes.py](src/routes.py) for more details.

Please refer to the [Swagger documentation](src/static/swagger.json) for more information about the API endpoints.

## Database

The server uses a SQLite database for storing movie data. The database is set up in [src/database/db.py](src/database/db.py) and [src/database/movie.py](src/database/movie.py).

## Features

- Trending Page: Explore the latest trending movies and see what's popular among users. Get access to a curated list of movies that are currently generating buzz in the film industry. Stay up-to-date with the latest releases and discover new movies to watch.
- Genres Page: Explore movies based on different genres. Browse through a wide range of genres such as action, comedy, drama, horror, romance, and more. Get recommendations and discover movies that match your preferred genre. Dive into the world of cinema and find movies that cater to your specific interests.
- Search Page: Use the search feature to find specific movies based on title, genre, or any other relevant criteria. Enter keywords or filters to narrow down your search and get accurate results. Find movies that match your preferences and explore a vast collection of films from various genres and languages.
- Upcoming Page: Get a sneak peek into the future of cinema with the Upcoming Page. Discover upcoming movies that are set to release soon and stay ahead of the curve. Find out about the latest trailers, release dates, and plot details of highly anticipated movies. Stay informed about the upcoming releases and plan your movie-watching schedule in advance.
- Favorites Page: Keep track of your favorite movies with the Favorites Page. Bookmark movies that you love and easily access them whenever you want. Create a personalized collection of movies that you can revisit anytime. Never miss out on your favorite films again.
- Bookmark Option: With the bookmark option, you can save movies to your favorites list. Simply click on the bookmark icon next to a movie and it will be added to your collection. This allows you to easily find and watch your favorite movies without having to search for them again.
- Dark Theme: Movie Mania also offers a dark theme option for a more visually pleasing and comfortable viewing experience. Switch to the dark theme to reduce eye strain and enjoy the movies in a sleek and stylish interface. The dark theme is perfect for watching movies in low-light environments or for users who prefer a darker aesthetic. Simply toggle the dark theme option in the settings to enable this feature.

## License

This project is licensed under the [MIT License](LICENSE).
