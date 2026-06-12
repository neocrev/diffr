<p align="center">
  <h1 align="center">diffr</h1>
  <p align="center"><i>Side-by-side and unified diff viewer — paste and compare text right in your browser.</i></p>
  <p align="center">
    <img alt="GitHub Pages" src="https://img.shields.io/badge/live-GitHub%20Pages-blue?style=flat">
    <img alt="License" src="https://img.shields.io/github/license/neocrev/diffr?style=flat">
    <img alt="Zero deps" src="https://img.shields.io/badge/deps-0-brightgreen?style=flat">
  </p>
</p>

<p align="center">
  <strong>→ <a href="https://neocrev.github.io/diffr/">neocrev.github.io/diffr</a></strong>
</p>

---

**diffr** is a zero-dependency, single-file HTML app for comparing text. Paste two versions, see exactly what changed.

## Features

- **Side-by-Side** mode — original and changed text aligned line by line
- **Unified** mode — classic diff format with context hunks
- **LCS-based** diff algorithm — accurate line-level comparison
- **Auto-diff** — results update automatically while you type (300ms debounce)
- **Tab size** control — renders tabs as 2, 4, or 8 spaces
- **Syntax-coloured** diff output — green additions, red deletions, neutral context
- **Diff summary** — shows +added/-removed/=unchanged line counts in header
- **Word Wrap** — toggle to wrap long lines instead of scrolling
- **Copy diff** — one-click copy as unified diff text
- **Zero dependencies** — no libraries, no build step, no telemetry

## Usage

1. Open [diffr](https://neocrev.github.io/diffr/)
2. Paste the original text in the left panel
3. Paste the changed text in the right panel
4. See the diff instantly

Switch between **Side** and **Unified** modes with the toggle in the toolbar.

## Technical

diffr implements a **Longest Common Subsequence (LCS)** algorithm from scratch to compute line-level diffs. The entire application is a single HTML file with inline CSS and JavaScript — no frameworks, no build tools, no network requests after page load.

## License

MIT
