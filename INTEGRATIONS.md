# Spotify & YouTube integrations

The included MVP is fully usable without API credentials. The external publishing buttons are intentionally safe placeholders until you create your own developer applications.

## Spotify
Create a Spotify Developer application, configure your exact redirect URI, and use OAuth Authorization Code with PKCE. Request only playlist scopes you need, such as `playlist-modify-public` and `playlist-modify-private`.

Never put a client secret in browser JavaScript.

## YouTube
Create a Google Cloud project, enable YouTube Data API v3, configure OAuth consent, and request the minimum permission needed to create playlists/add videos.

Keep credentials and token exchange logic out of GitHub.

## Why this is separate
Real OAuth integrations require provider-side credentials, redirect URLs and consent configuration. The local MVP therefore works first instead of pretending to contain working credentials.
