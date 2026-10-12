[Español](README.md) | [English](README.en.md)

<h1 align="center">Iván Gómez Dell'Osa</h1>

<p align="center">
  <em>Full Stack Developer · Backend · Inteligencia Artificial Aplicada</em>
</p>

<p align="center">
  🌐 <a href="https://www.ivangomezdellosa.com.ar"><strong>ivangomezdellosa.com.ar</strong></a>
</p>

---

Desarrollo productos de software completos, desde el diseño hasta la puesta en producción, con foco en backend e inteligencia artificial aplicada. Tengo proyectos propios y freelance en producción, con clientes y usuarios reales.

Sobre la base que me da la carrera de Ingeniería de Sistemas (lógica de programación, análisis matemático y diseño de algoritmos), trabajo de forma autodidacta con tecnologías actuales. Lo combino con la gestión operativa de una PyME, donde sumo conocimientos de administración de empresas, producto y manejo de equipos.

---

## 🛠 Proyectos

### [Ask Leonardo da Vinci](https://github.com/IvanGomezDellOsa/Ask_Leonardo_da_Vinci)
`Next.js` `React` `TypeScript` `Three.js` `RAG` `Transformers.js` `Gemini API` `Python`

**Leonardo da Vinci dejó más de 7.500 páginas escritas. Por primera vez, un software las utiliza para conversar con él sin inventar respuestas.**

El proyecto nace de cruzar dos datos. Una IA que simula ser una persona real inventa hasta su manera de expresarse y le atribuye frases que nunca dijo; para evitarlo, esa persona tendría que haber dejado por escrito un contexto enorme de sí misma, y casi nadie lo tiene. Leonardo es una excepción: durante toda su vida hizo una especie de *transfusión mental a papel*. El sistema consulta los 1.565 pasajes que Jean Paul Richter transcribió y tradujo en 1888.

Cruzar esos datos fue el punto de partida, no el resultado. El pipeline RAG está escrito desde cero: recuperación híbrida, un filtro que decide si los cuadernos tratan el tema y la comprobación de que cada cita exista en el pasaje original. Con el mismo modelo y las mismas preguntas, una IA actuando como Leonardo inventa el **96,9%** de sus citas (156 de 161); Ask Leonardo da Vinci, **0 de 187**. Incluye además una biblioteca 3D, un museo virtual 3D y un espacio vectorial que muestra cómo una pregunta encuentra sus pasajes.

