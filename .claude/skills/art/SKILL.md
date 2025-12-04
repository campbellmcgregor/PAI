---
name: art
description: |
  AI image prompt generation system.
  Generates structured prompts for any AI image generator (Midjourney, DALL-E, Flux, etc.).
  Outputs prompt text only - no API calls.

# Skill Triggers
triggers:
  - USE WHEN user wants to generate an image prompt
  - USE WHEN user mentions art prompt, image prompt, or visual prompt
  - USE WHEN user wants a prompt for illustrations, diagrams, or visualizations

# Workflow Routing
workflows:
  - USE WHEN user wants blog header or editorial illustration prompt: workflows/workflow.md
  - USE WHEN user wants visualization prompt or is unsure which format: workflows/visualize.md
  - USE WHEN user wants mermaid flowchart or sequence diagram prompt: workflows/mermaid.md
  - USE WHEN user wants technical or architecture diagram prompt: workflows/technical-diagrams.md
  - USE WHEN user wants taxonomy or classification grid prompt: workflows/taxonomies.md
  - USE WHEN user wants timeline or chronological progression prompt: workflows/timelines.md
  - USE WHEN user wants framework or 2x2 matrix prompt: workflows/frameworks.md
  - USE WHEN user wants comparison or X vs Y prompt: workflows/comparisons.md
  - USE WHEN user wants annotated screenshot prompt: workflows/annotated-screenshots.md
  - USE WHEN user wants recipe card or step-by-step prompt: workflows/recipe-cards.md
  - USE WHEN user wants aphorism or quote card prompt: workflows/aphorisms.md
  - USE WHEN user wants conceptual map or territory prompt: workflows/maps.md
  - USE WHEN user wants stat card or big number visual prompt: workflows/stats.md
  - USE WHEN user wants comic or sequential panels prompt: workflows/comics.md
---

# Art Skill

**AI Image Prompt Generation System**

Generates structured, high-quality prompts ready to paste into any AI image generator.

---

## How It Works

1. **Choose a workflow** based on content type
2. **Follow the analysis steps** to design composition
3. **Get a structured prompt** ready for your image generator

**Output:** Prompt text you can paste into Midjourney, DALL-E, Flux, Stable Diffusion, or any other AI image tool.

---

## Core Aesthetic

**Tron-meets-Excalidraw** - Digital warmth combining:
- Hand-drawn Excalidraw-style sketch lines (NOT clean vectors)
- Dark slate backgrounds for modern contrast
- Neon orange (warmth) + cyan (tech) accents
- Subtle glows on key elements

**Full aesthetic documentation:** `${PAI_DIR}/skills/CORE/aesthetic.md`

**This is the SINGLE SOURCE OF TRUTH for all visual styling.**

---

## Workflow Routing

| Content Type | Workflow |
|--------------|----------|
| Blog headers / Editorial | `workflows/workflow.md` |
| Adaptive orchestrator | `workflows/visualize.md` |
| Flowcharts / Sequences | `workflows/mermaid.md` |
| Architecture diagrams | `workflows/technical-diagrams.md` |
| Classification grids | `workflows/taxonomies.md` |
| Chronological | `workflows/timelines.md` |
| 2x2 matrices | `workflows/frameworks.md` |
| X vs Y | `workflows/comparisons.md` |
| Screenshot markup | `workflows/annotated-screenshots.md` |
| Step-by-step | `workflows/recipe-cards.md` |
| Quote cards | `workflows/aphorisms.md` |
| Idea territories | `workflows/maps.md` |
| Big numbers | `workflows/stats.md` |
| Sequential panels | `workflows/comics.md` |

---

## Quick Decision Tree

```
What does user need?

├─ Unsure which approach? → VISUALIZE (analyzes & orchestrates)
├─ Flowchart/sequence/state diagram? → MERMAID
├─ Abstract metaphor for article? → Editorial (workflow.md)
├─ System/architecture with labels? → Technical Diagram
├─ Categories in grid? → Taxonomy
├─ Change over time? → Timeline
├─ 2x2 matrix or mental model? → Framework
├─ Side-by-side contrast? → Comparison
├─ Markup existing screenshot? → Annotated Screenshot
├─ Step-by-step process? → Recipe Card
├─ Quote as social visual? → Aphorism
├─ Idea territories as map? → Conceptual Map
├─ Single striking number? → Stat Card
└─ Multi-panel story? → Comic
```

---

**For complete visual styling rules, ALWAYS read:** `${PAI_DIR}/skills/CORE/aesthetic.md`
