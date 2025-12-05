# AI Pic Editor — Small demo

This repository contains a simple single-page web demo in Tamil that matches your specifications:

- On open: a "Welcome" splash with a cute rabbit shown. The splash fades out after 2s.
- After splash: a small "AI Pic Editor" UI with random short descriptions (changes every few seconds).
- Background: light purple with floating bubbles animation.
- File access:
  - "Request File Access" uses the File System Access API (Chrome/Edge/Opera/Brave).
  - If access is granted and a file is chosen, the app will show the file name and preview (for images).
  - Before granting access, the "Drop File" button shows "Failed" when clicked.
  - After granting access, the "Drop File" button becomes "Open Dropped File" and opens the previously chosen file.
- The UI messages are intentionally simple and in line with what you asked (OK/Failed, etc).
- Ready to upload online (see deployment instructions below).

How to run locally
1. Download the files (index.html, styles.css, script.js).
2. Open `index.html` in a browser. For full file-access functionality use a Chromium-based browser (Chrome, Edge, Brave). The File System Access API is not supported in Firefox / Safari.

Deploy online
- GitHub Pages:
  1. Create a new repository and push these files to the `main` branch.
  2. In repo Settings → Pages, set source to `main` branch → `/ (root)`.
  3. Your site will be published at `https://<username>.github.io/<repo>/`.
- Vercel / Netlify:
  - Create a new project and point to the repo. Both detect static sites and will publish automatically.
  - Or drag & drop the site folder in Netlify Drop.

Notes
- File System Access API requires user gesture and secure context (HTTPS or localhost).
- If a browser doesn't support showOpenFilePicker, the app falls back to an invisible <input type="file">.

I implemented the demo and included the HTML, CSS and JS files below. You can copy them directly into a repo and deploy with GitHub Pages or Netlify. If you want, I can create the GitHub repo and push these files for you (tell me the owner/repo name) or prepare a zip for download.