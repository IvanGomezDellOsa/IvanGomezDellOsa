[English](README.en.md) | [Español](README.md)

<h1 align="center">Iván Gómez Dell'Osa</h1>

<p align="center">
  <em>Systems Engineering · Backend · Applied Artificial Intelligence</em>
</p>

---

I am studying Systems Engineering with a focus on backend and applied artificial intelligence. I have my own projects in production and freelance experience delivering software to real clients.

My degree provides solid fundamentals in programming logic, mathematical analysis and algorithm design. I complement them in a self-taught way with current technologies and constant study of product and markets. In combination with the operational management of a small business (PyME), where I developed an interest in business, product and team management.

---

## 🛠 Projects

### [Datos Pauta Oficial](https://github.com/IvanGomezDellOsa/DatosPautaOficial)
`Python` `ETL` `SQLite` `Astro` `React` `TypeScript` `Cloudflare R2/Pages`

The first and only unified database of Argentine official advertising spending: **540,413 advertising orders** from four jurisdictions (Nación, CABA, PBA and Santa Fe), covering 2003–2025, with amounts deflated by IPC so the figures are comparable across years. A custom ETL in Python that includes an **exclusive PBA 2020–2024 dataset reconstructed by processing more than 500 PDF resolutions** —data that does not exist in any open data portal—. A 100% backendless architecture: the SQLite database (~173 MB) lives on Cloudflare R2 and the browser queries only the bytes it needs via HTTP Range Requests (`sql.js-httpvfs`). Operating cost ≈ $0.

🌐 [datospautaoficial.com.ar](https://datospautaoficial.com.ar)

---

### [Navkok Security Group SRL — Corporate Website](https://github.com/IvanGomezDellOsa/NavkokSecurityGroup_Website) *(In progress)*
`Next.js` `TypeScript` `Tailwind CSS`

Complete redesign of the corporate website of a security company with over 30 years of experience and ISO 9001, 14001 and 45001 certifications. Focus on high-impact design that reflects its track record and credentials. Deploy in progress.

🌐 [Navkok](https://navkok-website-private.vercel.app/)

---

### [PilatesAllCanning](https://github.com/IvanGomezDellOsa/PilatesAllCanning_App)
`Flutter` `Python` `FastAPI` `PostgreSQL` `Firebase` `Docker`

A multiplatform management app (iOS, Android, Web) for a pilates franchise. A freelance project delivered and in production. Async backend with concurrency control to prevent double booking, credit validation, fixed slots with auto-booking, automatic account merge, push notifications and an administration panel. Deployed on a VPS with an operating cost of ~$4/month.

---

### [Inversiones en Argentina](https://github.com/IvanGomezDellOsa/Inversiones_Argentina)
`Python` `FastAPI` `Gemini API` `PostgreSQL` `GitHub Actions` `Next.js` `Telegram API`

Automated aggregator of private investments in Argentina. Weekly flow: scraping X via Apify → structuring with Gemini API + Google Search Grounding → semantic deduplication with pgvector → automatic publication on a Telegram channel via API → production deploy on Vercel.

🌐 [inversionesargentina.com.ar](https://inversionesargentina.com.ar)

---

### [FaceHunt](https://github.com/IvanGomezDellOsa/FaceHunt)
`Python` `DeepFace` `FaceNet` `RetinaFace` `FastAPI` `Docker`

A facial recognition system in video with deep learning that, from a reference image, generates a precise temporal index of appearances in a local video or YouTube. It includes an API with FastAPI and a dockerized web interface deployed on Hugging Face.

---

### [FreeMagicMirror](https://github.com/IvanGomezDellOsa/FreeMagicMirror)
`Python` `Kivy` `OpenCV` `PyInstaller`

A touch photobooth application with a multitouch image editor, animated counter and kiosk mode. Deployed in a real commercial environment and distributed as a portable executable (.exe) with no external dependencies.

---

### [RugidosWebSite](https://github.com/IvanGomezDellOsa/RugidosWebSite)
`Next.js` `TypeScript` `Tailwind CSS` `Framer Motion`

Second version of the commercial website of Rugidos Fiestas Tandil, currently in production. A complete redesign oriented toward a modern visual experience: animations, transitions, interactive gallery and responsive design. Optimized for mobile performance.

🌐 [rugidosfiestas.com.ar](https://www.rugidosfiestas.com.ar/)

---

### [RugidosWebSite 2023 (Legacy)](https://github.com/IvanGomezDellOsa/RugidosWebSite-2023-Legacy)
`HTML5` `CSS3` `JavaScript`

First version of the site, in production from 2023 until it was replaced by the current version. Built without frameworks, with automatic deploy to cPanel.

---

### [TexTok](https://github.com/IvanGomezDellOsa/TexTok---Universitario---Java)
`Java`

A data management engine in pure Java. Implements from scratch a BST, singly and doubly linked lists, cross references, recursion and full binary persistence with no frameworks or java.util.

---

## 📬 Contact

- **Email:** ivangomezdellosa@gmail.com
- **LinkedIn:** [linkedin.com/in/ivangomezdellosa](https://www.linkedin.com/in/ivangomezdellosa/)
