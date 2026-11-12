# UWE Revision Academy

A free, single-page revision app for two UWE Bristol modules:

- **UFCE53 – Cyber Security Forensics**
- **UFCF8R-30-2 – WebApp Development**

**Live site:** https://ws421778.github.io/DaTS-Revision/

## Features

- **Topic units** that follow the lecture slides, plus extra topics from the module briefs that haven't been taught yet.
- **Question banks** with about 690 questions: 368 for Forensics and 323 for WebApp, 147 of which are code questions.
- **Mixed question types** in the style of the Technical Exam, including code reading and code completion.
- **Forensics Section B practice** with scenario-based multiple-choice questions.
- **Progress tracking** saved in your browser.

## Using it

Open the live site, or download `index.html` and open it in any modern browser. You don't need to install anything or create an account.

> **Note:** progress is stored in your browser's local storage. It is lost if you use a private or InPrivate window or clear your site data. It also doesn't sync between devices.

## Project structure

```
app-source/
├── styles.css          # App styling
├── body.html           # Page markup
├── app.js              # App logic
├── lessons/<module>/   # Lesson content, one .txt per unit
├── bank/<module>/      # Question banks, one .txt per unit
└── build.py            # Bundles everything into one HTML file
```

## Building

You need Python 3. From `app-source/`, run:

```bash
py build.py
```

This writes `UWE Revision Academy.html` to the parent folder.

## Updating the live site

1. Rebuild with the command above.
2. Rename `UWE Revision Academy.html` to `index.html`.
3. Upload it to this repository, replacing the old file, and commit.
4. GitHub Pages redeploys automatically within a minute or two.

## Disclaimer

This is an unofficial study aid and is not affiliated with or endorsed by UWE Bristol. Always check what you learn against the official module materials.
