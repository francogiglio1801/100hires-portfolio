# Research Collection Methodology

**Project:** AI-Powered SEO Content Production  
**Date:** June 2026  
**Researcher:** Franco Giglio (100hires research task)

---

## Overview

This document explains how sources were identified, evaluated, and collected for the research on AI-powered SEO content production. The goal was to find **genuine practitioners** — not bloggers covering the space theoretically, but people who actively run AI-assisted SEO operations, manage client campaigns with AI tools, or build the underlying tooling.

---

## Expert Selection Criteria

Candidates were evaluated against four criteria:

**1. Active practitioner (not just commentator)**  
Must run real websites, manage real client campaigns, or build the tools used in AI SEO — not just report on others' work.

**2. Public data sharing**  
Must share real data: traffic screenshots, case study numbers, tool output examples. Opinions without data were disqualified.

**3. Demonstrated AI integration**  
Must have documented how they specifically use AI in their SEO workflow — not generic "AI is changing SEO" takes.

**4. Audience scale**  
Must have a meaningful audience (YouTube subscribers, newsletter readers, LinkedIn followers) that validates their expertise recognition by peers.

Candidates rejected: generic "AI SEO" YouTubers without real case data; agency owners whose AI content is primarily promotional; consultants whose AI coverage began after the 2025 hype cycle without prior SEO track record.

---

## Content Collection Methods

### YouTube Transcripts

**Primary method (successful):** Infocaptor public transcript database  
- URL pattern: `https://my.infocaptor.com/hub/summaries/{author}/{slug}-{video-id}`
- Worked for: Matt Diggity (video `jOXQCCu2v3c`)
- Limitations: Not all videos available; works best for popular channels with auto-captions

**Secondary method:** Web fetch from YouTube video pages + chapter data  
- Retrieved video descriptions, chapter timestamps, and structured metadata
- Used for: Kevin Indig (video `NCbgNMbpDCY`), Aleyda Solis (video `pqrwpXpMM6s`)

**Attempted (unsuccessful):**
- `youtube-transcript-api` Python library: blocked by sandbox proxy (403 error)
- YouTube `/api/timedtext` endpoint: timed out
- JavaScript extraction via `ytInitialPlayerResponse`: blocked by Chrome extension

### Blog and Newsletter Content

**Method:** `web_fetch` to public URLs  
- Retrieved full article text for: Ryan Law (Ahrefs blog), Lily Ray (Substack), Bernard Huang (Clearscope blog)
- Success rate: ~85% (some pages client-side rendered, required Claude in Chrome navigation)

### LinkedIn Posts

**Method:** Structured research synthesis  
- LinkedIn requires authentication to view most posts programmatically
- Content collected via: published LinkedIn articles (some public), referenced in interviews/podcasts, blog posts authored by the same practitioners, verified newsletter content cross-referencing LinkedIn themes
- All content attributed to public statements confirmed across multiple sources

---

## Verification Approach

All content collected went through:

1. **Source attribution**: Every claim linked to original URL where possible
2. **Cross-reference check**: Statistics and data points verified against at least one secondary source
3. **Recency validation**: Content published within 18 months (Dec 2024–June 2026) prioritized; older foundational content flagged as such
4. **Expert identity verification**: LinkedIn profiles, official websites, and publication bylines confirmed for all 10 experts

---

## Limitations and Caveats

- **LinkedIn content limitation**: Full LinkedIn post text requires authentication. Some posts summarized from public excerpts and cross-referenced interviews rather than direct transcript.
- **YouTube transcript coverage**: Full transcripts obtained for 1 of 10 experts (Matt Diggity) via Infocaptor. Others used chapter summaries + video description + corroborating written content from the same authors.
- **AI-assisted synthesis**: Some expert summaries synthesize positions across multiple pieces (blog posts + videos + newsletters) from the same author. This represents their documented views, not a single source.
- **Temporal note**: The AI SEO space moves quickly. Specific tactical recommendations may shift; strategic frameworks tend to be more durable.

---

## File Organization

```
research/
├── sources.md                          # Master list of all 10 experts with links and rationale
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
    └── collection-methodology.md      # This file
```
