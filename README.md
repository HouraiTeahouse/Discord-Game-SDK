# Discord Game SDK for Unity

<p align="center">
    <a href="https://discordapp.com/developers/docs/game-sdk/sdk-starter-guide">
        <img src="https://img.shields.io/badge/docs-passing-brightgreen.svg" alt="Docs">
    </a>
    <a href="https://discord.gg/discord-gamesdk">
        <img src="https://discordapp.com/api/guilds/151219753434742784/widget.png" alt="Offiical Discord Server">
    </a>
</p>

The [Discord Game SDK](https://discordapp.com/developers/docs/game-sdk/sdk-starter-guide)
repackaged as a Unity Package. For API documentation, please refer to the
official Discord API docs.

This package is up to date with the official SDK as of September 16th, 2020.

## Info

> The SDK is currently under extensive development and is subject to change. Suggestions
> about the current API are welcome.

### Setup

- Create an application on the Discord [developer site](https://discordapp.com/developers/applications/me).
- Set a redirect URL. If you don't have one right now, just use <http://127.0.0.1>.
- Enable Rich Presence for the application. This enables whitelist access for the SDK.
  - When you are ready to test with more people, add them to the whitelist.
- Copy the **Client ID**.
  - Use this `CLIENT_ID` when initializing the SDK.

## Installation

Installation of this package requires Unity 2018.3 or higher.

Under `Packages/manifest.json`, add the following lines, then open the Unity
Editor. Note: this will add a scoped registry to your project.

```json
{
  "dependencies": {
    "com.discord.game-sdk": "2.5.6"
  },
  "scopedRegistries": [
    {
      "name": "Hourai Teahouse",
      "url": "https://upm.houraiteahouse.net",
      "scopes": ["com.discord"]
    }
  ]
}
```

## License

As of time of writing (November 27th 2019), the Discord Game SDK is not considered
FOSS.  Thus this repository has no LICENSE file.  This repo is meant to be a
direct mirror to make it easier to import into Unity and includes pre-built
binary distributions of the package in it's source.

Note that if this third-party distribution of the SDK is not in line with
Discord's Terms of Service, it will be taken down.
