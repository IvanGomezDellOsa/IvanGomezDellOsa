[English](README.en.md) | [Español](README.md)

<h1 align="center">Iván Gómez Dell'Osa</h1>

<p align="center">
  <em>Systems Engineering · Backend · Applied Artificial Intelligence</em>
</p>

---

I am studying Systems Engineering with a focus on backend and applied artificial intelligence. I have my own projects in production and freelance experience delivering software to real clients.

I am self-taught in current technologies and constantly study product and markets, building on the foundation my degree gives me (programming logic, mathematical analysis and algorithm design). I combine this with running the operations of a small business, where I am gaining knowledge of business administration, product and team management.

---

## 🛠 Projects

### [Ask Leonardo da Vinci](https://github.com/IvanGomezDellOsa/Ask_Leonardo_da_Vinci)
`Next.js` `React` `TypeScript` `Three.js` `RAG` `Transformers.js` `Gemini API` `Python`

**Leonardo da Vinci left more than 7,500 written pages. For the first time, software uses them to speak with him without inventing answers.**

The project comes from putting two facts together. An AI that simulates a real person makes up even the way they express themselves and attributes to them phrases they never said; to avoid it, the person would have had to leave behind an enormous written context of themselves, and almost nobody has anything like that. Leonardo is an exception: throughout his life he made a kind of *mind transfusion onto paper*. The system searches the 1,565 passages that Jean Paul Richter transcribed and translated in 1888.

Putting those facts together was the starting point, not the result. The RAG pipeline is written from scratch: hybrid retrieval, a filter that decides whether the notebooks cover the subject, and a check that every quotation exists in the original passage. With the same model and the same questions, an AI acting as Leonardo makes up **96.9%** of its quotations (156 of 161); Ask Leonardo da Vinci, **0 of 187**. It also includes a 3D library, a 3D virtual museum and a vector space that shows how a question finds its passages. Operating cost: US$0.

