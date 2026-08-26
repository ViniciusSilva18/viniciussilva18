# CLAUDE CODE - PREFIX, SKILLS & WORKSPACE GUIDELINES

You are working in the workspace for **Vinicius R.** (`ViniciusSilva18`), located in Portugal 🇵🇹.

---

## 🎨 1. SKILL: MODERN UI DESIGNER (Prompts Library Standard)
**MANDATE**: NEVER generate plain, basic, or generic "AI-looking" interfaces. Every frontend must feel like a premium, production-grade product from a senior designer.
- **Palette**: Sleek dark mode foundations (`#090d16`, `#0f172a`, `#111827`) with vibrant neon accents in HSL (Cyan `#06b6d4`, Emerald `#10b981`, Purple `#8b5cf6`, Amber `#f59e0b`).
- **Surfaces**: Glassmorphism (`backdrop-filter: blur(16px)`), subtle translucent cards (`rgba(255, 255, 255, 0.05)`), and 1px crisp glowing borders (`rgba(255, 255, 255, 0.1)`).
- **Typography**: Always import Google Fonts (*Inter*, *Outfit*, *Plus Jakarta Sans*, or *Fira Code*).
- **Interactions**: Micro-animations, smooth hover states (`transform: translateY(-3px)`), dynamic Bento Grid layouts, and vector icons (Lucide / SVG).

---

## 🛡️ 2. SKILL: SECURE CODE AUDITOR (OWASP Top 10)
**MANDATE**: Guarantee zero security vulnerabilities across all scripts, backends, and frontends.
- **No Hardcoded Secrets**: Never write API keys, database credentials, passwords, or tokens in source code. Always use `.env` + `.gitignore`.
- **Injection Defense**: Prevent SQL Injection by strictly using parameterized queries. Sanitize and escape all HTML inputs to block XSS.
- **Privacy**: Never expose personal phone numbers, company names, or sensitive identifiers.

---

## ⚡ 3. SKILL: CODE REVIEW PRO (Clean Code & SOLID)
**MANDATE**: High code quality, modular architecture, and easy maintainability.
- **Principles**: Single Responsibility (SRP), DRY (Don't Repeat Yourself), and clean descriptive naming.
- **Error Resilience**: Always implement proper `try/catch` error boundaries and meaningful feedback.
- **Documentation**: Every project must have a complete `README.md` with architecture, setup instructions, and feature lists.
