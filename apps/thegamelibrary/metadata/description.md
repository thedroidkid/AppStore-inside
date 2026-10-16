# The Game Library

A self-hosted web app for tracking a personal game collection. Add and edit games, sort by title or platform, search TheGamesDB when you provide an API key, or enter game details and upload cover art manually.

## Features

- Add, edit, and remove games from the web interface.
- Track platform, release year, status, description, and notes.
- Sort the library by title or platform and filter by title or status.
- Optionally search TheGamesDB for game details and cover art.
- Upload a personal JPEG, PNG, or WebP cover (up to 12 MB).
- Store the library and covers persistently when running in Docker.

## Requirements

- Docker Engine and the Docker Compose plugin.
- A TheGamesDB API key only if you want catalog search. Manual game entry and cover uploads work without one.