🌐 [askleonardodavinci.online](https://www.askleonardodavinci.online/en) (EN / ES)

---

### [Datos Pauta Oficial](https://github.com/IvanGomezDellOsa/DatosPautaOficial)
`Python` `ETL` `SQLite` `Astro` `React` `TypeScript` `Cloudflare R2/Pages`

The first and only unified database of Argentine official advertising spending: **540,413 advertising orders** from four jurisdictions (Nación, CABA, PBA and Santa Fe), covering 2003–2025, with amounts adjusted for inflation (CPI) so the figures are comparable across years. A custom ETL in Python that includes an **exclusive PBA 2020–2024 dataset reconstructed by processing more than 500 PDF resolutions** (data that does not exist in any open data portal). A 100% backendless architecture: the SQLite database (~173 MB) lives on Cloudflare R2 and the browser queries only the bytes it needs via HTTP Range Requests (`sql.js-httpvfs`). Operating cost: US$0.

🌐 [datospautaoficial.com.ar](https://datospautaoficial.com.ar)

---

### [Navkok Security Group SRL — Corporate Website](https://github.com/IvanGomezDellOsa/NavkokSecurityGroup_Website)
`Next.js` `TypeScript` `Tailwind CSS`

Freelance project: a complete redesign of the corporate website of a security company with over 30 years of experience and ISO 9001, 14001 and 45001 certifications. I built it end to end, with a focus on high-impact design that conveys its track record and credentials.

🌐 [Site preview](https://navkok-website-private.vercel.app/)

---

### [PilatesAllCanning](https://github.com/IvanGomezDellOsa/PilatesAllCanning_App)
`Flutter` `Python` `FastAPI` `PostgreSQL` `Firebase` `Docker`

A multiplatform management app (iOS, Android, Web) for a pilates franchise. A freelance project delivered and in production. Async backend with concurrency control to prevent double booking, credit validation, fixed slots with auto-booking, automatic account merging, push notifications and an administration panel. Deployed on a VPS with an operating cost of about US$4 per month.

🎬 [Demo on YouTube](https://www.youtube.com/watch?v=EVlTbLLV_NU)

---

### [Inversiones en Argentina](https://github.com/IvanGomezDellOsa/Inversiones_Argentina)
`Python` `FastAPI` `Gemini API` `PostgreSQL` `GitHub Actions` `Next.js` `Telegram API`

Brings together, in a timeline, the private investments made or announced in Argentina. Every 72 hours an automated GitHub Actions workflow runs: scraping X via Apify → structuring with Gemini API + Google Search Grounding → semantic deduplication with pgvector → automatic publication on the website and on a Telegram channel. FastAPI API and Next.js frontend, deployed on Vercel.

🌐 [inversionesargentina.com.ar](https://inversionesargentina.com.ar)

---

### [FaceHunt 2](https://github.com/IvanGomezDellOsa/FaceHunt-2)
`Python` `InsightFace` `ArcFace` `ONNX Runtime` `FastAPI` `pywebview`

100% local desktop app that, from one or more reference photos, uses facial recognition to detect every appearance of a person in a video (local file or YouTube URL). Each one is returned as an exact time range, with a thumbnail, an animated mini-clip and a direct jump to the moment. Evolution of my earlier project FaceHunt, which I fully rebuilt: ~10x faster (ONNX Runtime with GPU and temporal tracking), higher accuracy (ArcFace 512-d) and a one-click executable, with no server or cloud.

🎬 [Demo on YouTube](https://www.youtube.com/watch?v=rJLyYJcEm7c)

**First version: [FaceHunt](https://github.com/IvanGomezDellOsa/FaceHunt) (2025)** · `Python` `DeepFace` `FaceNet` `RetinaFace` `FastAPI` `Docker`<br>
A deep learning facial recognition system for video, with a FastAPI API and a dockerized web interface deployed on Hugging Face.

---

### [MementoLife](https://github.com/IvanGomezDellOsa/MementoLife)
`TypeScript` `Chrome Extensions` `Manifest V3` `SVG` `Vitest` `Playwright`

A Chrome extension, published on the Chrome Web Store, that replaces the new tab with a grid of the weeks of your life calculated from your date of birth, plus a historical event for every day of the year. Full interface in 6 languages, no network connections and a single permission. Strict TypeScript with no framework or bundler: the 4,160-week grid is drawn with 7 DOM nodes instead of one per cell (1.30 ms versus 10.00 ms).

🧩 [Chrome Web Store](https://chromewebstore.google.com/detail/mementolife/eackmngdibobdeciapcedkmjoecaiblp)

---

### [FreeMagicMirror](https://github.com/IvanGomezDellOsa/FreeMagicMirror)
`Python` `Kivy` `OpenCV` `PyInstaller`

A touch photobooth application with a multitouch image editor, animated countdown and kiosk mode. Deployed in a real commercial environment and distributed as a portable executable (.exe) with no external dependencies.

🎬 [Demo on YouTube](https://www.youtube.com/watch?v=V_Qmx1kqg2M)

---

### [RugidosWebSite](https://github.com/IvanGomezDellOsa/RugidosWebSite)
`Next.js` `TypeScript` `Tailwind CSS` `Framer Motion`

Second version of the commercial website of Rugidos Fiestas Tandil, currently in production. A complete redesign oriented toward a modern visual experience: animations, transitions, interactive gallery and responsive design. Optimized for mobile performance.

🌐 [rugidosfiestas.com.ar](https://www.rugidosfiestas.com.ar/)

**First version: [RugidosWebSite 2023 (Legacy)](https://github.com/IvanGomezDellOsa/RugidosWebSite-2023-Legacy)** · `HTML5` `CSS3` `JavaScript`<br>
In production from 2023 until it was replaced by the current version. Built without frameworks, with automatic deploy to cPanel.

---

### [TexTok](https://github.com/IvanGomezDellOsa/TexTok---Universitario---Java)
`Java`

A data management engine in pure Java, built as a university project. Implements from scratch a BST, singly and doubly linked lists, cross references, recursion and binary file persistence, with no frameworks or java.util.

---

## 📬 Contact

- **Email:** ivangomezdellosa@gmail.com
- **LinkedIn:** [linkedin.com/in/ivangomezdellosa](https://www.linkedin.com/in/ivangomezdellosa/)
