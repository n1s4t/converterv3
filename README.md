# [Pro Studio v1.3 — Mobile & PC Optimized](https://n1s4t.github.io/converterv3/)

**Author:** n1s4t  
**Version:** 1.3
## 🔗 Socials

[![Visit My Guns.lol Profile](https://img.shields.io/badge/Guns.lol-n1s4t-blue?style=for-the-badge)](https://guns.lol/n1s4t)

## Highlights
Pro Studio v1.3 is optimized for both mobile and desktop:
- Responsive layout: 3-panel desktop, single-panel tabbed mobile.
- Touch-friendly targets (min 44px), collapsible FAB menu for mobile.
- Lazy-loading of heavy libraries (Mammoth, docx) to improve mobile performance.
- DOCX import/export, Markdown ↔ HTML sync, multi-tabs, export as .md/.html/.txt/.docx/.pdf.
- Resizable panels on desktop; tabbed navigation on mobile.

## How to use
1. Open `index.html` in a modern browser (desktop or mobile).
2. On desktop you'll see 3 panels (HTML | Markdown | Preview) and resizers.
3. On mobile use the bottom navigation to switch between HTML / Markdown / Preview.
4. Import files: click Import -> select .md/.html/.txt/.docx. DOCX uses Mammoth (loaded only when needed).
5. Export via FAB menu -> Export As -> choose format (.md/.html/.txt/.docx/.pdf).
6. Use Ctrl/Cmd+S to save session to localStorage.

## Files
- `index.html` — main responsive app
- `README.md` — this file

## Notes
- Libraries are loaded from CDNs. For offline or production use, bundle them.
- DOCX export creates basic Word documents; complex styling may be lost.
- PDF export uses browser print; quality depends on browser.

## Next steps (optional)
- Add drag-and-drop import to editor surface.
- Integrate Prettier / HTML tidy for formatting.
- Add cloud sync (GitHub Gist / Google Drive) with OAuth.