🌐 [askleonardodavinci.online](https://www.askleonardodavinci.online) (ES / EN)

🎬 [Video de presentación](https://youtu.be/35xaHDucoX8)

---

### [Inversiones en Argentina](https://github.com/IvanGomezDellOsa/Inversiones_Argentina)
`Python` `FastAPI` `Gemini API` `Jev (TypeSafe)` `PostgreSQL` `pgvector` `GitHub Actions` `Next.js` `Telegram API`

Las inversiones privadas que se anuncian en Argentina estaban dispersas en noticias, cuentas de X y registros oficiales. El proyecto automatiza la recolección y la publicación de esa información: cada 72 horas, un flujo programado en GitHub Actions reúne material de diversas fuentes y rastrea con Gemini y Search Grounding las menciones de inversiones publicadas en la web. Un sistema de capas define qué llega a publicarse: Gemini estructura cada mención, pgvector recupera los registros más parecidos y reglas de identidad junto con Jev (TypeSafe) resuelven qué es una inversión real y qué ya está publicado bajo otro nombre. Se publica sin intervención en la web y en un canal de Telegram, con API en FastAPI y frontend en Next.js con render en servidor, sobre Vercel.

🌐 [inversionesargentina.com.ar](https://inversionesargentina.com.ar)

🎬 [Video de presentación](https://youtu.be/aFhefFVcW4M)

---

### [Datos Pauta Oficial](https://github.com/IvanGomezDellOsa/DatosPautaOficial)
`Python` `ETL` `SQLite` `Astro` `React` `TypeScript` `Cloudflare R2/Pages`

La primera y única base unificada de pauta oficial argentina: **540.413 órdenes de publicidad** de cuatro jurisdicciones (Nación, CABA, PBA y Santa Fe), período 2003–2025, con montos deflactados por IPC para que las cifras sean comparables entre años. ETL propio en Python que incluye un **dataset exclusivo de PBA 2020–2024 reconstruido procesando más de 500 resoluciones en PDF** (datos que no existen en ningún portal de datos abiertos). Arquitectura 100% sin backend: la base SQLite (~173 MB) vive en Cloudflare R2 y el navegador consulta solo los bytes que necesita vía HTTP Range Requests (`sql.js-httpvfs`).

🌐 [datospautaoficial.com.ar](https://datospautaoficial.com.ar)

🎬 [Video de presentación](https://youtu.be/o8Ht_Qv4Ji4)

---

### [FaceHunt 2](https://github.com/IvanGomezDellOsa/FaceHunt-2)
`Python` `InsightFace` `ArcFace` `ONNX Runtime` `FastAPI` `pywebview`

Aplicación de escritorio 100% local que, a partir de una o varias fotos de referencia, usa reconocimiento facial para detectar cada aparición de una persona en un video (archivo local o URL de YouTube). Cada una se devuelve como un rango de tiempo exacto, con miniatura, mini-clip animado y salto directo al momento. Evolución de mi proyecto anterior FaceHunt, que reconstruí por completo: pasó de TensorFlow en CPU a ONNX Runtime con GPU y de FaceNet (128 dimensiones) a ArcFace (512), con seguimiento entre cuadros que recupera apariciones con el rostro de perfil, parcialmente cubierto o en baja resolución. Se usa con un ejecutable de un clic, sin servidor ni nube.

🎬 [Video de presentación](https://www.youtube.com/watch?v=huNRQiAW_ss)

**Primera versión: [FaceHunt](https://github.com/IvanGomezDellOsa/FaceHunt) (2025)** · `Python` `DeepFace` `FaceNet` `RetinaFace` `FastAPI` `Docker`<br>
Sistema de reconocimiento facial en video con deep learning, con API en FastAPI e interfaz web en Docker.

---

### [SeViVe (ex Pilates All Canning)](https://github.com/IvanGomezDellOsa/PilatesAllCanning_App)
`Flutter` `Python` `FastAPI` `PostgreSQL` `Firebase` `Docker` `Nginx`

Proyecto freelance: aplicación de reservas y gestión para un estudio de pilates (franquicia), con más de 200 usuarios. La desarrollé como único programador, desde la captación del cliente y la definición de requisitos hasta la puesta en producción. Reservas con control de concurrencia para evitar sobrerreservas, créditos con vencimiento, turnos fijos con reserva automática y calendario con feriados configurables. Las cuentas creadas por la administración se unifican automáticamente con la del alumno al registrarse (por DNI), preservando historial, créditos y turnos. Backend asíncrono con Python, FastAPI y PostgreSQL; aplicación en Flutter instalable como PWA, con autenticación de Google mediante Firebase. Docker Compose y Nginx en un VPS que administro. Finalizado el desarrollo, continúo a cargo del soporte, la administración del servidor y las actualizaciones solicitadas por el cliente.

🎬 [Video de presentación](https://www.youtube.com/watch?v=nI6Iz2L-hFs)

---

### [Navkok Security Group SRL · Sitio corporativo](https://github.com/IvanGomezDellOsa/NavkokSecurityGroup_Website)
`Next.js` `TypeScript` `Tailwind CSS`

Proyecto freelance: rediseño completo del sitio corporativo de una empresa de seguridad con más de 30 años de trayectoria y certificaciones ISO 9001, 14001 y 45001. Lo desarrollé de punta a punta (arquitectura de información, diseño UX/UI, redacción de los textos institucionales y desarrollo), con foco en un diseño de alto impacto que transmita su experiencia y sus credenciales.

🌐 [Vista previa del sitio](https://navkok-website-private.vercel.app/)

---

### [MementoLife](https://github.com/IvanGomezDellOsa/MementoLife)
`TypeScript` `Chrome Extensions` `Manifest V3` `SVG` `Vitest` `Playwright`

Extensión de Chrome, publicada en la Chrome Web Store, que reemplaza la pestaña nueva por una grilla con las semanas de la vida calculada a partir de la fecha de nacimiento, y suma una efeméride histórica para cada día del año. Interfaz completa en 6 idiomas, sin conexiones de red y con un solo permiso. TypeScript estricto, sin framework ni bundler: la grilla de 4.160 semanas se dibuja con 3 trazados SVG en vez de un elemento por celda (1,30 ms contra 10,00 ms).

🧩 [Chrome Web Store](https://chromewebstore.google.com/detail/mementolife/eackmngdibobdeciapcedkmjoecaiblp)

🎬 [Video de presentación](https://youtu.be/tZbJvq8xoBk)

---

### [FreeMagicMirror](https://github.com/IvanGomezDellOsa/FreeMagicMirror)
`Python` `Kivy` `OpenCV` `PyInstaller`

Aplicación de fotomatón táctil con editor multitáctil de imágenes, cuenta regresiva animada y modo kiosco. Desplegada en entorno comercial real y distribuida como ejecutable (.exe) portable sin dependencias externas.

🎬 [Video de presentación](https://www.youtube.com/watch?v=UjSz98p7nPk)

---

### [RugidosWebSite](https://github.com/IvanGomezDellOsa/RugidosWebSite)
`Next.js` `TypeScript` `Tailwind CSS` `Framer Motion`

Sitio comercial de Rugidos Fiestas Tandil, en producción, mobile first y optimizado para búsquedas locales. Rediseño integral en 2026, con diseño UX/UI propio. Lighthouse sobre el sitio en producción: 95 de rendimiento en móvil y 99 en escritorio.

🌐 [rugidosfiestas.com.ar](https://www.rugidosfiestas.com.ar/)

**Primera versión: [RugidosWebSite 2023 (Legacy)](https://github.com/IvanGomezDellOsa/RugidosWebSite-2023-Legacy)** · `HTML5` `CSS3` `JavaScript`<br>
En producción desde 2023 hasta ser reemplazada por la versión actual. Construida sin frameworks, con deploy automático a cPanel.

---

## 📬 Contacto

- **Web:** [ivangomezdellosa.com.ar](https://www.ivangomezdellosa.com.ar)
- **Email:** ivangomezdellosa@gmail.com
- **LinkedIn:** [linkedin.com/in/ivangomezdellosa](https://www.linkedin.com/in/ivangomezdellosa/)
