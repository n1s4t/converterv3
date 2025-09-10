# Pro Studio v2.1 — Markdown · HTML · DOCX Studio

**Author:** n1s4t  
**Version:** 2.1

## What’s new in v2.1
- All features from v2 plus:
  - **DOCX import** (via Mammoth.js) → converts to HTML & Markdown
  - **DOCX export** (via docx library) — exports editor content to .docx
  - New button formation (FABs, chips, glass pills) with ripple effect
  - Export menu with multiple formats (.md, .html, .txt, .docx, .pdf)
  - Improved UX: multi-file tabs, resizable panels, themes, search/replace

## Files
- `index.html` — main app (single-file, client-side)
- `README.md` — this file

## How to use
1. Open `index.html` in a modern browser (Chrome, Edge, Firefox).
2. Use **Import** to load `.md`, `.html`, `.txt`, or `.docx`.
   - DOCX is converted to HTML using Mammoth and saved into the current tab.
3. Use **New** to create tabs/files and switch between them.
4. Toggle **Auto-sync** to convert Markdown → HTML automatically.
5. Use the floating **Export As** menu to export to `.md`, `.html`, `.txt`, `.docx`, or `.pdf`.
6. `Ctrl/Cmd+S` saves the session into `localStorage`. Files persist in your browser.
7. For `.docx` export, the docx library constructs a simple Word doc from paragraphs (plain text). Complex DOCX styling is limited in this client-side implementation.

## Technical notes & limitations
- All conversion libraries are loaded from public CDNs; offline usage requires bundling them.
- DOCX export creates simple paragraphs — it does not preserve complex styling, images, or advanced formatting.
- PDF export uses the browser print dialog; quality depends on the browser’s print engine.
- This is a client-only app (no server). For cloud sync / GitHub integration you’ll need a backend and OAuth.

## License / Ownership
You retain full ownership. Use/modify freely. Suggested copyright:

```
© 2025 n1s4t — Pro Studio v2.1
```

## Next improvements (suggested)
- Add drag & drop import directly onto editors.
- Better DOCX -> HTML fidelity (preserve images).
- Integrate Prettier / HTML tidy for formatting.
- Add cloud save (GitHub Gist / Google Drive).

Enjoy — tell me if you want a packaged electron app or GitHub-ready repo with CI next!
