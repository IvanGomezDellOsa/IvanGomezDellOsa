[Español](README.md) | [English](README.en.md)

<h1 align="center">Iván Gómez Dell'Osa</h1>

<p align="center">
  <em>Ingeniería de Sistemas · Backend · Inteligencia Artificial Aplicada</em>
</p>

---

Curso Ingeniería de Sistemas con foco en backend e inteligencia artificial aplicada. Tengo proyectos propios en producción y experiencia freelance entregando software a clientes reales.

Trabajo de forma autodidacta con tecnologías actuales y estudio constante de producto y mercados, sobre la base que me da la carrera (lógica de programación, análisis matemático y diseño de algoritmos). Lo combino con la gestión operativa de una PyME, donde sumo conocimientos de administración de empresas, producto y manejo de equipos.

---

## 🛠 Proyectos

### [Ask Leonardo da Vinci](https://github.com/IvanGomezDellOsa/Ask_Leonardo_da_Vinci)
`Next.js` `React` `TypeScript` `Three.js` `RAG` `Transformers.js` `Gemini API` `Python`

**Leonardo da Vinci dejó más de 7.500 páginas escritas. Por primera vez, un software las utiliza para conversar con él sin inventar respuestas.**

El proyecto nace de cruzar dos datos. Una IA que simula ser una persona real inventa hasta su manera de expresarse y le atribuye frases que nunca dijo; para evitarlo, esa persona tendría que haber dejado por escrito un contexto enorme de sí misma, y casi nadie lo tiene. Leonardo es una excepción: durante toda su vida hizo una especie de *transfusión mental a papel*. El sistema consulta los 1.565 pasajes que Jean Paul Richter transcribió y tradujo en 1888.

Cruzar esos datos fue el punto de partida, no el resultado. El pipeline RAG está escrito desde cero: recuperación híbrida, un filtro que decide si los cuadernos tratan el tema y la comprobación de que cada cita exista en el pasaje original. Con el mismo modelo y las mismas preguntas, una IA actuando como Leonardo inventa el **96,9%** de sus citas (156 de 161); Ask Leonardo da Vinci, **0 de 187**. Incluye además una biblioteca 3D, un museo virtual 3D y un espacio vectorial que muestra cómo una pregunta encuentra sus pasajes. Costo de operación: US$0.

