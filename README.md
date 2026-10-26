<div align="center">

<img src="assets/header.svg" width="100%" alt="Silvio Duarte · Matemático · Consultor de TI y de IA" />

<br />

[<img src="assets/badge-web.svg" alt="silvioduarte.com" height="34" />](https://silvioduarte.com)
[<img src="assets/badge-linkedin.svg" alt="LinkedIn" height="34" />](https://linkedin.com/in/silvioduarte)
[<img src="assets/badge-email.svg" alt="contacto@silvioduarte.com" height="34" />](mailto:contacto@silvioduarte.com)

📍 Managua, Nicaragua · 🇬🇧 [English version](./README.en.md)

</div>

## 👋 Quién soy

Soy matemático y consultor de TI con más de 12 años de trabajo en QA, infraestructura cloud/híbrida, Business Intelligence y desarrollo web.

Vengo del mundo de las olimpiadas de matemática: gané dos veces la olimpiada nacional de Nicaragua y obtuve menciones de honor en la Iberoamericana y la Centroamericana. Ahí aprendí lo que hasta hoy define mi trabajo: **entender el problema antes de tocar la solución**.

Esa base me llevó a la docencia (Academia Sabatina de Jóvenes Talento, capacitación a maestros del MINED, Data Analytics para instituciones públicas) y después a dirigir durante 10 años el proyecto **CODE de Fundación Uno**, en alianza con **Harvard CS50x**: un programa que forma a más de **940 estudiantes cada año** en ciencias de la computación, donde lideré el QA funcional de un equipo de **73 técnicos** bajo estándares de Harvard University.

Hoy trabajo como consultor independiente. Rescato plataformas en producción, audito seguridad y rendimiento, diseño infraestructura y construyo sistemas de datos para empresas que dependen de que su tecnología funcione todos los días. Cada vez más, ese trabajo pasa por conectar la operación real de una empresa con modelos de IA, de forma segura y medible.

## 🛠️ Qué hago

| Área | En la práctica |
|:-----|:---------------|
| **Consultoría TI & IA** | Diagnóstico tecnológico, arquitectura de soluciones, integración de IA en operaciones reales de negocio |
| **IA aplicada** | Servidores MCP para consultar sistemas en producción desde Claude con cuentas de solo lectura, agentes y skills a medida, flujos agénticos (encadenar, enrutar, RAG) |
| **QA & Debugging** | Pruebas funcionales (UAT), auditoría de código, debugging profundo para rescatar plataformas en producción |
| **Infraestructura & Cloud** | Servidores Linux/Windows, VPS (cPanel/WHM), entornos híbridos on-premise, VoIP cloud (3CX + Dinstar), Fortinet, Mikrotik |
| **Data & BI** | Dashboards ejecutivos web, SSRS, ETL de Excel a sistemas vivos, KPIs que la gerencia usa de verdad |
| **Desarrollo web y móvil** | Aplicaciones full stack (PHP, Laravel, Next.js/TypeScript, Node), PWAs instalables, apps Android nativas en Kotlin, portales con autenticación propia, WordPress experto |

## 🚀 Trabajo reciente

Sistemas diseñados y construidos de punta a punta, la mayoría ya en producción.

### Operación de una cadena de supermercados

- **Control de facturas de energía eléctrica** — cada mes llegan unas 110 facturas en PDF donde cada cifra es una imagen incrustada, no texto. El lector reconoce los dígitos contra un banco de 812 glifos calibrado a mano, sin OCR; valida cada valor contra el propio documento y contra el histórico, reparte el pago entre tarjetas de crédito y genera la plantilla de importación al ERP. Expone un servidor **MCP** de solo lectura con OAuth para consultar consumo, costos y pagos desde Claude. `PHP 8.5 · Python · SQL Server/MySQL · MCP`
- **Puerta única del ecosistema de mantenimiento** — une flota, energía, agua y refrigeración con inicio de sesión único, sin tocar cada sistema por dentro: los enlaces van con peticiones firmadas y todo dato personal se guarda cifrado con XChaCha20-Poly1305 (libsodium). Segundo factor TOTP y sin Composer. `PHP 8.5 · MySQL · libsodium`
- **Gestión de flota, refrigeración y plantas eléctricas** — recorrido y rendimiento de combustible, costo por km, preventivos y reemplazo de unidades, con sincronización de las APIs de combustible y GPS. Despliegue automático desde `main` en menos de cinco minutos, con la base migrada antes de copiar el código. `PHP 8.5 · MySQL`
- **Inspección de contenedores refrigerados** — app de patio que guía al inspector por 11 puntos con lógica condicional, funciona con señal intermitente (cola en IndexedDB) y avisa al gerente solo con los hallazgos. No tiene base de datos: cada inspección es un commit por la API de GitHub, y el historial de git es la auditoría. `Next.js 16 · TypeScript · Tailwind 4 · Vercel`
- **Portal de conocimiento operativo** — procesos, políticas, indicadores, reuniones, herramientas y formatos como documentos interconectados, ingeridos desde Excel, con flujogramas SVG interactivos, versionado por aprobación con diff campo a campo y perfiles de puesto generados solos. Escrito para migrar a .NET + SQL Server sin reescribir la lógica. `Laravel 13 · MySQL · Tailwind 4 · Alpine.js`
- **Plataforma de órdenes de trabajo de mantenimiento** (en equipo) — PWA sobre Business Central para todo el ciclo de mantenimiento de tiendas: órdenes de trabajo, cotizaciones a proveedores, contratos, cheques, anticipos, órdenes de compra y dashboards de SLA, con los manuales por rol integrados en la app. `Blazor · .NET · Business Central · Azure`
- **Sistema de gestión de solicitudes de cambio** — PWA multiproyecto con 4 roles y notificaciones push que llegan con la app cerrada. La criptografía Web Push (RFC 8291 + VAPID ES256) está implementada a mano con extensiones nativas de PHP: cero Composer, migrar la app es copiar archivos. `PHP 8 · SQLite/MySQL`
- **Dashboard de indicadores comerciales** — procesa respaldos de Excel de ~5,900 filas de 58 tiendas y calcula KPIs de ocupación y renta. El histórico vive versionado en un repo de GitHub: sin base de datos que mantener. `Next.js 14 · TypeScript · Tailwind · Recharts · Vercel`

### Productos propios

- **Dialens** — app Android que identifica a qué operador pertenece cualquier número de Centroamérica a partir de los rangos de numeración de cada regulador, sin enviar contactos ni llamadas a ningún servidor. Muestra el operador sobre la pantalla de llamada y bloquea números por prefijo antes de que suenen. Dependencias verificadas con huella SHA-256. `Kotlin · Jetpack Compose · Android`
- **Cerebro** — bóveda Obsidian que convierte cada sesión de trabajo con Claude Code en una nota con título, proyecto, temas y enlaces, y redacta las credenciales antes de guardarla. Más de 1,600 notas buscables, mapas de contenido por proyecto y tema, y un visor 3D del grafo que funciona sin internet. Es la memoria de decisiones de todos mis proyectos. `Python · Obsidian · 3d-force-graph`

### Clientes y consultoría

- **Fundación Uno · Archive & Vault** — dos plataformas privadas con un solo acceso entre ambas: el archivo institucional del legado de la Fundación y un repositorio documental que cataloga fotos (SmugMug), videos (YouTube) y archivos (Google Drive). Sin WordPress ni Composer, con 2FA y CSP. `PHP · MySQL · OAuth`
- **New Connections International** — sitio bilingüe de una agencia de movilidad internacional con sede en Irlanda, migrado de WordPress a PHP propio con panel de administración, rediseño de marca 2026, SEO/AEO/GEO y consentimiento RGPD con Consent Mode v2. `PHP · MySQL · SCSS`
- **[nekupe.com](https://nekupe.com)** — sitio de Nekupe Sporting Resort (Nandaime, Nicaragua): arquitectura de parciales PHP compartidos, panel de administración con galería drag-and-drop, SEO/GA4, despliegue FTPS. `PHP · AngularJS · MySQL · Bluehost`
- **Taller de Carpintería La Divina Providencia** — catálogo en línea, pedidos y gestión para un taller de artesanía franciscana y su tienda de artículos religiosos, con máquina de estados de pedidos y permisos por rol. `Laravel 12 · Livewire 3 · MySQL`

## 🎤 Talleres y charlas

- **«Diseño e implementación de flujos de trabajo agénticos»** — I Congreso de Inteligencia Artificial de la UNAH (Tegucigalpa, julio 2026). Notebooks progresivos sobre encadenar y enrutar prompts, RAG con ChromaDB y un servidor MCP propio, todo sobre endpoints gratuitos para que cualquiera lo reproduzca. Material en [silfdv/flujos-agenticos](https://github.com/silfdv/flujos-agenticos).

## 🧭 Cómo trabajo

- **Dependencias mínimas.** Varios de mis sistemas en producción funcionan sin Composer, sin npm y sin framework. Bajar la cantidad de dependencias reduce la superficie de ataque y hace que migrar el sistema sea prácticamente copiar archivos de un servidor a otro. Este mismo perfil de GitHub no consume ningún servicio externo: el banner, los iconos y los badges son archivos SVG que viven dentro del repositorio.
- **Seguridad desde el primer commit.** Contraseñas con hash fuerte, sesiones firmadas, segundo factor, datos personales cifrados en la base, archivos sensibles fuera del webroot y sanitización de entradas contra XSS. Lo defino en la arquitectura inicial del proyecto, antes de escribir la lógica de negocio.
- **Documentación en cada entrega.** Todo sistema que entrego incluye su README con la arquitectura, la guía de migración y un changelog versionado, para que otra persona pueda tomar el proyecto sin depender de mí.
- **Memoria de proyecto.** Cada decisión queda registrada en el Cerebro, así que cuando retomo un sistema meses después parto de lo que ya se decidió y por qué, no de cero.
- **IA aplicada con criterio.** Trabajo con Claude Code, agentes y skills propias en desarrollo, QA y documentación, y cada entrega pasa por una revisión adversarial antes de darla por buena. Reviso a fondo cada línea de código que lleva mi firma.

## 🧰 Stack

<div align="center">

**Lenguajes & Frontend**

<img src="assets/skills-1.svg" alt="TypeScript, JavaScript, PHP, Python, HTML, CSS, React, Next.js, Tailwind, AngularJS" />

**Backend, datos & infraestructura**

<img src="assets/skills-2.svg" alt="Node.js, MySQL, SQLite, Git, GitHub, Linux, Vercel, WordPress, LaTeX, VS Code" />

**Móvil, frameworks & nube**

<img src="assets/skills-3.svg" alt="Kotlin, Android Studio, Laravel, Alpine.js, .NET, Azure, Cloudflare, Obsidian, Postman, Windows" />

</div>

<br />

**Además** · SQL Server (SSRS) · Business Central · Jetpack Compose · Livewire · Excel avanzado (Power Query, VBA, macros) · PWA & Web Push · libsodium · cPanel/WHM · DNS · 3CX · Fortinet · Mikrotik · Model Context Protocol (MCP) · Claude Code, agentes y flujos de trabajo con LLM en desarrollo, QA y análisis de datos

## 🏅 Reconocimientos

- 🥇 Ganador de la **Olimpiada Nacional de Matemática de Nicaragua** (2007 y 2009)
- 🌎 **Mención de Honor** — Olimpiada Iberoamericana de Matemáticas (México 2009, Paraguay 2010)
- 🌎 **Mención de Honor** — Olimpiada Matemática de Centroamérica y el Caribe (Honduras 2008)
- 🏛️ Comité organizador de la 15.ª Olimpiada Matemática de Centroamérica y el Caribe (2013)
- 🎓 Co-fundador de la comisión de tecnología de la **Olimpiada Matemática Nicaragüense**

## 📫 Hablemos

¿Tenés una plataforma que rescatar, datos que no dicen nada o una operación que querés conectar con IA? Escribime.

**[contacto@silvioduarte.com](mailto:contacto@silvioduarte.com)** · **[silvioduarte.com](https://silvioduarte.com)** · **[linkedin.com/in/silvioduarte](https://linkedin.com/in/silvioduarte)**

<div align="center">

<img src="assets/footer.svg" width="100%" alt="" />

<sub>Silvio Duarte · Matemático · Consultor de IT y de IA</sub>

</div>
