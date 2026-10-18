# NostalgiaTV Server

A self-hosted companion server for the NostalgiaTV Android app. Build a live TV guide from Plex, Jellyfin, and Emby libraries, watch from a browser, and use the built-in HDHR/IPTV tuner with DVR apps.

## Features

- Connect multiple Plex, Jellyfin, and Emby servers.
- Build per-profile schedules up to 30 days ahead.
- Manage channels, commercials, and profiles from the browser.
- Expose an HDHR tuner, M3U playlist, and XMLTV guide for compatible DVR apps.

## Setup

Open `http://<server>:19850` to sign in and configure your media servers. The same address can be used by the NostalgiaTV Android app and DVR clients on your network.

The server's timezone and container user/group IDs can be set in the app configuration. The user and group IDs should have permission to write to the app's persistent data directories.

## Persistent data

- `data/` stores server data.
- `config/` stores server configuration.
- `logos/` stores channel logos.

The image is pulled from `purestream711/nostalgiatv-server:latest` and supports `amd64` and `arm64`.
