# ![SmartResume](https://img.shields.io/badge/SmartResume-AI%20Resume%20Analyzer-blue) SmartResume

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Vercel](https://img.shields.io/badge/Deploy-Vercel-brightgreen)](https://vercel.com) [![npm version](https://img.shields.io/npm/v/npm?label=Dependencies)](https://www.npmjs.com/)

SmartResume is an interactive AI-powered resume builder and analyzer web application built with **React/Next.js**. Users can upload resumes, get summaries, insights, and feedback using **Puter.js** integration.

---

## 🎬 Demo / Screenshot

### Web App Screenshot

![SmartResume Screenshot](./public/images/demo-screenshot.png)

---

## 🚀 Features

* Upload resumes (PDF/DOCX)
* AI-powered resume analysis and scoring via Puter.js
* Generate summaries and actionable feedback
* Interactive UI with responsive design
* Cloud storage using Puter.js KV and FS
* User authentication with Puter.js

---

## 🛠 Tech Stack

* **Frontend:** React / Next.js
* **State Management:** Zustand
* **Styling:** Tailwind CSS, tw-animate-css
* **AI & Cloud:** Puter.js
* **Build Tools:** Vite

---

## ⚡ Getting Started

### Prerequisites

* Node.js >= 18.x
* npm >= 9.x

### Installation

```bash
git clone https://github.com/<your-username>/SmartResume.git
cd SmartResume
npm install
```

---

### 🏃 Running Locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

### ☁️ Deployment

We recommend **Vercel** for deploying this project:

1. Push your repo to GitHub.
2. Go to [Vercel](https://vercel.com/) → Import Git Repository.
3. Configure build settings (Next.js auto-detected).
4. Deploy and get a live URL.

---

## 📂 Project Structure

```
app/
 ├─ components/   # Reusable UI components
 ├─ lib/          # Puter.js integration, utilities
 ├─ routes/       # Application pages
 ├─ constants/    # App constants
 ├─ types/        # TypeScript type definitions
 ├─ public/       # Static assets (screenshots, GIFs)
app.css           # Global styles
package.json      # Dependencies and scripts
```

---

## ⚙️ Environment Setup

1. Include Puter.js script in your `Layout`:

```html
<script src="https://js.puter.com/v2/"></script>
```

2. Initialize Puter.js in your root layout/component:

```tsx
import { usePuterStore } from "~/lib/puter";
import { useEffect } from "react";

const { init } = usePuterStore();
useEffect(() => {
  init();
}, [init]);
```

---

## 📜 Available Scripts

* `npm run dev` → Run development server
* `npm run build` → Build production version
* `npm run start` → Serve production build

---

## 🤝 Contributing

1. Fork the repository
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push to branch: `git push origin feature/my-feature`
5. Open a Pull Request


---
