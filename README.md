# IGDB Video Game Database API
Video Game Data Analysis – Early Release Popularity.
# API Overview and Purpose:
•	The IGDB API is free for non-commercial usage.

•	This API taps into complete, holistic, accurate and an up-to-date data representation of the video game market, it’s game products and consumer opinions.

•	This project gathers data from the IGDB API to aggregate all games, no matter which platform.   The data includes popularity by region, release date and game type such as First Person Shooter, Top-Down Strategy and many more.

•	Our main objective was to find out which video game titles were most popular during the early-access phase regardless of region, platform, genre and game style.


# Installation/Setup/Usage:

•	Using a “Client ID and a “Client Secret”, we gained access to this API as a “Twitch Developer”. We crafted a custom POST request to the endpoint and obtained an authentication token from the streaming platform TWITCH.  We then used that token to pass POST and GET requests to the Internet Games Database API (IGDB).

•	The data was then received in JSON format which we then converted to DataFrames using Python and Pandas Jupyter Notebook.

•	Most of the requests to the API use the POST method.  Using the base URL, we defined which endpoint to query by appending /{endpoint name} to the base URL.  We included the CLIENT ID and ACCESS TOKEN in the HEADER of the request.  This was obtained in the JSON data received in the request and response we received initially.


# Endpoints and Documentation:

•	https://api.igdb.com/v4/age_ratings - Age Rating according to various rating organisations

•	https://api.igdb.com/v4/age_rating_content_descriptions - Age Rating Descriptors

•	https://api.igdb.com/v4/companies - Video game companies. Both publishers & developers

•	https://api.igdb.com/v4/games - Video games

•	https://api.igdb.com/v4/game_modes - Single player, Multiplayer etc

•	https://api.igdb.com/v4/genres - Genres of video games

•	https://api.igdb.com/v4/involved_companies - Companies involved in the creation/publication of the games

•	https://api.igdb.com/v4/platforms - The hardware used to run the game or game delivery network

•	https://api.igdb.com/v4/platform_version_release_dates - Platform release dates, platforms and versions

•	https://api.igdb.com/v4/regions - The region for game localization

•	https://api.igdb.com/v4/release_dates - Platform release dates, platforms and versions


# Data Models Created:

•	Game mode summary using “value counts” (Python/Pandas)

•	Genre summary using “value counts” (Python/Pandas)

•	Release date summary “value counts” (Python/Pandas)

•	Platform summary “value counts” (Python/Pandas)

•	Region summary “value counts” (Python/Pandas)

•	Developer summary “value counts” (Python/Pandas)

•	Publisher summary “value counts” (Python/Pandas)


# Data Visualizations Created:

•	Bin the average score rating into human-readable grades using the “binning” option in Python/Pandas

•	Summarized the number of games according to grades

•	Grouped “Very High” graded games by the number of games per region

•	Generated a Pie Graph for Top Rated Games by Region

•	Grouped all games by region

•	Generated a Pie Graph for Games by Region

•	Generated a Stacked Bar Graph for Genres and Average Score

•	Generated a Stacked Bar Graph representing the Number of Games by Genre

•	Generated a Stacked Bar Graph for Game Modes and Average Score

•	Generated a Stacked Bar Graph for Number of Games by Game Modes

•	Generated a Scatter Plot to show the Developer Experience and Average Score using Linear Regression calculations

•	Generated a Scatter Plot to show the Publisher Experience and Average Score using Linear Regression calculations
