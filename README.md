# Project Documentation Organizer & Tree Index

A browser-based, local-first documentation and project manager. Organize, browse, and edit your project files and documentation with a beautiful tree index—all in your browser, with no server or backend required.

## Features

- **Tree-based Index:** Drag-and-drop, add, and organize folders/files in a jsTree-powered UI (`tree_index.html`).
- **Local File Editing:** Create, open, and edit files and folders directly on your computer using the File System Access API (`project_manager.html`).
- **Save/Load Index:** Export/import your tree structure as a JSON file.
- **Hyperlinked Navigation:** Click any file in the tree to open it (if accessible).
- **No Backend Required:** 100% client-side, works offline, no installation needed.
- **Modern, Minimal UI:** Clean design for productivity.

## Technology Stack

- **HTML5, CSS3, JavaScript (ES6+)**
- **[jsTree](https://www.jstree.com/):** For the interactive tree view
- **[jQuery](https://jquery.com/):** For DOM manipulation and jsTree integration
- **File System Access API:** For direct local file/folder read/write (Chromium browsers only)

## Limitations

- **Browser Compatibility:**
  - Requires a Chromium-based browser (Chrome, Edge, Brave, Opera, etc.)
  - **Not supported on Safari or Firefox** (due to lack of File System Access API)
  - Will show an error if loaded in an unsupported browser
- **Local-Only:**
  - Cannot access files outside user-selected folders
  - Cannot set the default folder for the file picker (browser security limitation)
- **No Real-Time Collaboration:**
  - This is a single-user, local tool

## How is this different from other solutions?

- **No install, no account, no backend:** Everything runs in your browser, with your files.
- **Direct local file editing:** Unlike Notion, Obsidian, or Joplin, you can edit files directly in your file system from the browser.
- **Publishable as a static site:** Host on GitHub Pages, Netlify, or any static host—no server required.
- **Simple, focused UI:** Designed for project documentation and code snippets, not as a general-purpose note-taking app.

## Open-Source Alternatives

- **[Obsidian](https://obsidian.md/):** Markdown knowledge base, but requires a desktop app and doesn’t support browser-based local editing.
- **[Joplin](https://joplinapp.org/):** Open-source note-taking, but not browser-based for local files.
- **[Dendron](https://www.dendron.so/), [Foam](https://foambubble.github.io/foam/):** Markdown knowledge bases for VSCode.
- **[Logseq](https://logseq.com/):** Open-source, local-first, but works best as an Electron app.
- **[jsTree](https://www.jstree.com/):** The library used for the index, but not a full documentation manager.

## Getting Started

1. **Clone or download this repo.**
2. **Open `project_manager.html` in your Chromium browser.**
3. **Click "Index" to open the tree index UI.**
4. **Start organizing and editing your documentation!**

## Deploy as a GitHub Page

1. Push this repository to GitHub.
2. Go to your repo's Settings → Pages.
3. Set the source to the `main` branch (or `gh-pages` if you use that).
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/`.

---
- **[Try the demo](https://sanjaysingh13.github.io/ProjectDocumentationOrganizer/index.html)**

**Made with ❤️ for local-first, browser-based documentation.**
