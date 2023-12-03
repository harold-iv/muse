# muse 🎧

[![deploy](https://github.com/GrantBirki/muse/actions/workflows/deploy.yml/badge.svg)](https://github.com/GrantBirki/muse/actions/workflows/deploy.yml) [![Unlock On Merge](https://github.com/GrantBirki/muse/actions/workflows/unlock-on-merge.yml/badge.svg)](https://github.com/GrantBirki/muse/actions/workflows/unlock-on-merge.yml)

A self-hosted version of [muse](https://github.com/codetheweb/muse).

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
