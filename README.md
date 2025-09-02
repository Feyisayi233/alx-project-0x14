# MoviesDatabase API – Developer Overview

## API Overview
The **MoviesDatabase API** provides complete and updated data for over **9 million titles**, including movies, series, and episodes.  
- **Weekly updates** for new titles  
- **Daily updates** for ratings and episode data  
- Rich models covering titles, actors, ratings, episodes, and metadata  
- Flexible query parameters for filtering, sorting, and customizing responses  

This makes it a powerful tool for developers building movie, TV, or media-related applications.

---

## Version
Current version: **v1** (latest public release).

---

## Available Endpoints

### Titles
- **`/titles`** – Returns an array of titles based on filters/sorting.  
- **`/x/titles-by-ids`** – Fetch multiple titles by IMDb IDs.  
- **`/titles/{id}`** – Fetch details for a single title by IMDb ID.  
- **`/titles/{id}/ratings`** – Get rating and votes for a title.  
- **`/titles/series/{id}`** – Returns all episodes (with IDs, season, and episode numbers).  
- **`/titles/seasons/{id}`** – Returns the total number of seasons for a series.  
- **`/titles/series/{id}/{season}`** – Get episodes for a specific season.  
- **`/titles/episode/{id}`** – Fetch detailed data for a single episode.  
- **`/titles/x/upcoming`** – Upcoming movies and series.  

### Search
- **`/titles/search/keyword/{keyword}`** – Search titles by keyword.  
- **`/titles/search/title/{title}`** – Search titles by exact or partial title.  
- **`/titles/search/akas/{aka}`** – Search titles by an alternative known-as title.  

### Actors
- **`/actors`** – Returns a list of actors (supports pagination).  
- **`/actors/{id}`** – Fetch full details for a specific actor.  

### Utils
- **`/title/utils/titleType`** – Get all available title types.  
- **`/title/utils/genres`** – Get all genres.  
- **`/title/utils/lists`** – Predefined title lists (e.g., top box office, top rated).  

---

## Request and Response Format

### Base URL
