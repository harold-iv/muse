# muse 🎧

[![deploy](https://github.com/GrantBirki/muse/actions/workflows/deploy.yml/badge.svg)](https://github.com/GrantBirki/muse/actions/workflows/deploy.yml) [![Unlock On Merge](https://github.com/GrantBirki/muse/actions/workflows/unlock-on-merge.yml/badge.svg)](https://github.com/GrantBirki/muse/actions/workflows/unlock-on-merge.yml)

A self-hosted version of [muse](https://github.com/codetheweb/muse).

## Commands 💻

Here is a table of all commands that are available to use:

> Note: Many commands have optional arguments. View more details about a command by starting to type the command

| Command | Description |
| ------- | ----------- |
| `/play <query>` | Play a song or playlist from YouTube or Spotify |
| `/next` | Skip to the next song |
| `/stop` | Stop playback, disconnect, and clear all songs in the queue |
| `/clear` | Clears all songs in the queue except the currently playing song |
| `/now-playing` | Show the currently playing song |
| `/disconnect` | Pause and disconnect |
| `/favorites create` | Create a new favorite |
| `/favorites list` | List all favorites |
| `/favorites remove` | Removes a favorite |
| `/favorites use` | Favorites use |
| `/fseek <time>` | Seek forward to a time in the current song |
| `/loop` | Toggle looping of the current song |
| `/move <from> <to>` | Move songs within the queue |
| `/queue` | Show the current queue |
| `/remove <index>` | Remove songs from the queue |
| `/replay` | Replay the current song |
| `/resume` | Resume playback |
| `/seek <time>` | Seek to a position from the begining of the song |
| `/shuffle` | Shuffle the current queue |
| `/skip` | Skip the next song or songs depending on your inputs |
| `/unskip` | Go back in the queue by one song |

## Features ⭐

- 🎥 Livestreams
- ⏩ Seeking within a song/video
- 💾 Local caching for better performance
- 📋 No vote-to-skip - this is anarchy, not a democracy
- ↔️ Autoconverts playlists / artists / albums / songs from Spotify
- ↗️ Users can add custom shortcuts (aliases)
- 🔊 Normalizes volume across tracks

## Updating 📦

To update the version that is deployed, do the following:

- Go to the upstream [releases page](https://github.com/codetheweb/muse/releases) and find the latest version (e.g. `v2.4.3`)
- Open the [`docker-compose.yml`](./docker-compose.yml) file and change the `image` field of the `muse` service to the new version (e.g. `codetheweb/muse:2.4.3`) - note: we leave out the `v` prefix here
- Open a pull request with your changes
- Once approved, comment `.deploy` on your PR to deploy the new version to production
- If all goes well, merge the pull request
- ✅ Done!
