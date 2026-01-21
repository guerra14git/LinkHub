# LinkHub — Personal Links & Projects Organizer

Simple single-file personal link hub and small projects organizer.

This repository is a minimal, static site you can open locally in a browser to keep your important links and a short projects list. Projects are stored in your browser's localStorage, so nothing is uploaded to a server.

## Features

- Header with quick icons and a short title.
- Avatar + name area.
- Main buttons area for links (Projects, Github, LinkedIn, About).
- Projects section where you can add project title, optional URL and short description.
- Projects are persisted locally using localStorage.

## Files

- `index.html` — main page (single page app style).
- `styles.css` — styling and responsive rules.
- `scripts.js` — small client-side logic to add/list/remove projects (uses localStorage).
- `icons/` and `img/` — image assets used by the page.

## How to use

1. Open `index.html` in your browser (double-click or `File -> Open`).
2. In the "Projects" section, add a project title, optional link and a short description. Click "Add project".
3. Projects appear below; use "Open" to open the link or "Delete" to remove it.
4. Use "Clear all" to wipe the whole projects list (this removes localStorage data).

Notes:
- Data is stored only in your browser's localStorage for this site. Clearing site data or using a different browser/device will not carry over the saved projects.

## Customization ideas

- Replace the placeholder buttons with the real links you use.
- Add icons to project items (small SVGs or images) and store an icon URL in the project object.
- Add tags/categories and a simple filter UI.
- Hook the site to a backend or sync via GitHub gist / Drive for cross-device sync.

## Development

This is a pure static site, no build step required. To preview locally, open `index.html` in your browser. For local web server (optional):

```bash
# python 3
python -m http.server 8000
# then open http://localhost:8000
```

## License

Use as you wish. No warranty.
