# ⛩️ Kage — Kyoto Nightwalk

<p align="center">
  <img src="https://raw.githubusercontent.com/fallss/kage-kyoto-nightwalk-web/main/public/favicon.svg" alt="Kage Logo" width="80" height="80" />
</p>

<p align="center">
  <em>"Where stillness reveals the unseen."</em><br />
  A five-chapter night walk through a Kyoto mountain temple. Charred cypress, lantern light, and a vermilion moon, rendered live in WebGL.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-19.2-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 19" />
  <img src="https://img.shields.io/badge/TypeScript-Ready-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Vite-8.2-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/WebGL-Custom_Shaders-990000?style=for-the-badge&logo=webgl&logoColor=white" alt="WebGL" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

---

## 📖 Overview

**Kage (影)** is an atmospheric, interactive web experience built with modern React and WebGL. It transports visitors through a meditative journey across a Kyoto mountain sanctuary at twilight.

### ✨ Key Features

- **🌙 5 Atmospheric Chapters**: Seamless narrative flow from *The Hidden Gate*, through lantern-lit pathways, to the mountaintop afterlight.
- **🏮 Live WebGL & Shaders**: Real-time atmospheric depth, particle effects, vermilion moon lighting, and responsive canvas rendering.
- **✒️ Curated Typography & Motion**: Custom typographic hierarchy using the Onest typeface, paired with delicate cubic-bezier scroll transitions.
- **⚡ Modern Frontend Architecture**: Built on Vite with React 19, TypeScript, and high-performance Oxlint integration.

---

## 🛠️ Tech Stack

- **Framework**: [React 19](https://react.dev/)
- **Build Tool**: [Vite 8](https://vite.dev/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Graphics & Styling**: WebGL, GLSL Shaders, Modern Vanilla CSS Tokens
- **Linter**: [Oxlint](https://oxc.rs/)

---

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed (v18+ recommended):

```bash
node -v
npm -v
```

### Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/fallss/kage-kyoto-nightwalk-web.git
cd kage-kyoto-nightwalk-web
npm install
```

### Development Server

Start the local development server:

```bash
npm run dev
```

Open your browser and navigate to:
```
http://localhost:5175/
```

> **Note:** If port 5175 is in use, specify a custom port: `PORT=3000 npm run dev`

### Production Build

Create an optimized production bundle:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

---

## 📂 Project Structure

```text
├── public/
│   ├── favicon.svg
│   ├── icons.svg
│   └── landing-pages/
│       ├── kage.html               # WebGL engine & shader pipeline
│       └── secret-pathways-assets/ # Typography & asset files
├── src/
│   ├── components/
│   │   └── KageLandingPage.tsx    # React wrapper component
│   ├── shaders/                   # Typography & frame orchestrators
│   ├── App.tsx                    # Application root
│   ├── main.tsx                   # Entry point
│   └── index.css                  # Base styles
├── PANDUAN_MENJALANKAN.md          # Panduan lengkap (Bahasa Indonesia)
├── package.json
└── vite.config.ts
```

---

## 🇮🇩 Dokumentasi Bahasa Indonesia

Panduan langkah demi langkah menjalankan website ini secara lokal tersedia di:  
👉 **[PANDUAN_MENJALANKAN.md](./PANDUAN_MENJALANKAN.md)**

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
