<div align="center">

<img src="assets/header-en.svg" width="100%" alt="Silvio Duarte · Mathematician · IT & AI Consultant" />

<br />

[<img src="assets/badge-web.svg" alt="silvioduarte.com" height="34" />](https://silvioduarte.com)
[<img src="assets/badge-linkedin.svg" alt="LinkedIn" height="34" />](https://linkedin.com/in/silvioduarte)
[<img src="assets/badge-email.svg" alt="contacto@silvioduarte.com" height="34" />](mailto:contacto@silvioduarte.com)

📍 Managua, Nicaragua · 🇪🇸 [Versión en español](./README.md)

</div>

## 👋 Who I am

I'm a mathematician and IT consultant with 12+ years of work in QA, cloud/hybrid infrastructure, Business Intelligence, and web development.

I come from the math olympiad world: I won Nicaragua's national olympiad twice and earned honorable mentions at the Ibero-American and Central American olympiads. That's where I learned what still defines my work today: **understand the problem before touching the solution**.

That foundation took me into teaching (Jóvenes Talento Saturday Academy, training for Ministry of Education teachers, Data Analytics for public institutions), and later to a 10-year run directing **Fundación Uno's CODE project**, in alliance with **Harvard CS50x**: a program that trains **940+ students every year** in computer science, where I led functional QA for a team of **73 technical staff** under Harvard University standards.

Today I work as an independent consultant. I rescue production platforms, audit security and performance, design infrastructure, and build data systems for companies that depend on their technology working every day. More and more, that work means connecting a company's real operation to AI models, safely and measurably.

## 🛠️ What I do

| Area | In practice |
|:-----|:------------|
| **IT & AI Consulting** | Technology assessments, solution architecture, AI integration into real business operations |
| **Applied AI** | MCP servers to query production systems from Claude through read-only accounts, custom agents and skills, agentic workflows (chaining, routing, RAG) |
| **QA & Debugging** | Functional testing (UAT), code audits, deep debugging to rescue platforms in production |
| **Infrastructure & Cloud** | Linux/Windows servers, VPS (cPanel/WHM), hybrid on-premise environments, cloud VoIP (3CX + Dinstar), Fortinet, Mikrotik |
| **Data & BI** | Executive web dashboards, SSRS, Excel-to-live-system ETL, KPIs management actually uses |
| **Web & mobile development** | Full-stack applications (PHP, Laravel, Next.js/TypeScript, Node), installable PWAs, native Android apps in Kotlin, portals with custom authentication, WordPress expert |

## 🚀 Recent work

Systems designed and built end to end, most of them already in production.

### Operations for a supermarket chain

- **Electricity bill control** — about 110 PDF bills arrive every month, and every figure in them is an embedded image, not text. The reader recognizes the digits against a hand-calibrated bank of 812 glyphs, with no OCR; it checks each value against the document itself and against history, splits payment across credit cards, and produces the ERP import template. It exposes a read-only **MCP** server with OAuth to query consumption, costs, and payments from Claude. `PHP 8.5 · Python · SQL Server/MySQL · MCP`
- **Single gateway for the maintenance ecosystem** — joins fleet, energy, water, and refrigeration under single sign-on without touching each system's internals: links use signed requests and every piece of personal data is stored encrypted with XChaCha20-Poly1305 (libsodium). TOTP second factor, no Composer. `PHP 8.5 · MySQL · libsodium`
- **Fleet, refrigeration, and generator management** — mileage and fuel efficiency, cost per km, preventive maintenance and unit replacement, synced with the fuel and GPS APIs. Automatic deployment from `main` in under five minutes, with the database migrated before the code is copied. `PHP 8.5 · MySQL`
- **Refrigerated container inspection** — a yard app that walks the inspector through 11 checkpoints with conditional logic, works on spotty signal (IndexedDB queue), and emails the manager only the findings. It has no database: each inspection is a commit through the GitHub API, and git history is the audit trail. `Next.js 16 · TypeScript · Tailwind 4 · Vercel`
- **Operational knowledge portal** — processes, policies, indicators, meetings, tools, and forms as interlinked documents, ingested from Excel, with interactive SVG flowcharts, approval-based versioning with field-by-field diffs, and auto-generated job profiles. Written to migrate to .NET + SQL Server without rewriting the logic. `Laravel 13 · MySQL · Tailwind 4 · Alpine.js`
- **Maintenance work-order platform** (team project) — a PWA on top of Business Central covering the whole store-maintenance cycle: work orders, supplier quotes, contracts, checks, advances, purchase orders, and SLA dashboards, with role-based manuals built into the app. `Blazor · .NET · Business Central · Azure`
- **Change-request management system** — multi-project PWA with 4 roles and push notifications that arrive with the app closed. The Web Push cryptography (RFC 8291 + VAPID ES256) is implemented by hand with native PHP extensions: zero Composer, migrating the app means copying files. `PHP 8 · SQLite/MySQL`
- **Business-indicators dashboard** — processes ~5,900-row Excel backups from 58 stores and computes occupancy and rent KPIs. The history lives versioned in a GitHub repo: no database to maintain. `Next.js 14 · TypeScript · Tailwind · Recharts · Vercel`

### My own products

- **Dialens** — an Android app that identifies which carrier any Central American number belongs to, using each regulator's numbering ranges, without sending contacts or calls to any server. It shows the carrier over the call screen and blocks numbers by prefix before they ring. Dependencies verified with SHA-256 checksums. `Kotlin · Jetpack Compose · Android`
- **Cerebro** — an Obsidian vault that turns every Claude Code work session into a note with a title, project, topics, and links, redacting credentials before saving it. 1,600+ searchable notes, maps of content by project and topic, and an offline 3D graph viewer. It's the decision memory for all my projects. `Python · Obsidian · 3d-force-graph`

### Clients & consulting

- **Fundación Uno · Archive & Vault** — two private platforms with a single login across both: the institutional archive of the Foundation's legacy and a document repository that catalogs photos (SmugMug), videos (YouTube), and files (Google Drive). No WordPress, no Composer, with 2FA and CSP. `PHP · MySQL · OAuth`
- **New Connections International** — bilingual website for an Ireland-based international mobility agency, migrated from WordPress to custom PHP with its own admin panel, a 2026 brand redesign, SEO/AEO/GEO, and GDPR consent with Consent Mode v2. `PHP · MySQL · SCSS`
- **[nekupe.com](https://nekupe.com)** — website of Nekupe Sporting Resort (Nandaime, Nicaragua): shared PHP partials architecture, admin panel with drag-and-drop gallery, SEO/GA4, FTPS deployment. `PHP · AngularJS · MySQL · Bluehost`
- **La Divina Providencia Carpentry Workshop** — online catalog, orders, and management for a Franciscan craft workshop and its religious-goods shop, with an order state machine and role-based permissions. `Laravel 12 · Livewire 3 · MySQL`

## 🎤 Workshops & talks

- **"Designing and implementing agentic workflows"** — 1st Artificial Intelligence Congress at UNAH (Tegucigalpa, July 2026). Progressive notebooks on prompt chaining and routing, RAG with ChromaDB, and a custom MCP server, all on free endpoints so anyone can reproduce it. Material at [silfdv/flujos-agenticos](https://github.com/silfdv/flujos-agenticos).

## 🧭 How I work

- **Minimal dependencies.** Several of my production systems run without Composer, npm, or a framework. Fewer dependencies mean a smaller attack surface and a migration that comes down to copying files from one server to another. This GitHub profile consumes no external service either: the banner, icons, and badges are SVG files that live inside the repository.
- **Security from the first commit.** Strong password hashing, signed sessions, second factor, personal data encrypted at rest, sensitive files kept outside the webroot, and input sanitization against XSS. I define it in the project's initial architecture, before writing the business logic.
- **Documentation with every delivery.** Every system I hand over includes its README with the architecture, a migration guide, and a versioned changelog, so someone else can pick up the project without depending on me.
- **Project memory.** Every decision is recorded in Cerebro, so when I come back to a system months later I start from what was already decided and why, not from scratch.
- **AI applied with judgment.** I work with Claude Code, my own agents and skills across development, QA, and documentation, and every delivery goes through an adversarial review before I call it done. I review every line of code that carries my name.

## 🧰 Stack

<div align="center">

**Languages & Frontend**

<img src="assets/skills-1.svg" alt="TypeScript, JavaScript, PHP, Python, HTML, CSS, React, Next.js, Tailwind, AngularJS" />

**Backend, data & infrastructure**

<img src="assets/skills-2.svg" alt="Node.js, MySQL, SQLite, Git, GitHub, Linux, Vercel, WordPress, LaTeX, VS Code" />

**Mobile, frameworks & cloud**

<img src="assets/skills-3.svg" alt="Kotlin, Android Studio, Laravel, Alpine.js, .NET, Azure, Cloudflare, Obsidian, Postman, Windows" />

</div>

<br />

**Also** · SQL Server (SSRS) · Business Central · Jetpack Compose · Livewire · Advanced Excel (Power Query, VBA, macros) · PWA & Web Push · libsodium · cPanel/WHM · DNS · 3CX · Fortinet · Mikrotik · Model Context Protocol (MCP) · Claude Code, agents, and LLM workflows for development, QA, and data analysis

## 🏅 Honors

- 🥇 Winner, **Nicaraguan National Mathematical Olympiad** (2007 and 2009)
- 🌎 **Honorable Mention** — Ibero-American Mathematical Olympiad (Mexico 2009, Paraguay 2010)
- 🌎 **Honorable Mention** — Central American and Caribbean Mathematical Olympiad (Honduras 2008)
- 🏛️ Organizing committee, 15th Central American and Caribbean Mathematical Olympiad (2013)
- 🎓 Co-founder, technology commission of the **Nicaraguan Mathematical Olympiad**

## 📫 Let's talk

Got a platform to rescue, data that isn't telling you anything, or an operation you want to connect to AI? Write me.

**[contacto@silvioduarte.com](mailto:contacto@silvioduarte.com)** · **[silvioduarte.com](https://silvioduarte.com)** · **[linkedin.com/in/silvioduarte](https://linkedin.com/in/silvioduarte)**

<div align="center">

<img src="assets/footer.svg" width="100%" alt="" />

<sub>Silvio Duarte · Mathematician · IT & AI Consultant</sub>

</div>
