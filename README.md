# music-brainstorming-bgm

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A collection of AI-generated instrumental tracks designed to aid focus and creativity during brainstorming sessions. This repository provides a web-based music player to listen to the tracks and browse the prompts used to create them.

## Demo

[**▶️ Listen in your browser**](https://code4fukui.github.io/music-brainstorming-bgm/)

The player features a three-panel interface showing the playlist, the current track's album art with audio controls, and the AI generation prompt.

## Features

- **Web-Based Player**: A simple, static HTML player that runs in any modern browser.
- **AI Prompt Display**: Shows the exact prompts used to generate each track with Suno AI.
- **Native Media Controls**: Integrates with your operating system's media controls (e.g., lock screen, keyboard shortcuts) via the Media Session API.
- **Open Data**: All music, images, and metadata are included in this repository for reuse.

## Data Source

The music was generated using [Suno](https://suno.com/).

- **Original Suno Playlist:** [https://suno.com/playlist/ed50f5df-5017-4e51-b88a-9aadf3ca025d](https://suno.com/playlist/ed50f5df-5017-4e51-b88a-9aadf3ca025d)

The playlist data and audio files were downloaded and localized using a script from the [music-opendata-fukui](https://github.com/code4fukui/music-opendata-fukui) project. You can replicate this process with the following Deno command:

```sh
deno run -A https://code4fukui.github.io/music-opendata-fukui/download.js ed50f5df-5017-4e51-b88a-9aadf3ca025d
```

## Usage

To run the player locally, clone this repository and open the `index.html` file in a web browser.

```bash
git clone https://github.com/code4fukui/music-brainstorming-bgm.git
cd music-brainstorming-bgm
# Open index.html in your browser
```
