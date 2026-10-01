# Changelog

All notable changes to Internet Download Hub Pro are recorded here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
Each release's notes are taken from its section below, so every version that is
tagged needs one.

## [Unreleased]

## [2.0.0] - Unreleased

The first release of Internet Download Hub Pro. It builds on the free
Internet Download Hub 1.3.2 and adds a Firefox add-on that finds and catches
downloads in the browser, the way IDM does.

### Added

- **A Firefox add-on that finds the video on the page you are watching.**
  Point at a video and a "Download this video" bar appears; it lists the
  qualities the site really offers and sends the one you pick to the app. It
  finds HLS and DASH streams, whole media files and `<video>` elements, and
  skips stream segments and ads so the list stays short. It keeps up with sites
  that change page without reloading.
- **Firefox downloads go to the app.** When Firefox starts downloading a file
  of a type you chose (archives, installers, PDFs, video and more), the app
  takes it over, with progress, pause and resume. Turn it on or off, and pick
  the types, in the add-on's settings.
- **Streams that only their own page may fetch now download.** For that one
  download, the add-on passes the app what the browser sent with it: the page
  address, the browser's identity and that site's cookie. The cookie is used
  for that download only, never written to the log, and deleted afterwards.
- **Files are named after the page**, not after the stream (no more
  `master.mp4`).
- The add-on talks only to the app on your own PC, after a one-time pairing you
  allow in the app.

### Changed

- **A new, compact interface.** One screen holds the link bar and your
  downloads, with filters (All, Active, Finished, Failed), multi-select and
  actions for several downloads at once. Supported Sites moved to
  the Help menu.
- Playlists list one video per line, so long playlists are quick to scan.
- Installs beside the free Internet Download Hub, with its own settings and
  history.

### Fixed

- A short network hiccup that the engine retried on its own is no longer shown
  as a failed download.
- New downloads appear in the list straight away, without switching tabs.
- "Loading more…" stops once a playlist has finished loading.
- Direct file downloads show their progress, speed and time left.
