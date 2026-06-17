# 100hires-portfolio

Portfolio project for the 100hires junior growth marketing specialist selection process — Franco Giglio

---

## Tools Installed

### Cursor IDE
AI-powered code editor built on VS Code, available at [cursor.com](https://www.cursor.com/). It combines a familiar coding environment with built-in AI assistance, making it easy to write, debug, and navigate code using natural language.

### Claude Code (Anthropic)
Official Anthropic extension for VS Code / Cursor. Integrates the Claude AI assistant directly into the editor, enabling natural language queries about the codebase, code generation, and debugging — without leaving the IDE.

### Codex (OpenAI)
OpenAI's extension for VS Code / Cursor. Provides AI-powered code suggestions and autocomplete, helping write code faster based on context and intent.

---

## Steps Completed

1. **Installed Cursor IDE** — Downloaded the installer from cursor.com and installed it on Windows.
2. **Installed "Claude Code" extension** — Opened the Extensions panel in Cursor (Ctrl+Shift+X), searched for "Claude Code", and installed the Anthropic extension. Logged in with my Anthropic account.
3. **Installed "Codex" extension** — Searched for "Codex" in the same Extensions panel and installed the OpenAI extension. Logged in with my OpenAI account.
4. **Created the `100hires-portfolio` folder** — Created the project folder locally and opened it in Cursor via File > Open Folder.
5. **Created this `README.md` file** — Documented the tools, steps, and issues encountered throughout the process.
6. **Published to GitHub** — Created the public repository `100hires-portfolio` under the account `francogiglio1801` and pushed the file.

---

## Issues Encountered & How I Solved Them

### 1. Cursor's Extension Marketplace doesn't always show VS Code extensions
- **Issue:** Cursor uses its own extension registry (Open VSX) by default, which doesn't include all extensions available on the official VS Code Marketplace. Some extensions like Claude Code weren't showing up in the default search.
- **Solution:** Enabled VS Code Marketplace access in Cursor settings (Cursor Settings > Extensions > Enable VS Code Extension Marketplace), which made both extensions available and installable.

### 2. Git identity not configured for the first commit
- **Issue:** When initializing the local repo, Git refused to commit because no user name or email was set.
- **Solution:** Ran `git config --global user.name "Franco Giglio"` and `git config --global user.email "francogiglio1801@gmail.com"` to configure the global identity before committing.

### 3. GitHub authentication via HTTPS no longer accepts passwords
- **Issue:** Running `git push` prompted for credentials, but GitHub rejected the account password — standard password authentication was deprecated.
- **Solution:** Generated a Personal Access Token (PAT) from GitHub Settings > Developer settings > Personal access tokens, and used that token as the password when prompted during push.

---

## Repository

- **GitHub:** [https://github.com/francogiglio1801/100hires-portfolio](https://github.com/francogiglio1801/100hires-portfolio)
- **Author:** Franco Giglio ([@francogiglio1801](https://github.com/francogiglio1801))
- **Date:** June 2026


---

## Research Project: AI-Powered SEO Content Production

**Objective:** Map the current practitioner landscape for AI-assisted SEO content production — identifying who is actually building these workflows, what they've learned, and what patterns emerge across expert approaches.

**Scope:** 10 expert practitioners curated by demonstrated experience (not just commentary), with sources collected across YouTube transcripts, blog posts, newsletters, and LinkedIn content.

### Research Structure

```
research/
├── sources.md                          # Annotated master list of all 10 experts
├── youtube-transcripts/
│   ├── matt-diggity--seo-strategy-2025.md
│   └── kevin-indig--ai-overviews-seo-impact.md
├── linkedin-posts/
│   ├── lily-ray.md
│   ├── ryan-law.md
│   ├── bernard-huang.md
│   ├── aleyda-solis.md
│   ├── julian-goldie.md
│   ├── kevin-indig.md
│   ├── kyle-byers.md
│   ├── tim-soulo.md
│   └── ross-hudgens.md
└── other/
    └── collection-methodology.md
```

### The 10 Experts

| Expert | Role | Key Contribution |
|--------|------|-----------------|
| Matt Diggity | CEO, Diggity Marketing | Real-money site testing; brand + topical authority at scale |
| Lily Ray | VP SEO, Amsive | GEO vs SEO tension; 5 tactics that backfire |
| Ryan Law | Director of Content, Ahrefs | 14 AI SEO use cases; quality-over-volume framework |
| Bernard Huang | Co-founder, Clearscope | Topical authority + information gain as AI era foundation |
| Kevin Indig | Growth Advisor | AIO CTR impact data; cosine similarity optimization |
| Aleyda Solis | Founder, Orainti | AI search crawlability; LearningAIsearch.com curriculum |
| Julian Goldie | CEO, Goldie Agency | End-to-end AI pipelines (Gemini → Claude → HeyGen) |
| Kyle Byers | Director Growth, Semrush | Enterprise AI content; hallucination risk management |
| Tim Soulo | CMO, Ahrefs | Original data as moat; depth-over-volume framework |
| Ross Hudgens | Founder, Siege Media | Agency AI ops; E-E-A-T in practice |

### Key Themes Across Experts

1. **AI accelerates production but doesn't replace expertise** — Every practitioner uses AI for speed; none have replaced human judgment on quality.
2. **GEO and SEO are converging** — ChatGPT/Perplexity draw from Google's index (85–90% correlated per Lily Ray). SEO foundation is prerequisite for AI search visibility.
3. **Original data is the durable moat** — Content AI cannot produce (proprietary data, real case studies, named expertise) is increasingly the differentiating factor.
4. **E-E-A-T is now business strategy** — Not a Google checkbox; the actual criterion for AI system source selection.
5. **Measurement must evolve** — Traditional rank tracking insufficient; need AI search visibility metrics alongside CTR and brand signals.
