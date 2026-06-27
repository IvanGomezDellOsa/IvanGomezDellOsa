[Español](README.md) | [English](README.en.md)

<h1 align="center">Iván Gómez Dell'Osa</h1>

<p align="center">
  <em>Ingeniería de Sistemas · Backend · Inteligencia Artificial Aplicada</em>
</p>

---

Curso Ingeniería de Sistemas con foco en backend e inteligencia artificial aplicada. Tengo proyectos propios en producción y experiencia freelance entregando software a clientes reales.

Trabajo de forma autodidacta con tecnologías actuales y estudio constante de producto y mercados, sobre una base de fundamentos sólidos que aporta la carrera (lógica de programación, análisis matemático y diseño de algoritmos). Lo combino con la gestión operativa de una PyME, donde desarrollé interés en la gestión de negocio, producto y equipos.

---

## 🛠 Proyectos

### [Datos Pauta Oficial](https://github.com/IvanGomezDellOsa/DatosPautaOficial)
`Python` `ETL` `SQLite` `Astro` `React` `TypeScript` `Cloudflare R2/Pages`

La primera y única base unificada de pauta oficial argentina: **540.413 órdenes de publicidad** de cuatro jurisdicciones (Nación, CABA, PBA y Santa Fe), período 2003–2025, con montos deflactados por IPC para que las cifras sean comparables entre años. ETL propio en Python que incluye un **dataset exclusivo de PBA 2020–2024 reconstruido procesando más de 500 resoluciones en PDF** —datos que no existen en ningún portal de datos abiertos—. Arquitectura 100% sin backend: la base SQLite (~173 MB) vive en Cloudflare R2 y el navegador consulta solo los bytes que necesita vía HTTP Range Requests (`sql.js-httpvfs`). Costo operativo ≈ $0.

🌐 [datospautaoficial.com.ar](https://datospautaoficial.com.ar)

---

### [Navkok Security Group SRL — Sitio Corporativo](https://github.com/IvanGomezDellOsa/NavkokSecurityGroup_Website) *(En curso)*
`Next.js` `TypeScript` `Tailwind CSS`

Rediseño completo del sitio corporativo de una empresa de seguridad con más de 30 años de trayectoria y certificaciones ISO 9001, 14001 y 45001. Foco en diseño de alto impacto que refleje su trayectoria y credenciales. Deploy a cargo.

🌐 [Navkok](https://navkok-website-private.vercel.app/)

---

### [PilatesAllCanning](https://github.com/IvanGomezDellOsa/PilatesAllCanning_App)
`Flutter` `Python` `FastAPI` `PostgreSQL` `Firebase` `Docker`

App de gestión multiplataforma (iOS, Android, Web) para franquicia de pilates. Proyecto freelance entregado y en producción. Backend asíncrono con control de concurrencia para evitar doble reserva, validación de créditos, turnos fijos con auto-booking, merge automático de cuentas, notificaciones push y panel administrativo. Deploy en VPS con costo operativo de ~$4/mes.

---

### [Inversiones en Argentina](https://github.com/IvanGomezDellOsa/Inversiones_Argentina)
`Python` `FastAPI` `Gemini API` `PostgreSQL` `GitHub Actions` `Next.js` `Telegram API`

Agregador automatizado de inversiones privadas en Argentina. Flujo semanal: scraping de X vía Apify → estructuración con Gemini API + Google Search Grounding → deduplicación semántica con pgvector → publicación automática en canal de Telegram vía API → deploy en producción en Vercel.

🌐 [inversionesargentina.com.ar](https://inversionesargentina.com.ar)

---

### [FaceHunt 2](https://github.com/IvanGomezDellOsa/FaceHunt-2)
`Python` `InsightFace` `ArcFace` `ONNX Runtime` `FastAPI` `pywebview`

Aplicación de escritorio 100% local que, a partir de una o varias fotos de referencia, usa reconocimiento facial para detectar cada aparición de una persona en un video (archivo local o URL de YouTube) y la devuelve como rangos de tiempo exactos, cada uno con miniatura, mini-clip animado y salto directo al momento. Evolución de mi proyecto anterior FaceHunt, que reconstruí por completo: ~10x más rápido (ONNX Runtime con GPU y tracking temporal), mayor precisión (ArcFace 512-d) y ejecutable de un clic, sin servidor ni nube.

🎬 [Demo en YouTube](https://www.youtube.com/watch?v=rJLyYJcEm7c)

---

### [FaceHunt](https://github.com/IvanGomezDellOsa/FaceHunt)
`Python` `DeepFace` `FaceNet` `RetinaFace` `FastAPI` `Docker`

Primera versión de FaceHunt: sistema de reconocimiento facial en video con deep learning, con API en FastAPI e interfaz web dockerizada desplegada en Hugging Face. Posteriormente lo reconstruí por completo en FaceHunt 2 (arriba), ~10x más rápido y más preciso.

---

### [FreeMagicMirror](https://github.com/IvanGomezDellOsa/FreeMagicMirror)
`Python` `Kivy` `OpenCV` `PyInstaller`

Aplicación de fotomatón táctil con editor multitáctil de imágenes, contador animado y modo kiosco. Desplegada en entorno comercial real y distribuida como ejecutable (.exe) portable sin dependencias externas.

---

### [RugidosWebSite](https://github.com/IvanGomezDellOsa/RugidosWebSite)
`Next.js` `TypeScript` `Tailwind CSS` `Framer Motion`

Segunda versión del sitio comercial de Rugidos Fiestas Tandil, actualmente en producción. Rediseño completo orientado a una experiencia visual moderna: animaciones, transiciones, galería interactiva y diseño responsivo. Optimizado para performance en mobile.

🌐 [rugidosfiestas.com.ar](https://www.rugidosfiestas.com.ar/)

---

### [RugidosWebSite 2023 (Legacy)](https://github.com/IvanGomezDellOsa/RugidosWebSite-2023-Legacy)
`HTML5` `CSS3` `JavaScript`

Primera versión del sitio, en producción desde 2023 hasta ser reemplazada por la versión actual. Construida sin frameworks, con deploy automático a cPanel.

---

### [TexTok](https://github.com/IvanGomezDellOsa/TexTok---Universitario---Java)
`Java`

Motor de gestión de datos en Java puro. Implementa desde cero ABB, listas enlazadas simples y dobles, referencias cruzadas, recursión y persistencia binaria total sin frameworks ni java.util.

---

## 📬 Contacto

- **Email:** ivangomezdellosa@gmail.com
- **LinkedIn:** [linkedin.com/in/ivangomezdellosa](https://www.linkedin.com/in/ivangomezdellosa/)
