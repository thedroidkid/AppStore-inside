# AppStore-inside

AppStore-inside is a custom app store for [Runtipi](https://runtipi.io), maintained by DroidKid. It contains the following apps:

| App | Description |
| --- | --- |
| [The Game Library](apps/thegamelibrary) | A self-hosted web app for tracking a personal game collection. |
| [NostalgiaTV Server](apps/nostalgiatv-server) | A self-hosted live TV guide and tuner for Plex, Jellyfin, and Emby libraries. |
| [Surveillance](apps/surveillance) | A web interface for managing and viewing RTSP video streams. |

## Using the app store

Add this repository as a custom app store in your Runtipi instance. See the [Runtipi guide to creating and using custom app stores](https://runtipi.io/docs/guides/create-your-own-app-store) for the current setup instructions.

After adding the store, install and manage its apps from the Runtipi interface. Check each app's description and configuration for its requirements and available options.

## Repository structure

Each directory in `apps/` contains one app:

```text
apps/<app-id>/
├── config.json
├── docker-compose.yml
└── metadata/
    ├── description.md
    └── logo.jpg
```

- `config.json` defines the app's Runtipi metadata and settings.
- `docker-compose.yml` defines its container service.
- `metadata/` contains the app description and logo shown in the store.

## Development

Install the dependencies and run the app-store tests with [Bun](https://bun.sh/):

```sh
bun install
bun test
```

To add an app, create a directory under `apps/` with its configuration, Docker Compose file, and metadata. Run the tests before submitting changes.
