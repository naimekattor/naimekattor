<div align="center">

# Hi, I'm Naim Hossen 👋

### Full-Stack Developer · AI/LLM Integration · Systems-Level Engineering

I build products end-to-end — from pixel-perfect React interfaces down to real-time audio pipelines and AI-powered backends.

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://naim-portfolio-delta.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/naimekattor/)
[![Twitter](https://img.shields.io/badge/Twitter-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Naimekattor)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:naimekattor@gmail.com)

</div>

---

## About Me

- 🎓 Mathematics student, based in Dhaka — self-taught into full-stack and systems development
- 💼 Building production-grade full-stack and AI-integrated systems — see case study below
- ⚙️ Comfortable across the stack: React/Next.js frontends, Node/Next API routes and Postgres/Supabase backends, and Rust for systems-level performance work
- 🤖 Shipped projects using RAG (vector search), multi-provider LLM integration (Ollama/OpenAI/Anthropic), and real-time speech-to-text pipelines
- 🎨 Strong interest in high-craft UI/UX — I care as much about interaction detail as functionality
- ✈️ Long-term goal: travel and work from around the world

---

## Tech Stack

**Frontend**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Backend & Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)

**AI / Systems**
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=for-the-badge&logo=tauri&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logo=qdrant&logoColor=white)

**Tools**
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

---

## 🎯 Case Study: AI Desktop Assistant & Real-Time Meeting Transcriber

A cross-platform desktop app (Tauri v2 + Rust + React 19) that captures **microphone and system speaker audio simultaneously** and transcribes both in real time — either fully offline or via a cloud API, switchable at runtime.

**The hard problem:** naive time-based audio chunking cuts sentences mid-phrase, which wrecks transcription accuracy. I implemented natural-pause endpointing — detecting 500–700ms silence gaps to close an utterance — with a 500ms pre-roll buffer so word boundaries never get clipped.

**What it does:**
- Dual STT engines: offline `whisper.cpp` (zero cost, zero internet, ~150ms–300ms on CPU) or Groq's `whisper-large-v3-turbo` cloud API (<200ms latency)
- Custom Automatic Gain Control — amplifies quiet speech up to 20× without clipping, using peak-normalization math I derived myself
- WASAPI loopback capture on Windows to grab system audio (Teams/Zoom/Meet/YouTube) alongside the mic, mixed via a Rust DSP pipeline
- Single-instance mutex locking to keep memory under ~150MB even with two parallel audio streams — an early version without this leaked RAM per spawned process

**Stack:** Rust, Tauri v2, React 19, TypeScript, `cpal`, `whisper.cpp`, Groq API

[→ View repo](https://github.com/naimekattor/sytem-level-mic-and-speaker-tracker-desktop-app)

---

## 🌟 Projects

| Project | What it does | Stack | Live |
|---|---|---|---|
| [AI Desktop Assistant / Transcriber](https://github.com/naimekattor/sytem-level-mic-and-speaker-tracker-desktop-app) | Real-time dual-stream (mic + speaker) transcription, offline or cloud STT — see case study above | Rust, Tauri, React, whisper.cpp | Desktop app |
| [EduGuide](https://github.com/naimekattor/university-admission-assistant) | AI advisor for Bangladeshi students — chat-based guidance, eligibility checking, and semantic search over university data via a vector DB | Next.js, Qdrant, Drizzle, multi-LLM (Ollama/OpenAI/Anthropic) | _add demo link_ |
| [AI Client Generator (Dashboard)](https://github.com/naimekattor/ai_client_generator_frontend) | Internal agency portal for lead import, pipeline tracking, automated site audits, and AI-drafted outreach emails | Next.js 16, TanStack Query, Zustand, Zod | _add demo link_ |
| [Blog Platform](https://github.com/naimekattor/assunnah_blog) | Role-based blog (user/moderator/admin) with a full approval workflow and database-level Row Level Security | Next.js 15, Supabase, PostgreSQL RLS | [hokpath.com](https://www.hokpath.com/) |

---

## GitHub Stats

<div align="center">

![Naim's GitHub stats](https://github-readme-stats.vercel.app/api?username=naimekattor&show_icons=true&theme=dark&hide_border=false&include_all_commits=false&count_private=false&cache_seconds=86400)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=naimekattor&theme=dark&hide_border=false&cache_seconds=86400)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=naimekattor&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact&cache_seconds=86400)

</div>

---

<div align="center">

*Crafting the web with intention — one interface at a time.*

[![Profile Views](https://visitcount.itsvg.in/api?id=naimekattor&icon=0&color=0)](https://visitcount.itsvg.in)

</div>