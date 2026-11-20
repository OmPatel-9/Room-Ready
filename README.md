# RoomReady: VR Interview Practice

RoomReady is a browser based mock interview app. Practice with role specific questions, spoken prompts, voice typing, written answers, STAR notes, and immediate coaching feedback. A WebXR interview room is available on supported VR headsets, with a desktop and mobile interface as a fallback.

## Features

- Interview tracks for general, software engineering, product management, and internship roles
- Balanced, warm-up, and challenge practice modes
- Spoken questions using the browser's speech synthesis
- Voice typing with the browser's speech recognition API, plus a text answer option
- Optional notes organized around Situation, Task, Action, and Result
- Coaching based on answer length, structure, filler words, and evidence of outcomes
- WebXR interview room for compatible headsets and browsers
- Responsive layout for desktop and mobile

## Run locally

No build step or package installation is required. From this folder, start a local server:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

Microphone access depends on browser support and permission. WebXR requires a compatible browser and headset. It generally requires HTTPS, except when using localhost.

## Publish with GitHub Pages

1. Create a new GitHub repository and upload these project files.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions** as the source.
4. Push to the `main` branch. The included workflow deploys the site to GitHub Pages.

The first deployment may take a minute. GitHub will show the published URL under **Settings → Pages**.

## Project structure

```text
RoomReady/
├── .github/workflows/pages.yml
├── index.html
├── .gitignore
└── README.md
```

## Notes

This is a front-end prototype. Coaching scores are simple practice heuristics, not an AI evaluation or hiring assessment. Answers are kept in the page while it is open; the app has no account system or server-side storage. The page loads A-Frame and Google Fonts from their public CDNs. Speech recognition availability varies by browser.
