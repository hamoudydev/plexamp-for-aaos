# Unofficial Plex client for Android Automotive

This app is a Plex music client for Android Automotive.

The application is available in the [Play Store](https://play.google.com/store/apps/details?id=us.berkovitz.plexaaos)

## Features

### Music Browsing
- **Playlists** - Browse and play your Plex playlists
- **Artists** - Browse all artists, view their albums, and play tracks
- **Albums** - Browse all albums and play tracks

### Playback
- Background playback with media notification
- Shuffle and repeat modes (persisted between sessions)
- Resume playback from last position
- Track prefetching for seamless playback

### Offline Support
- Automatic caching of recently played tracks
- Works with intermittent connectivity

## Browse Hierarchy

```
Root
├── Playlists
│   └── [Playlist] → Tracks
├── Artists
│   └── [Artist] → [Albums] → Tracks
└── Albums
    └── [Album] → Tracks
```

## Screenshots

*Coming soon*

## Requirements

- Android Automotive OS (Android 10+)
- Plex Media Server with music library
- Plex account

## Changelog

### v0.8.0 (Unreleased)
- Added Artists browsing - view all artists, their albums, and tracks
- Added Albums browsing - view all albums and their tracks
- New icons for Artists and Albums categories
- Playback support for album-based track selection

### v0.7.2
- Artist name now uses `originalTitle` if present

### v0.7.1
- Remember shuffle and repeat modes between sessions

### v0.7.0
- Added offline playback support
- Track prefetching for better streaming experience

## TODOs

- Multi-server support
- Multi-user support
- Relay fallback when direct connect fails
- Improved login logic
- ~~Support for music selection other than playlists~~ ✓ Implemented

## Building

1. Clone the repository
2. Create `local.properties` with your signing key configuration
3. Build with Android Studio or `./gradlew assembleRelease`

## Dependencies

- [kotlin-plexapi](https://github.com/joeyberkovitz/kotlin-plexapi) - Plex API client library
- ExoPlayer - Media playback
- Glide - Image loading

## License

Apache 2.0

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
