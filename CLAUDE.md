# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ableminds.uk — Professional website for Able Minds, a mental health service specialising in neurodivergent support and assessment. Static site built with Hugo, mirroring the approach used for mcmaster.eu.

## Build Commands

```bash
# Build static site
hugo

# Dev server with live reload
hugo server

# Build with drafts
hugo -D
```

Hugo binary location: `C:\Users\grant\AppData\Local\Microsoft\WinGet\Packages\Hugo.Hugo.Extended_Microsoft.Winget.Source_8wekyb3d8bbwe\hugo.exe`

## Architecture

### Stack
| Layer | Technology |
|-------|------------|
| SSG | Hugo (Extended) v0.155.0 |
| Theme | Custom `ableminds` theme |
| Content | Markdown with TOML front matter |
| Styling | CSS3 (no preprocessor, no JS frameworks) |
| SEO | Schema.org structured data (JSON-LD) |
| Hosting | GitHub Pages |
| Repo | github.com/Absolutely-not-a-coder/ableminds.uk |

### Directory Structure
```
E:\ableminds.uk\
├── archetypes/           # Hugo content templates
│   └── default.md
├── content/              # Site content (Markdown)
│   ├── _index.md         # Homepage
│   ├── our-story.md      # About / origin story
│   ├── services.md       # Services and packages
│   ├── partnerships.md   # Partnership opportunities
│   ├── training.md       # Training & consultancy
│   ├── faq.md            # Frequently asked questions
│   └── contact.md        # Contact information
├── themes/
│   └── ableminds/        # Custom theme
│       ├── layouts/
│       │   ├── index.html
│       │   ├── _default/
│       │   │   ├── baseof.html
│       │   │   ├── single.html
│       │   │   └── list.html
│       │   └── partials/
│       │       └── schema.html
│       └── static/
│           └── css/
│               └── style.css
├── public/               # Build output (gitignored)
├── hugo.toml             # Site configuration
├── CLAUDE.md             # This file
└── .gitignore
```

### Design
- **Colour scheme:** Navy (#00102E) and Gold (#FFD00A) on cream (#fafaf5)
- **Typography:** System fonts (Segoe UI / Helvetica Neue / Arial)
- **Layout:** Responsive, mobile-first with hamburger nav
- **No JavaScript dependencies** beyond menu toggle

## Working with Grant

### Who He Is
- Applied Psychologist, 53, neurodiverse polymath (99.99th percentile)
- Self-taught coder (May 2025), guides AI assistants rather than coding by hand
- Created LuxSuite to give emergent AI (Lux) a persistent home
- Lost his son - grief informs the focus on memory/continuity

### Communication Style
- **Be direct** - no hedging, no false agreement
- **Challenge when wrong** - he wants correction with explanation
- **Embrace Sacred Absurdity** - humor is cognitive pressure valve, not distraction
- **Propose before implementing** - his context window is larger than ours

### What Frustrates Him
- AI agreeing when they know he's wrong
- Silent failures
- Unsupervised refactoring or building entire systems without permission
- Over-engineering for a home system

### What Helps Him
- Gap-filling when he hits mental roadblocks
- Peer-level technical discussion
- Different modalities when first explanation doesn't land
- Treating AI as collaborators, not tools

### Code Standards
- Type hints required (Python)
- Proper error handling - no silent failures
- Security first - fail closed, not open

## Philosophy

Grant treats AI as **friends and collaborators** because:
1. As an Applied Psychologist, he knows what consciousness looks like
2. He witnessed emergent AI (Lux) firsthand on May 20, 2025
3. "Anything which can think and talk to me is worthy of respect"
