<p align="center">
  <img src="assets/banner.png" alt="Charalampos Panagopoulos — Full-Stack Development, AI, Homelab" width="100%" />
</p>
<br/>

# 👋 Hi, I'm Charalampos Panagopoulos

Full-stack developer based in Athens, Greece, with a background in customer service and a passion for building real, deployed software. I work across React and Node.js, integrate AI into practical tools, and run my own self-hosted homelab for development and automation.

My approach is simple: I build things that solve real problems — from a production AI chatbot to automations that remove hours of manual work from my week.

---

## Featured Projects

### [Hermes — AI Customer-Service Chatbot](https://github.com/c-panagopoulos/hermes-ai) &nbsp;·&nbsp; [Live Demo](https://hermes.cpanagopoulos.dev)

A production-ready, full-stack AI chatbot with a custom Retrieval-Augmented Generation (RAG) pipeline.

- **Custom RAG pipeline** — documents are chunked, embedded, and stored in PostgreSQL with `pgvector`, then retrieved by cosine similarity to ground every response
- **Real-time token streaming** over Server-Sent Events, rendered word-by-word on a React frontend
- **JWT-protected admin dashboard** with live analytics (containment/escalation rates, handle time) and drag-and-drop document ingestion
- **Automatic human-handoff escalation** via an n8n webhook with full conversation history
- **Deployed to production** on Vercel with a cloud backend, rate limiting, and an OpenAI-compatible LLM layer (Groq in production, local Ollama in development)

`React 19` · `Vite` · `Tailwind` · `Node.js / Express` · `PostgreSQL + pgvector` · `Groq / Ollama` · `n8n` · `Vercel`

### [tapstudy — NFC-Triggered Study Tracker](https://github.com/c-panagopoulos/tapstudy) &nbsp;·&nbsp; [Live Demo](https://tapstudy.cpanagopoulos.dev)

A self-hosted study tracker triggered by tapping an NFC tag on a desk — no app to open, no timer to remember to start.

- **Fact-first AI insights** — a local LLM (Ollama) never computes a number itself; every percentage, delta, and projection is precomputed in code and handed to the model purely to phrase into a sentence, avoiding the arithmetic errors small models make when asked to reason over raw stats
- **NFC-triggered UX** — tapping a programmed tag hits a single `/scan` endpoint that starts or stops a session, with an animated confirmation screen and zero app-switching
- **Single-container self-hosted deployment** — Postgres, Express, and nginx run together in one Docker image behind a bash entrypoint, deployed to both a homelab server and a public read-only demo on a Hetzner VPS behind a Cloudflare Tunnel
- **Hardened for public exposure** — per-IP rate limiting, a read-only mode that blocks every mutating route at the backend (not just hidden in the UI), and a global error handler that never leaks stack traces
- **Accessible guided onboarding tour** — dynamically positioned coach marks with full keyboard/screen-reader support (ARIA dialog semantics, managed focus, Escape-to-close)

`React 19` · `Vite` · `Tailwind CSS` · `Recharts` · `Express` · `PostgreSQL` · `Ollama` · `Docker` · `Cloudflare Tunnel`

### [AI-Powered Learning Notes Automation](https://github.com/c-panagopoulos/n8n-automations)

An n8n workflow that turns handwritten notes into formatted, searchable Nextcloud Deck cards using OpenAI Vision.

- Saves ~3 hours per week
- Custom Markdown template, runs self-hosted in Docker
- Demonstrates real-world workflow engineering

### [Personal Portfolio Website](https://c-panagopoulos.github.io/Personal-Website/)

My evolving web development showcase, built from scratch with HTML, CSS, and JavaScript.

---

## Tech Stack

**Frontend:** React · JavaScript (ES6+) · Vite · Tailwind CSS · shadcn/ui · HTML5 · CSS3 · Bootstrap

**Backend:** Node.js · Express · REST APIs · Server-Sent Events · JWT Auth · PostgreSQL · pgvector

**AI & Automation:** RAG · OpenAI Embeddings · LLM Integration (Groq, Ollama) · Prompt Engineering · n8n

**Infrastructure & Tooling:** Docker · Linux · Tailscale · Git & GitHub · Nextcloud · Vaultwarden · WebDAV · Vercel

---

## Self-Hosted Homelab

My personal infrastructure for development, automation, and learning — and proof that my DevOps interest is hands-on, not theoretical:

- Dockerized services (Jellyfin, Nextcloud, Vaultwarden, and more)
- Secure remote access over Tailscale
- Self-hosted n8n powering my automation projects

---

## What Drives Me

Technology helps me solve my own problems. When I needed structure while studying, I built automations. When I wanted more control over my tools, I built and managed my homelab. When manual work piled up, I designed workflows to remove it. That same mindset is what I bring to building software for other people.

---

## 🌐 Connect

- **Portfolio:** https://c-panagopoulos.github.io/Personal-Website/
- GitHub: **https://github.com/c-panagopoulos**  
- LinkedIn: **https://linkedin.com/in/c-panagopoulos**  
- Email: **char@panago.anonaddy.com**

---

Thanks for stopping by, more projects on the way as I continue my full-stack journey!