🌐 [askleonardodavinci.online](https://www.askleonardodavinci.online) (ES / EN)

---

### [Datos Pauta Oficial](https://github.com/IvanGomezDellOsa/DatosPautaOficial)
`Python` `ETL` `SQLite` `Astro` `React` `TypeScript` `Cloudflare R2/Pages`

La primera y única base unificada de pauta oficial argentina: **540.413 órdenes de publicidad** de cuatro jurisdicciones (Nación, CABA, PBA y Santa Fe), período 2003–2025, con montos deflactados por IPC para que las cifras sean comparables entre años. ETL propio en Python que incluye un **dataset exclusivo de PBA 2020–2024 reconstruido procesando más de 500 resoluciones en PDF** (datos que no existen en ningún portal de datos abiertos). Arquitectura 100% sin backend: la base SQLite (~173 MB) vive en Cloudflare R2 y el navegador consulta solo los bytes que necesita vía HTTP Range Requests (`sql.js-httpvfs`). Costo de operación: US$0.

🌐 [datospautaoficial.com.ar](https://datospautaoficial.com.ar)

---

### [Navkok Security Group SRL — Sitio Corporativo](https://github.com/IvanGomezDellOsa/NavkokSecurityGroup_Website)
`Next.js` `TypeScript` `Tailwind CSS`

Proyecto freelance: rediseño completo del sitio corporativo de una empresa de seguridad con más de 30 años de trayectoria y certificaciones ISO 9001, 14001 y 45001. Lo desarrollé de punta a punta —arquitectura de información, diseño UX/UI, redacción de los textos institucionales y desarrollo—, con foco en un diseño de alto impacto que transmita su experiencia y sus credenciales.

🌐 [Vista previa del sitio](https://navkok-website-private.vercel.app/)

---

### [PilatesAllCanning](https://github.com/IvanGomezDellOsa/PilatesAllCanning_App)
`Flutter` `Python` `FastAPI` `PostgreSQL` `Firebase` `Docker`

App de gestión multiplataforma (iOS, Android, Web) para una franquicia de pilates. Proyecto freelance entregado y en producción. Backend asíncrono con control de concurrencia para evitar doble reserva, validación de créditos, turnos fijos con auto-booking, unificación automática de cuentas, notificaciones push y panel administrativo. Deploy en VPS con un costo de operación de unos US$4 por mes.

🎬 [Demo en YouTube](https://www.youtube.com/watch?v=EVlTbLLV_NU)

---

### [Inversiones en Argentina](https://github.com/IvanGomezDellOsa/Inversiones_Argentina)
`Python` `FastAPI` `Gemini API` `Jev (TypeSafe)` `PostgreSQL` `pgvector` `GitHub Actions` `Next.js` `Telegram API`

Reúne en una cronología las inversiones privadas realizadas o anunciadas en Argentina, un dato que estaba disperso en noticias, cuentas de X y registros oficiales. Cada 72 horas, un flujo en GitHub Actions recolecta de cuatro tipos de fuente —cuentas de X vía Apify, seis medios por RSS, el registro oficial RIGI del Ministerio de Economía y Google con Gemini Search Grounding— y Gemini estructura cada inversión. La decisión final no la toma el modelo generativo: Gemini no ve la base, así que filtros deterministas y **Jev**, que devuelve decisiones tipadas con probabilidad calibrada, descartan lo que no corresponde y resuelven, sobre los candidatos que recupera pgvector, si dos noticias hablan del mismo proyecto — **el rediseño pasó de detectar 0 de 12 duplicados reales a 10, sin falsos positivos**. Publicación automática en la web y en Telegram, con API en FastAPI y frontend en Next.js con render en servidor, en Vercel.

🌐 [inversionesargentina.com.ar](https://inversionesargentina.com.ar)

---

### [FaceHunt 2](https://github.com/IvanGomezDellOsa/FaceHunt-2)
`Python` `InsightFace` `ArcFace` `ONNX Runtime` `FastAPI` `pywebview`

Aplicación de escritorio 100% local que, a partir de una o varias fotos de referencia, usa reconocimiento facial para detectar cada aparición de una persona en un video (archivo local o URL de YouTube). Cada una se devuelve como un rango de tiempo exacto, con miniatura, mini-clip animado y salto directo al momento. Evolución de mi proyecto anterior FaceHunt, que reconstruí por completo: ~10x más rápido (ONNX Runtime con GPU y tracking temporal), mayor precisión (ArcFace 512-d) y ejecutable de un clic, sin servidor ni nube.

🎬 [Demo en YouTube](https://www.youtube.com/watch?v=rJLyYJcEm7c)

**Primera versión: [FaceHunt](https://github.com/IvanGomezDellOsa/FaceHunt) (2025)** · `Python` `DeepFace` `FaceNet` `RetinaFace` `FastAPI` `Docker`<br>
Sistema de reconocimiento facial en video con deep learning, con API en FastAPI e interfaz web dockerizada desplegada en Hugging Face.

---

### [MementoLife](https://github.com/IvanGomezDellOsa/MementoLife)
`TypeScript` `Chrome Extensions` `Manifest V3` `SVG` `Vitest` `Playwright`

Extensión de Chrome, publicada en la Chrome Web Store, que reemplaza la pestaña nueva por una grilla con las semanas de la vida calculada a partir de la fecha de nacimiento, y suma una efeméride histórica para cada día del año. Interfaz completa en 6 idiomas, sin conexiones de red y con un solo permiso. TypeScript estricto, sin framework ni bundler: la grilla de 4.160 semanas se dibuja con 7 nodos del DOM en vez de uno por celda (1,30 ms contra 10,00 ms).

🧩 [Chrome Web Store](https://chromewebstore.google.com/detail/mementolife/eackmngdibobdeciapcedkmjoecaiblp)

---

### [FreeMagicMirror](https://github.com/IvanGomezDellOsa/FreeMagicMirror)
`Python` `Kivy` `OpenCV` `PyInstaller`

Aplicación de fotomatón táctil con editor multitáctil de imágenes, cuenta regresiva animada y modo kiosco. Desplegada en entorno comercial real y distribuida como ejecutable (.exe) portable sin dependencias externas.

🎬 [Demo en YouTube](https://www.youtube.com/watch?v=V_Qmx1kqg2M)

---

### [RugidosWebSite](https://github.com/IvanGomezDellOsa/RugidosWebSite)
`Next.js` `TypeScript` `Tailwind CSS` `Framer Motion`

Segunda versión del sitio comercial de Rugidos Fiestas Tandil, actualmente en producción. Rediseño completo orientado a una experiencia visual moderna: animaciones, transiciones, galería interactiva y diseño responsivo. Optimizado para performance en mobile.

🌐 [rugidosfiestas.com.ar](https://www.rugidosfiestas.com.ar/)

**Primera versión: [RugidosWebSite 2023 (Legacy)](https://github.com/IvanGomezDellOsa/RugidosWebSite-2023-Legacy)** · `HTML5` `CSS3` `JavaScript`<br>
En producción desde 2023 hasta ser reemplazada por la versión actual. Construida sin frameworks, con deploy automático a cPanel.

---

### [TexTok](https://github.com/IvanGomezDellOsa/TexTok---Universitario---Java)
`Java`

Motor de gestión de datos en Java puro, desarrollado como trabajo de la carrera. Implementa desde cero ABB, listas enlazadas simples y dobles, referencias cruzadas, recursión y persistencia en archivos binarios, sin frameworks ni java.util.

---

## 📬 Contacto

- **Email:** ivangomezdellosa@gmail.com
- **LinkedIn:** [linkedin.com/in/ivangomezdellosa](https://www.linkedin.com/in/ivangomezdellosa/)
