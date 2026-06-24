# நூல் / NOOL — steal-kit

> *The Reasoning Thread: a record of INTENT (why), ABSTRACTION (what type), and CHAIN (how).*

---

## நோக்கம் / Intent (Soul: WHY)

### The Problem
Knowledge workers lack a systematic, tool-supported method for processing external knowledge. They consume endlessly (articles, books, podcasts, talks) and store compulsively (bookmarks, highlights, databases), yet the conversion rate from consumption to capability remains near zero. There are tools for *storing* information (Notion, Obsidian, Readwise) but no toolkit for the cognitive act of *translating* information into personal, applicable intelligence.

### The Purpose
An open-source toolkit that operationalizes the STEAL methodology (Scan, Translate, Evaluate, Abstract, Leverage) with CLI commands, templates, workflows, and the companion book ("Let's STEAL: Copy Nothing, Learn Everything") shipped inside `/docs/book/`. steal-kit is the Body layer of the 3-layer franchise: **STEAL Gracefully** (brand/philosophy) → **Let's STEAL** (book/methodology) → **steal-kit** (OSS/tooling). It is the most accessible entry point into the SYNTHAI ecosystem, the "gateway drug" that requires zero prior knowledge.

### What We're Avoiding
- Over-engineering the CLI before the methodology is proven (book first, tooling second)
- Building another note-taking app (steal-kit is a *learning* tool, not a *storage* tool)
- Locking content behind paywalls (all digital formats are free, print is paid)
- SYNTHAI jargon in the public interface (MBS lives under the hood)
- Duplicating Kleon's "Steal Like an Artist" aesthetic without the methodological depth

---

## வடிவம் / Abstraction (Mind: WHAT TYPE)

### Problem Type
**DESIGN**: Architecting an OSS learning toolkit that bundles methodology (MANIFESTO), content (book in 3 formats), templates (exercises), and CLI tooling into a single repository.

### Key Dimensions
1. **The STEAL Protocol**: 5-step cognitive methodology (Scan → Translate → Evaluate → Abstract → Leverage), the core intellectual asset
2. **The Book**: 35 pages, 5 stages × 5 page types (Principle, Scene, Anti-Pattern, Practice, Example), ships as HTML/PDF/EPUB inside `/docs/book/`
3. **The Grace Principles**: Attribution, Transformation, Sovereignty, the ethical framework for learning from others
4. **The Intention Arc** (hidden spine): Curiosity → Ownership → Courage → Insight → Agency, woven through Intention Prompts
5. **Multi-Format Pipeline**: Single-source markdown builds to responsive HTML, 210mm square PDF (Paged.js), and reflowable EPUB (Pandoc)
6. **Gateway Economics**: Free digital maximizes reach, paid print ($12.99) funds operations, upsell to Let's SPAR and SYNTHAI consulting

### Key Relations
- Book **ENABLES** adoption (methodology must be readable before it's toolable)
- MANIFESTO **REQUIRES** book (the manifesto promises, the book delivers)
- CLI **AMPLIFIES** book (automates the exercises: `steal scan`, `steal translate`, etc.)
- Multi-format pipeline **ENABLES** gateway economics (free HTML = discoverability)
- Grace Principles **CONSTRAIN** all CLI output (attribution is built into the template system)
- steal-kit **ENABLES** spar-kit adoption (you STEAL the knowledge, then you SPAR the decision)
- Intention Arc **DAMPENS** surface-level use (the hidden spine guides depth without forcing it)

---

## சங்கிலி / Chain (Body: HOW)

### Execution Path

| Phase | Activity | Status |
|-------|----------|--------|
| 1. MANIFESTO | Write the steal-kit manifesto | ✅ Done (SPAR #44) |
| 2. NOOL | Create kit NOOL (this file) | ✅ Done |
| 3. Book NOOL | Create/update book NOOL | ✅ Done (v0.4) |
| 4. Page Types Defined | 5 page types with full specimens | ✅ Done (SPAR #43) |
| 5. Format Strategy | Sizing, multi-device, distribution | ✅ Done (SPAR #44) |
| 6. Kit Config | `kit-config.yaml` with 5 page type constraints | ⬜ |
| 7. Writer's Bible | Voice, style, constraints per page type | ⬜ |
| 8. Stage Drafts | 5 stages × 5 pages = 25 core pages (markdown) | ⬜ |
| 9. Intro/Outro | 5 framing pages | ⬜ |
| 10. Build Pipeline | Markdown → HTML + PDF + EPUB CI/CD | ⬜ |
| 11. CLI Scaffold | `steal scan`, `steal translate`, etc. | ⬜ |
| 12. Templates | Exercise templates, steal journal templates | ⬜ |
| 13. README | Public-facing repo README | ⬜ |
| 14. Audit | Full page audit per kit-book pipeline | ⬜ |
| 15. Launch | GitHub release, social campaign | ⬜ |

### Repo Structure (target)

```
steal-kit/
├── methodology/
│   ├── MANIFESTO.md
│   ├── PROTOCOL.md
│   ├── GRACE_PRINCIPLES.md
│   ├── INTENTION_ARC.md
│   └── STEAL_IN_5_MINUTES.md
├── docs/
│   └── book/
│       ├── src/            # Markdown source (per-page .md)
│       ├── html/           # Built responsive HTML
│       ├── pdf/            # Built 210mm×210mm PDF
│       └── epub/           # Built reflowable EPUB
├── templates/
│   ├── steal-journal.md
│   ├── one-sentence-translation.md
│   ├── evaluation-rubric.md
│   ├── abstraction-ladder.md
│   └── leverage-checklist.md
├── cli/                    # CLI tooling (future)
├── NOOL.md
├── MANIFESTO.md → methodology/MANIFESTO.md
├── LICENSE                 # MIT (code), CC BY-NC-SA 4.0 (content)
└── README.md
```

### Success Criteria
- [ ] MANIFESTO.md defines the philosophy clearly enough that a stranger understands STEAL in 5 minutes
- [ ] Book ships in 3 formats (HTML, PDF, EPUB) from single-source markdown
- [ ] PDF renders at 210mm × 210mm, matching the SPAR book series
- [ ] HTML is responsive and readable on mobile (320px+)
- [ ] Exercise templates are usable standalone without reading the full book
- [ ] CLI scaffold exists with at least `steal --help` and `steal scan` commands
- [ ] README makes the repo star-worthy on first glance
- [ ] 100+ GitHub stars within 90 days of launch (validation metric)

### Revision Triggers
<!-- When a Revision Trigger fires, write a LOON entry (templates/LOON-template.md) before updating this NOOL. -->
- STEAL protocol changes (step added, removed, or renamed)
- Book structure changes (page count, page types, or stage ordering)
- Distribution model changes (free → paid or vice versa)
- Build pipeline technology changes (Paged.js → alternative)
- CLI architecture decisions (language choice, framework)
- First community contribution received (validates the OSS model)

---

## Evolution History

| Version | Date | Layer Changed | What Changed | Source |
|---------|------|---------------|--------------|--------|
| v0.1 | 2026-02-27 | All | Initial NOOL. MANIFESTO written, 3-layer franchise defined, format/distribution locked. | SPAR #43, #44, MANIFESTO.md |

---

> *நூல் (nool): the thread that connects, the text that records, the classic that endures.*
>
> **Triad**: NOOL (thread, forward) ↔ LOON (mirror, backward) + LOOM (weave, across). See `templates/LOON-template.md` and `templates/LOOM-template.md`.
