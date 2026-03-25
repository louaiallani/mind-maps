# Mind-Maps - Interactive Mind Map

Mind-Maps is a browser-based mind-mapping workspace built as a single-page app.
It supports rapid ideation, visual structuring, and lightweight knowledge capture without any backend.

In practical terms: this is a local-first thinking surface. You can map, connect, annotate, and export your work fast.

## Why This Project Exists

Most note tools optimize for storage. Mind-Maps optimizes for cognition under time pressure:
- Build structure quickly
- Reposition ideas fluidly
- Preserve output in reusable formats

The core logic is simple and deliberate: clarity of use beats architectural complexity for this problem class.

## Core Capabilities

- Create, edit, delete, and color-code nodes
- Add child nodes and root nodes
- Collapse and expand branches
- Connect any two entities (node-to-node, node-to-image, image-to-image)
- Drag nodes and images freely
- Pan and zoom canvas
- Import and export map data as JSON
- Export visuals as PNG, JPEG, SVG, and PDF
- Upload image nodes into the map
- Draw freehand annotations with pen and eraser tools
- Undo/redo support (`Ctrl+Z`, `Ctrl+Shift+Z`, `Ctrl+Y`)
- Local persistence via browser storage

## Tech Stack

- HTML
- CSS
- Vanilla JavaScript
- Runtime-loaded libraries:
  - html2canvas (image capture)
  - jsPDF (PDF export)

## Run Locally

No build step is required.

1. Clone the repository.
2. Open `index.html` in any modern browser.

Optional local server (recommended for smoother browser behavior):

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Project Structure

```text
.
|-- index.html
|-- README.md
|-- LICENSE
|-- CONTRIBUTING.md
|-- SECURITY.md
`-- .github/
```

## Known Constraints

- The app is intentionally single-file for portability.
- External CDN dependencies require network access the first time they are loaded.
- Local storage is browser-scoped.

## Roadmap Ideas

- Multi-select node operations
- Search and filter
- Optional dark/light themes
- Better mobile ergonomics for dense maps
- Snapshot versioning

## Contributing

Pull requests are welcome. Read `CONTRIBUTING.md` before opening one.

## Security

If you discover a vulnerability, follow `SECURITY.md`.

## License

This project is distributed under the MIT License. See `LICENSE`.
