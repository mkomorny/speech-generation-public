# Speech Generation (TTS Pipeline)

> **Tri-Platform Agent Skill** for Claude Desktop / Code, Grok CLI, and Google Antigravity / Gemini.  
> High-Fidelity Text-to-Speech Synthesis Pipeline — Converts radio show scripts or multi-speaker dialogues into production speech audio using Gemini TTS via the Interactions API, applying telephone bandpass filtering to correspondent voices while preserving clean studio host audio.

---

## Overview

`speech-generation` provides standardized capabilities across conversational AI platforms:
- Automated script parsing and dynamic speaker voice assignment.
- Parallel multi-worker TTS generation with retry logic and exponential backoff.
- Telephone bandpass filter (300Hz-3.4kHz) + compression for caller segments.
- Clean studio host audio preservation without coloration.
- Single-pass audio concatenation to 24kHz 16-bit PCM master WAV.
- Tri-platform NTFS junctions connecting Claude, Grok, and Antigravity.
- Standard documentation suite: SKILL.md, HOW_TO_USE.txt, IMPLEMENTATION_PLAN.md, and README.md.

---

## Tri-Platform Architecture

Zero duplicate code across platforms. Canonical source resides in `.agents`:
- **Canonical Source**: `C:\Users\<you>\.agents\skills\speech-generation`
- **Claude**: `C:\Users\<you>\.claude\skills\speech-generation` (NTFS Junction)
- **Grok**: `C:\Users\<you>\.grok\skills\speech-generation` (NTFS Junction)
- **Antigravity**: `C:\Users\<you>\.gemini\config\skills\speech-generation` (NTFS Junction)

---

## Documentation Suite

- [`HOW_TO_USE.txt`](HOW_TO_USE.txt): Standardized user guide and prompt templates.
- [`IMPLEMENTATION_PLAN.md`](IMPLEMENTATION_PLAN.md): Feature checklist and roadmap.
- [`App Changes Tracker.html`](App%20Changes%20Tracker.html): Interactive visual version log.
- [`SKILL.md`](SKILL.md): Agent system instructions and triggers.
