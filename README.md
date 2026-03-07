# SQL Canvas

**SQL Canvas** is a high-performance Single Page Application that instantly **formats, cleans, compresses, and visualizes SQL scripts**.  
> A powerful, high-performance Single Page Application designed to instantly format, clean, compress, and visualize SQL scripts.  
> Built as a Single File Component, this application runs entirely in your browser without any backend server.

> This app is developed using AI.

---

## Live Demo

Try it out instantly: **[[Live Demo Link](https://bh00t.github.io/SQL-Canvas/) ]**

---

## Key Features

- **Zero Setup**  
  The entire application lives in a single `index.html` file. No build steps, no `npm install`, no local server required — just double-click to run. 

- **Secure Client-Side Processing**  
  All parsing, tokenization, and formatting happen locally in your browser so your SQL never leaves your machine. 

### Advanced AST-Driven Minification
- **Two-Pass Engine**: Safely strips `--` and `/* */` comments and unnecessary whitespace without breaking string literals or complex operators.  
- **Smart Auto-Aliasing**: Optionally generates compact aliases (e.g., `t1`, `t2`) for unaliased tables to reduce footprint.  
- **Single-Line Output**: Collapse the entire script into a single continuous line for maximum minification.  
- **Detailed Reports**: View original vs. minified size, space saved, and counts of characters, lines, and comments removed.

### Intelligent SQL Beautifier
- **Context-Aware Indentation**: Handles subqueries, `CASE` statements, `JOIN` conditions, and block statements (`BEGIN ... END`).  
- **Keyword Normalization**: Converts SQL keywords and functions to uppercase while preserving identifier casing.  
- **Edge-Case Handling**: Supports PostgreSQL casts (`::`), concatenations (`||`), and assignment operators (`:=`).  
- **Live Syntax Highlighting**: Lightweight custom highlighter for keywords, functions, strings, and numbers.

### Highly Interactive UI
- **Split-Pane Design**: Resizable input and output panels.  
- **Drag & Drop**: Drop `.sql` or `.txt` files to load instantly.  
- **Dark/Light Mode**: Theme support for comfortable viewing.  
- **Quick Export**: One-click **Copy to Clipboard** and **Download** buttons.

---

## How to Use

1. **Input your SQL**  
   - Open [Live Website](https://bh00t.github.io/SQL-Canvas/) or open your local `index.html`.  
   - Paste raw SQL into the left editor or drag-and-drop a `.sql` file.

2. **Choose your Mode**  
   - **Minify**: Click the *Minify* tab or press **Ctrl+Enter / Cmd+Enter**. Toggle **Auto-Alias** or **Single Line** for extra compression. View the savings report via the lightbulb icon.  
   - **Beautify**: Click the *Beautify* tab to format and syntax-highlight your SQL.

3. **Export**  
   - Click **Copy** to copy processed SQL to clipboard.  
   - Click **Download** to save as `.min.sql` or `.fmt.sql`.

---

## Technology Stack

- **Core**: HTML5, JavaScript (ES6+)  
- **UI Framework**: React 18 (via ESM importmap)  
- **Styling**: Tailwind CSS (CDN)  
- **Compiler**: Babel Standalone (JSX on the fly)  
- **Icons**: Lucide React  
- **Architecture**: Custom lexical analyzers and AST tokenizers. 

--- 

## Contributing

- Bug reports, feature requests, and pull requests are welcome.  
- Keep changes focused and include tests or examples when applicable.

---