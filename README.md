# SQL Canvas

**SQL Canvas** is a high-performance Single Page Application that instantly **formats, cleans, and compresses SQL scripts** — entirely in your browser, with no backend, no build steps, and no data ever leaving your machine.
---

## Live Demo

Try it out instantly: **[[SQL Canvas](https://bh00t.github.io/SQL-Canvas/) ]**

---

## Screenshots

**Minify** — strips comments, whitespace, and auto-generates aliases. 40%+ size reduction on real scripts.

![SQL Canvas Minify](image-1.png)



**Beautify** — transforms a single-line mess into clean, indented, syntax-highlighted SQL.

![SQL Canvas Beautify](image.png)

---

## Getting Started

No installation required.

1. Visit the [Live Demo](https://bh00t.github.io/SQL-Canvas/), **or**
2. Download `index.html` and open it in any modern browser.

That's it — the entire application is a single self-contained file.

---

## Key Features

### Zero Setup
The entire application lives in a single `index.html` file. No `npm install`, no build process, no local server — just open it in a browser and start working.

### Secure Client-Side Processing
All parsing, tokenization, and formatting happen locally in your browser. Your SQL never leaves your machine.

### Advanced AST-Driven Minification
- **Two-Pass Engine** — safely strips `--` and `/* */` comments and unnecessary whitespace without breaking string literals or complex operators.
- **Smart Auto-Aliasing** — optionally generates compact aliases (e.g., `t1`, `t2`) for unaliased tables to reduce script size.
- **Single-Line Output** — collapses the entire script into one continuous line for maximum compression.
- **Detailed Reports** — view original vs. minified size, space saved, and counts of characters, lines, and comments removed.

### Intelligent SQL Beautifier
- **Context-Aware Indentation** — handles subqueries, `CASE` statements, `JOIN` conditions, and block statements (`BEGIN ... END`).
- **Keyword Normalization** — converts SQL keywords and functions to uppercase while preserving identifier casing.
- **Edge-Case Handling** — supports PostgreSQL casts (`::`), concatenations (`||`), and assignment operators (`:=`).
- **Live Syntax Highlighting** — lightweight custom highlighter for keywords, functions, strings, and numbers.

### Highly Interactive UI
- **Split-Pane Design** — resizable input and output panels.
- **Drag & Drop** — drop `.sql` or `.txt` files directly onto the editor to load instantly.
- **Dark / Light Mode** — theme support for comfortable viewing in any environment.
- **Quick Export** — one-click Copy to Clipboard and Download as `.min.sql` or `.fmt.sql`.

---

## How to Use

1. **Load your SQL** — paste it into the left editor, or drag and drop a `.sql` file onto the panel.
2. **Choose a mode:**
   - **Minify** — press `Ctrl+Enter` / `Cmd+Enter`, or click the Minify button. Toggle **Auto-Alias** or **Single Line** for extra compression. Use the lightbulb icon to view the savings report.
   - **Beautify** — click the Beautify tab to format and syntax-highlight your SQL.
3. **Export** — click **Copy** to copy the output to clipboard, or **Download** to save the file.

---

## Technology Stack

| Layer | Technology |
|---|---|
| Core | HTML5, JavaScript (ES6+) |
| UI Framework | React 18 (via ESM import map) |
| Styling | Tailwind CSS (CDN) |
| Compiler | Babel Standalone (JSX on the fly) |
| Icons | Lucide React |
| Architecture | Custom lexical analyzers and AST tokenizers |

---

## Browser Compatibility

SQL Canvas works in all modern browsers. The following are recommended:

- Google Chrome 90+
- Mozilla Firefox 88+
- Microsoft Edge 90+
- Safari 14+

> Note: Opening `index.html` directly via `file://` may restrict some browser APIs (e.g., clipboard). For full functionality, use the [Live Demo](https://bh00t.github.io/SQL-Canvas/) or serve the file through a local server.

---

## Contributing

Bug reports, feature requests, and pull requests are welcome.

- **Bugs** — open an issue with a clear description and a minimal SQL example that reproduces the problem.
- **Features** — open an issue first to discuss the idea before submitting a PR.
- **Pull Requests** — keep changes focused and include a brief description of what was changed and why.

---

## License

This project is open source. See [LICENSE](LICENSE) for details.

---

## Acknowledgements

Built with the help of AI tools. Core SQL parsing and formatting logic is custom-written and browser-native.