# Internet Download Hub Pro

A download manager for Windows that works with Firefox. Point at a video on
almost any site and download it in the quality you choose, or let the app take
over the files Firefox starts downloading, with progress, pause and resume.

> **Not released yet.** The first version, 2.0.0, is being prepared. Installers
> and updates will be published on this repository's
> [Releases page](https://github.com/Isaac-Onyango-Dev/Internet-Download-Hub-Pro/releases).
> This repository holds releases only; the source code is private.

## What it does

- **Finds the video on the page you're watching.** With the Firefox add-on,
  point at a video and a "Download this video" bar appears. It lists the
  qualities the site actually offers; pick one and the app downloads it.
- **Downloads streams other tools can't reach.** Some sites only let their own
  page fetch a video. For that one download, the add-on passes the app what
  your browser sent with it, including that site's cookie. The cookie is never
  written to the app's log and is deleted afterwards.
- **Takes over Firefox downloads.** Archives, installers, PDFs, video and the
  other types you choose go to the app instead of Firefox, so you can pause and
  resume them.
- **Names files after the page**, not after the stream.
- **Downloads from 1000+ sites** with bundled engines (yt-dlp, FFmpeg,
  streamlink, gallery-dl, N_m3u8DL-RE). Nothing else to install.
- One compact window: paste a link, pick a quality, and watch your downloads
  in one list with filters and multi-select.

## Requirements

- Windows 10 or 11, 64-bit.
- Firefox, for the add-on. The app also works on its own: paste a link into it.

## Installing

1. Download `Internet-Download-Hub-Pro-Setup-X.Y.Z.exe` from the
   [latest release](https://github.com/Isaac-Onyango-Dev/Internet-Download-Hub-Pro/releases/latest).
   If your browser says the file isn't commonly downloaded, choose to keep it.
2. Open it. Windows will stop it with a blue panel (see below): click
   **More info**, then **Run anyway**.
3. Follow the installer, then open **Internet Download Hub Pro** from the Start
   menu or the desktop.
4. Install the Firefox add-on, then allow the connection when the app asks. The
   add-on's Firefox Add-ons link will be added here when it is listed.

Pro installs beside the free Internet Download Hub; you can keep both.

### "Windows protected your PC"

The installer is not code-signed, so Windows SmartScreen shows this the first
time you open it:

> **Windows protected your PC**
>
> Microsoft Defender SmartScreen prevented an unrecognized app from starting.
> Running this app might put your PC at risk.

Only **Don't run** is offered at first. To install:

1. Click **More info** under the message.
2. Check the two lines that appear: **App:**
   `Internet-Download-Hub-Pro-Setup-X.Y.Z.exe` and **Publisher:** Unknown
   publisher.
3. Click **Run anyway**.

"Unknown publisher" is expected: the file carries no code-signing certificate.
Download it only from this repository's Releases page. If Windows says it
*blocked* the app and offers no **Run anyway** button, Smart App Control is on,
and it does not allow unsigned apps.

## Updates

The app checks this repository for new versions: **Help → Check for Updates**.
What changed in each version is in the [changelog](CHANGELOG.md).

## Help

- Something not working? [Open an issue](https://github.com/Isaac-Onyango-Dev/Internet-Download-Hub-Pro/issues/new).
  Say which site, and attach the log from **Help → Open Log File** if you can.
- Looking for the free version? It's at
  [Internet Download Hub](https://github.com/Isaac-Onyango-Dev/Internet-Download-Hub).

Download only what you have the right to download.

## Licence

Internet Download Hub Pro is proprietary software. © 2026 Isaac Onyango.
All rights reserved. Use of the app is governed by its
[End User License Agreement](EULA.txt), which the installer also shows.
It also explains what the Firefox add-on sends to the app (section 11).
