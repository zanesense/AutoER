# ⚡ AutoER — Instant SQL → ERD Visualizer  
> Transform your SQL schemas into beautiful, interactive ER diagrams — in real time.

<p align="center">
  <a href="https://github.com/zanesense/AutoER/stargazers">
    <img src="https://img.shields.io/github/stars/zanesense/AutoER?color=22d3ee&style=for-the-badge" alt="GitHub Stars">
  </a>
  <a href="https://github.com/zanesense/AutoER/issues">
    <img src="https://img.shields.io/github/issues/zanesense/AutoER?color=facc15&style=for-the-badge" alt="GitHub Issues">
  </a>
  <a href="https://github.com/zanesense/AutoER/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/zanesense/AutoER?color=4ade80&style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/zanesense/AutoER/fork">
    <img src="https://img.shields.io/github/forks/zanesense/AutoER?color=06b6d4&style=for-the-badge" alt="Forks">
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Made%20with-HTML%20%7C%20Tailwind%20%7C%20JS-1e293b?style=for-the-badge&logo=javascript" alt="Tech Stack">
  </a>
</p>

<p align="center">
  🎯 <a href="https://zanesense.github.io/AutoER/" target="_blank"><b>LIVE DEMO → AutoER</b></a>  
</p>

---

## 🚀 Overview

**AutoER** is a minimalist, AI-enhanced tool that converts **SQL DDL** statements into **Entity-Relationship Diagrams (ERDs)** instantly.  
Whether you paste SQL, upload a `.sql` file, or describe your database in plain English — AutoER builds your ERD in seconds.

No setup. No backend. 100% client-side and lightning fast ⚡  

🎥 **[Try the Live Demo →](https://zanesense.github.io/AutoER/)**  

---

## ✨ Key Features

- 🧠 **AI DDL Generator** — Describe your database idea, and AutoER generates SQL automatically (Gemini API)
- ⚙️ **Real-Time ERD Rendering** — Watch your diagram update as you type  
- 🌓 **Dark / Light Mode** — Seamless minimalist themes  
- 🌲 **Custom Mermaid Themes** — Dark, Default, Forest, and Neutral  
- 📦 **SQL Import** — Upload `.sql` files instantly  
- 🔍 **Zoom Controls** — Smooth scaling for complex diagrams  
- 🖼️ **Export as PNG** — Download your ER diagram in one click  
- 💾 **Local Persistence** — Your last SQL and theme are auto-saved  

---

## 🧩 Built With

| Technology | Purpose |
|-------------|----------|
| **HTML5 / JS (ES6 Modules)** | Core app logic |
| **Tailwind CSS** | Clean, responsive UI |
| **Mermaid.js** | ER diagram rendering |
| **html-to-image** | PNG export |
| **Google Gemini API (optional)** | AI-powered DDL generation |

---

## 🛠️ Setup & Run Locally

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/zanesense/AutoER.git
cd AutoER
````

### 2️⃣ Start a Local Server

If you’re on Windows, simply double-click:

```
start.bat
```

Or run manually:

```bash
python -m http.server 8000
```

Then open your browser and visit:

```
http://localhost:8000
```

---

## 🔑 AI Setup (Optional)

To enable **AI DDL generation**:

1. Get a **Gemini API Key** from [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Open `index.html`
3. Find this line:

   ```js
   const GEMINI_API_KEY = 'YOUR_API_KEY_HERE';
   ```
4. Replace it with your actual key.

---

## 💡 Example Usage

Paste SQL like this:

```sql
CREATE TABLE Customers (
  customer_id INT PRIMARY KEY,
  name VARCHAR(50),
  email VARCHAR(100) UNIQUE
);

CREATE TABLE Orders (
  order_id INT PRIMARY KEY,
  customer_id INT,
  total DECIMAL(10,2),
  FOREIGN KEY (customer_id) REFERENCES Customers(customer_id)
);
```

✅ Instantly see the ER diagram appear!

---

## 🧑‍💻 Author

**Developed by [@zanesense](https://github.com/zanesense)**
Built with ❤️ for developers, students, and database enthusiasts.

---

## 📜 License

MIT License © 2025 — Feel free to fork, improve, and innovate!
