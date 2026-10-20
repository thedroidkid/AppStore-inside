# The Game Library

A self-hosted web app for tracking a personal game collection. Add and edit games, import game titles from a text file, export the library to CSV, or search TheGamesDB when you provide an API key.

## Features

- Add, edit, and remove games from the web interface.
- Click a game's title or cover to view its details and edit it.
- Track platform, release year, status, description, and notes.
- Sort by title or platform and filter by title, status, or platform.
- Import game titles from a `.txt` file, assign a platform, review the preview, and confirm before saving.
- Detect and skip duplicate title/platform pairs during import.
- Export the full library to a spreadsheet-friendly CSV file.
- Optionally search TheGamesDB for game details and cover art.
- Upload a personal JPEG, PNG, or WebP cover (up to 12 MB).
- Store the library and covers persistently when running in Docker.

## Requirements

- Docker Engine and the Docker Compose plugin.
- A TheGamesDB API key only if you want catalog search. Manual game entry and cover uploads work without one.
