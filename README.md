# book-cover-design — AI-generated book covers with genre conventions

> Design genre-appropriate book covers using AI image generation via the inference.sh CLI. Covers 7 fiction genres and 5 non-fiction categories, with professional print specs built in.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
book-cover-design guides you through creating professional book covers that match genre reader expectations — from dark thriller aesthetics to warm romance palettes. It uses the `infsh` CLI (inference.sh) for AI image generation and bakes in standard print rules: safe zone, bleed, thumbnail test. Follows an iterative concept → generate → test → refine workflow.

## Features
**Fiction genres:** Thriller/Mystery, Romance, Sci-Fi, Fantasy, Literary Fiction, Horror, Historical
**Non-fiction categories:** Business/Self-help, Memoir, Science/Academic, Cookbook, Travel

**Print specs:**
- Thumbnail test at 80px (legibility check)
- Safe zone: 0.25" from edge
- Bleed: 0.125"
- Spine text: only for books ≥ 100 pages

## Usage / Quick Start
```bash
# Install inference.sh CLI
curl -fsSL https://cli.inference.sh | sh
infsh login

# Generate a cover concept
infsh app run falai/flux-dev-lora --input '{"prompt": "dark moody book cover...", "width": 832, "height": 1248}'
```
**Workflow:** concept → generate → thumbnail test at 80px → refine.

## Trigger Keywords (OpenClaw)
book cover, cover design, ebook cover, kindle cover, novel cover, audiobook cover, book jacket

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
