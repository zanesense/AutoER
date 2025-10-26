# ⚡ AutoER: SQL DDL to ERD Minimalist Visualizer

AutoER is a modern, minimalist web tool designed for developers and database architects to quickly visualize SQL Data Definition Language (DDL) into an Entity-Relationship Diagram (ERD). It features a sleek, high-contrast dark/light theme, instant rendering, and an AI integration for rapid schema prototyping.

## ✨ Features

* **Instant Visualization:** Converts `CREATE TABLE` statements into a live, interactive **Mermaid ERD** as you type.
* **AI DDL Generation:** Integrated feature to generate complex SQL schemas instantly from a plain-text scenario description using the **Gemini API**.
* **Minimalist Aesthetic:** Clean, modern UI with a high-contrast **Dark/Light Mode** toggle.
* **Customizable Diagram:** Supports multiple Mermaid themes (`Dark`, `Default`, `Forest`, `Neutral`) and includes a **Zoom Slider** for detailed inspection.
* **Export:** Easily download the generated diagram as a **PNG** image.
* **Local Persistence:** Automatically saves your last entered SQL DDL in your browser's local storage.

---

## 🚀 Getting Started

AutoER is a single-file application requiring no build steps.

### Prerequisites

* A modern web browser.
* For the **AI Generation** feature, you **must** run the file using a **local web server** (e.g., VS Code Live Server, Python's `http.server`) to avoid Cross-Origin Resource Sharing (CORS) errors when calling the Gemini API.

### Installation & Setup

1.  **Save the file:** Save the entire provided code as a single HTML file (e.g., `index.html`).
2.  **Add API Key (Optional):** To enable AI DDL generation, open the HTML file and locate the following line in the main `<script>` block:

    ```javascript
    const GEMINI_API_KEY = ''; // <-- PASTE YOUR KEY HERE
    ```
    Replace the empty string with your actual Google Gemini API key.
3.  **Run Locally:** Launch your local web server and navigate to `index.html`.

---

## 🛠️ How to Use

### 1. DDL Input

* **Type or Paste:** Enter your PostgreSQL, MySQL, or generic SQL `CREATE TABLE` statements into the **SQL DDL Source** textarea.
* **Import:** Use the **Import .sql** button to load a schema file from your local machine.
* **Instant Render:** The diagram updates automatically, typically within 500 milliseconds of your last change.

### 2. AI DDL Generation

1.  Click the **Generate DDL (AI)** button.
2.  In the modal, provide a detailed description of the database requirements (e.g., "A social media schema with users, posts, comments, and a likes many-to-many table.").
3.  Click **Generate DDL**. The resulting SQL will replace the content in the input box and automatically render the ERD.

### 3. Diagram Interaction

* **Zoom:** Use the **Zoom Slider** to pan in and out of complex diagrams. The diagram area is fully scrollable in all directions.
* **Theme:** Use the **ERD Theme** dropdown to change the visual style of the diagram itself (`dark`, `default`, `forest`, `neutral`).
* **Export:** Click **Export PNG** to save the visualization as a high-resolution image.

---

## 🎨 Theme Customization

The application supports two distinct UI themes and saves your preference automatically:

| Mode | Accent Color | Main Background | Card Background |
| :--- | :--- | :--- | :--- |
| **Dark** | Cyan-400 (`#22d3ee`) | Slate-900 (`#0f172a`) | Slate-800 (`#1e293b`) |
| **Light** | Cyan-400 (`#22d3ee`) | Sky-50 (`#f8fafc`) | White (`#ffffff`) |

Toggle the theme using the switch in the upper-right corner of the header.

---

## ⚙️ Technology Stack

* **Frontend:** Vanilla HTML, CSS (Tailwind CSS CDN)
* **Visualization:** [Mermaid.js](https://mermaid.js.org/) (for generating SVG diagrams)
* **AI Integration:** [Google Gemini API](https://ai.google.dev/) (using `gemini-2.5-flash`)
* **Export:** [html-to-image](https://www.npmjs.com/package/html-to-image)

---

## 🔗 Connect

*If you've enjoyed using AutoER or have suggestions, feel free to connect!*



| Platform | Link |
| :--- | :--- |
| **GitHub** | `https://github.com/zanesense` |
| **LinkedIn** | `https://linkedin.com/in/saaimaly` |
