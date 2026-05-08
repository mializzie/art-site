# ✦ My Portfolio – Setup Guide

## Folder Structure

Keep all files like this:

```
portfolio/
├── index.html
├── artwork.html
├── music.html
├── animations.html
├── data.json          ← YOU EDIT THIS to add content
├── README.txt
└── images/
    ├── artwork/       ← drop your artwork images here
    └── animations/    ← drop your GIF files here
```

---

## How to Add Artwork

1. Copy your image file into the `images/artwork/` folder.
   (Supported formats: .jpg, .jpeg, .png, .webp, .gif)

2. Open `data.json` in any text editor (Notepad, TextEdit, VS Code, etc.)

3. Find the `"artwork"` section and add a new entry:

```json
{
  "id": "art-3",
  "image": "images/artwork/your-filename.jpg",
  "title": "Your Title Here",
  "description": "Your description here."
}
```

4. Save `data.json` and refresh the browser. Done!

---

## How to Add a GIF / Animation

1. Copy your .gif file into the `images/animations/` folder.

2. Open `data.json` and find the `"animations"` section. Add:

```json
{
  "id": "gif-2",
  "image": "images/animations/your-file.gif",
  "title": "Animation Title",
  "description": "Description here."
}
```

---

## How to Add Music

Open `data.json` and find the `"music"` section. Add:

```json
{
  "id": "song-2",
  "youtubeId": "PASTE_YOUTUBE_ID_HERE",
  "title": "Song Title – Artist",
  "relatedArtwork": "Name of related artwork (optional)",
  "description": "Notes about this song."
}
```

To find the YouTube ID: it's the part after `v=` in the URL.
Example: `https://www.youtube.com/watch?v=dQw4w9WgXcQ` → ID is `dQw4w9WgXcQ`

---

## IDs

Each entry needs a unique `"id"` value — just use any text with no spaces,
e.g. `"art-3"`, `"gif-beach"`, `"song-summer"`.

---

## Opening the Site

Double-click `index.html` to open in your browser.
If images don't load, try using a simple local server:
- VS Code: install "Live Server" extension, right-click index.html → Open with Live Server
- Or run in terminal: `npx serve .`
