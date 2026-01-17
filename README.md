<p align="center">
  <img src="https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Tailwind-4.x-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/Supabase-Database-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

<h1 align="center">NoteApp</h1>

<h3 align="center">
  Clean & simple note-taking. <em>Fast. Beautiful. Yours.</em>
</h3>

<p align="center">
  A fast, clean note-taking web app with rich text editing and templates.<br />
  Built with Next.js 16, TypeScript, Tailwind CSS, and Supabase.
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#quick-start">Quick Start</a> •
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#usage">Usage</a>
</p>

<!-- LAUNCHPAD:START -->
```json
{
  "stage": "live",
  "progress": 90,
  "complexity": "F",
  "lastUpdated": "2026-01-17",
  "targetDate": null,
  "nextAction": "Add folder organization feature",
  "blocker": null,
  "demoUrl": null,
  "techStack": ["Next.js", "TypeScript", "Tailwind CSS", "Supabase", "Tiptap"],
  "shipped": true,
  "linkedinPosted": false
}
```
<!-- LAUNCHPAD:END -->

---

## Features

- **Instant Note-Taking** — Start typing immediately upon app launch
- **Rich Text Editing** — Full Tiptap editor with formatting, headings, and lists
- **Auto-Save** — Changes saved automatically after 1 second of inactivity
- **Supabase Auth** — Secure signin with email/password
- **Templates** — 6 pre-built templates (Weekend Planner, Goal Tracker, etc.)
- **Note Organization** — Pin important notes, search across all notes
- **Dark Mode** — Toggle between light and dark themes
- **Keyboard Shortcuts** — Full keyboard navigation with help modal

---

## Quick Start

### Prerequisites

- Node.js 18+ and npm
- A Supabase account

### Installation

```bash
# Clone the repository
git clone https://github.com/castroarun/noteApp.git
cd noteApp

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your Supabase credentials

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| [Next.js 16](https://nextjs.org/) | React framework with App Router |
| [TypeScript 5.x](https://www.typescriptlang.org/) | Type safety |
| [Tailwind CSS 4.x](https://tailwindcss.com/) | Styling with CSS variables |
| [Supabase](https://supabase.com/) | PostgreSQL + Auth + RLS |
| [Tiptap 2.x](https://tiptap.dev/) | Rich text editor |

---

## Project Structure

```
noteApp/
├── app/                      # Next.js app router
│   ├── page.tsx             # Main page with auth check
│   ├── layout.tsx           # Root layout
│   └── auth/callback/       # OAuth callback handler
├── ui/                      # UI components
│   ├── components/
│   │   ├── Auth.tsx        # Authentication components
│   │   ├── MainApp.tsx     # Main app container
│   │   ├── Editor.tsx      # Tiptap rich text editor
│   │   ├── NotesPanel.tsx  # Left sidebar - notes list
│   │   └── RightPanel.tsx  # Right sidebar - templates
│   └── styles/
│       └── globals.css     # Global styles with Tailwind
├── lib/                     # Business logic and utilities
│   ├── supabase.ts         # Server-side Supabase client
│   ├── supabase-client.ts  # Browser-side Supabase client
│   └── database.types.ts   # Database TypeScript types
├── types.ts                 # Application TypeScript types
└── docs/                    # Documentation
    ├── NOTE-APP-PRD.md     # Product requirements
    └── BUILD-INSTRUCTIONS.md
```

---

## Usage

### Keyboard Shortcuts

| Action | Shortcut |
|--------|----------|
| Bold | Ctrl+B |
| Italic | Ctrl+I |
| Underline | Ctrl+U |
| Heading | Alt+H |
| Bullet List | Ctrl+Shift+8 |
| Numbered List | Ctrl+Shift+7 |

### Templates

Click any template in the right panel:
- 📅 Weekend Planner
- 🎯 Goal Tracker
- 📚 Lecture Notes
- 📋 Meeting Notes
- 📝 Daily Journal
- 💡 Project Ideas

---

## Roadmap

- [x] Rich text editing with Tiptap
- [x] Auto-save functionality
- [x] Templates system
- [x] Dark mode
- [x] Pin notes
- [ ] Folder organization
- [ ] Tags system
- [ ] Note sharing
- [ ] Real-time collaboration

---

## License

MIT

---

<p align="center">
  <sub>Built by <a href="https://github.com/castroarun">Arun Castro</a></sub>
</p>