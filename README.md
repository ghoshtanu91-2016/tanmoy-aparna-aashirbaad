# Tanmoy & Aparna — Paka Katha & Aashirbaad 🌺
### 18 June 2026

A Bengali engagement ceremony gallery platform, ready to deploy on GitHub Pages.

---

## 📁 Repository Folder Structure

```
your-repo/
├── index.html          ← main platform (do not rename)
├── README.md
├── images/
│   ├── photo1.jpg      ← your ceremony photos go here
│   ├── photo2.jpg
│   ├── photo3.jpg
│   └── ...             ← add as many as you like
└── music/
    └── song.mp3        ← your background song goes here
```

---

## 🖼️ How to Add Your Photos

1. Put all your ceremony `.jpg` / `.jpeg` / `.png` photos inside the `images/` folder.
2. Open `index.html` in a text editor, find this section near the bottom:

```js
const IMAGE_FILES = [
  "images/photo1.jpg",
  "images/photo2.jpg",
  ...
];
```

3. Update the list to match your actual filenames exactly. Example:

```js
const IMAGE_FILES = [
  "images/ceremony_01.jpg",
  "images/ceremony_02.jpg",
  "images/family_blessing.jpg",
  "images/ring_exchange.jpg",
  "images/sweets_table.jpg"
];
```

> ⚠️ Filenames are **case-sensitive** on GitHub. `Photo1.JPG` ≠ `photo1.jpg`

---

## 🎵 How to Add Your Song

1. Place your `.mp3` file inside the `music/` folder.
2. In `index.html`, find:

```js
const MUSIC_FILE = "music/song.mp3";
const MUSIC_DISPLAY_NAME = "Aaj Amar Mon Bhalo Nei";
```

3. Change `song.mp3` to your actual filename, and update the display name:

```js
const MUSIC_FILE = "music/tumi_je_amar.mp3";
const MUSIC_DISPLAY_NAME = "Tumi Je Amar — Kishore Kumar";
```

> ℹ️ Browsers require a user click before audio plays. The song auto-starts on the first click anywhere on the page.

---

## 🚀 Deploying to GitHub Pages (Step by Step)

### Step 1 — Create a GitHub Repository
- Go to [github.com](https://github.com) and sign in
- Click **"New repository"**
- Name it something like `tanmoy-aparna-aashirbaad`
- Set it to **Public**
- Click **Create repository**

### Step 2 — Upload Your Files
- Click **"uploading an existing file"** on the repository page
- Upload `index.html` first
- Create the `images/` folder: type `images/photo1.jpg` in the file name box to auto-create the folder, then upload all your photos
- Create the `music/` folder the same way: type `music/song.mp3` and upload your song
- Click **Commit changes**

### Step 3 — Enable GitHub Pages
- Go to your repository **Settings**
- Click **Pages** in the left sidebar
- Under **Source**, select **Deploy from a branch**
- Set Branch to **main**, folder to **/ (root)**
- Click **Save**

### Step 4 — Your site goes live!
Within 1–2 minutes, your platform will be available at:

```
https://YOUR-USERNAME.github.io/tanmoy-aparna-aashirbaad/
```

Share this link with family and friends 🌸

---

## ✏️ Quick Customisations

| What | Where in index.html |
|------|---------------------|
| Change song display name | `const MUSIC_DISPLAY_NAME = "..."` |
| Add / remove photos | `const IMAGE_FILES = [...]` |
| Change background music volume | `audio.volume = 0.42` → 0.0 to 1.0 |
| Edit the love story paragraph | Find "One auspicious day in June" section |
| Edit the Bengali verse | Find `<div class="bengali-verse">` |

---

*Made with love for Tanmoy & Aparna · শুভ আশীর্বাদ*
