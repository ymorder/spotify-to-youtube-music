# Spotify to YouTube Music

A single-page browser tool for moving your Spotify playlists and podcasts to YouTube Music.

**Status: unfinished prototype.**

- It lists your Spotify playlists and podcasts and searches YouTube for a match. It doesn't create playlists on YouTube yet.
- It signs in to Spotify with the old implicit flow (`response_type=token`), which Spotify has dropped. Sign-in needs to move to Authorization Code with PKCE before the tool can work.

## Setup

1. Create an app at [developer.spotify.com/dashboard](https://developer.spotify.com/dashboard).
2. Create a Google Cloud project and turn on YouTube Data API v3.
3. Put both client IDs at the top of the script in `index.html`, and add your page's address as a redirect URI in both services.
4. Serve the folder from a local web server and open the page. Opening the file directly won't work with sign-in.

## Files

- `index.html`: the whole app (HTML, CSS and JavaScript).
