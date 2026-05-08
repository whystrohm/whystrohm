### I become your brand's creative engine.

Your brand has a voice. It lives in your head, how you explain things on sales calls, in team meetings, to investors. The problem is that voice doesn't scale. It stays trapped in you.

I extract it, codify it as enforceable rules, and build a system that produces brand-consistent content without routing everything through the founder. Then I run it.

---

**Free tools.** Install any of these and run them on your own content:

| Tool | What It Does | Install |
|-------|-------------|---------|
| [**shotkit**](https://github.com/whystrohm/shotkit) **· NEW** | Pre-production for founder-led video at scale. Turn a brief into a storyboard, shot specs, per-generator prompts, and a versioned audit trail. Four Claude Code skills. | `git clone https://github.com/whystrohm/shotkit.git && cd shotkit && ./install.sh` |
| [Ritual](https://github.com/whystrohm/ritual) | Scans your shell history + repos + Claude Code memory. Ranks your top 5 automation candidates. Drafts your first Claude Code scheduled trigger with real repo names, paste-ready. | [Download `.skill` ↗](https://github.com/whystrohm/ritual/releases/latest) |
| [Digital Twin](https://github.com/whystrohm/digital-twin-of-yourself) | Reverse-engineer how you think and talk. Build a stress-tested AI System Prompt of yourself. | `git clone https://github.com/whystrohm/digital-twin-of-yourself.git ~/.claude/skills/digital-twin` |
| [Content Audit](https://github.com/whystrohm/whystrohm-audit) | Score your content against a 5-layer framework. See what's broken. Get one piece rewritten live. | `git clone https://github.com/whystrohm/whystrohm-audit.git ~/.claude/skills/whystrohm-audit` |
| [Voice Extract](https://github.com/whystrohm/whystrohm-voice-extract) | Extract a structured voice profile from any URL. 6 dimensions scored, 15+ guardrails generated. | `git clone https://github.com/whystrohm/whystrohm-voice-extract.git ~/.claude/skills/whystrohm-voice-extract` |
| [Voice Scorer](https://github.com/whystrohm/whystrohm-voice-scorer) | Measure voice drift between your website and social content. Find where the brand is leaking. | `git clone https://github.com/whystrohm/whystrohm-voice-scorer.git ~/.claude/skills/whystrohm-voice-scorer` |
| [media-tsunami](https://github.com/whystrohm/media-tsunami) | The empirical layer. Extracts brand voice as executable code (cadence, signature vocab, forbidden words, exemplar sentences) serialized as a drop-in `CLAUDE.md` any LLM can load. | `git clone https://github.com/whystrohm/media-tsunami.git && cd media-tsunami && pip install -e .` |

No API keys. No accounts. No email gates. shotkit, Ritual, and the four skill repos install into Claude Code as skills. media-tsunami is a Python CLI that generates the files those skills consume.

---

### How they work together

```
 Ritual (orchestration layer, Claude Code scheduled triggers)
   │   scans your machine, drafts the routine that runs the rest
   ▼
 media-tsunami (Python CLI)
   │   generates brand-config.json + CLAUDE.md
   ▼
   ├── Voice Extract .... quick conversational voice analysis
   ├── Content Audit .... scores new content against the extracted voice
   ├── Voice Scorer ..... measures social-vs-site drift using the forbidden list
   └── Digital Twin ..... layers personal voice on top of brand voice
```

**Ritual is the orchestration layer.** Claude Code routines just shipped. Scheduled remote agents that run in Anthropic's cloud. Ritual tells you which one to build first based on your actual work, then hands you the paste-ready prompt. The four skills above become what the scheduled routines invoke.

**tsunami is the ground-truth layer.** It computes the empirical voice profile once: cadence statistics, vocabulary clusters, centroid-based exemplar sentences, forbidden words vs a wikitext baseline. Output is deterministic and reproducible.

**The four Claude skills are conversational operators.** They run inside Claude, fast and subjective, and can use the tsunami output as their shared reference point. Use them standalone for quick work, or chain them on top of a tsunami-generated `brand-config.json` for multi-brand consistency. Scheduled sweeps via Ritual keep them running nightly across every repo.

One operator runs both. Hundreds of videos a month, every platform, every aspect ratio.

```
 shotkit (pre-production layer, Claude Code skills)
   │   brief becomes structured storyboard files and per-generator prompts
   ▼
   ├── storyboard-architect ... brief → storyboard.md + shots.json
   ├── visual-prompt-forge .... shots → 7 generator-specific prompt files
   ├── visual-asset-critic .... QA loop on generated images
   └── storyboard-html-preview  shareable single-file HTML preview
```

**shotkit is the pre-production layer.** Brief in, structured storyboard files out. Composes with the voice tools above when the brand-pack drives the storyboard's brand-lock.

---

**Background:** 10+ years in defense systems engineering. Built production systems where the output had to be right every time. Now I apply that same discipline to content. Brand voice enforced in code, not a PDF someone ignores.

**Currently serving:** 11 brands with fully automated content pipelines. Each brand has its voice codified as 40-60 enforceable rules, a video production engine, and multi-platform distribution.

[whystrohm.com](https://whystrohm.com) | [Score your content free](https://whystrohm.com/scan?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop) | [YouTube](https://youtube.com/@Whystrohm) | [LinkedIn](https://linkedin.com/in/yuri-strohm)

---

## Brand Infrastructure Consulting

This is one component of the full brand infrastructure I build for founder-led brands. The free skills extract the voice. Then I build the rest.

Voice guardrails encoded into every content pipeline. Programmatic video production. Automated publishing across every platform, every aspect ratio. One operator, full stack, 30 minutes of your time per week.

11 brands. Hundreds of videos a month. Every platform, every aspect ratio. At scale. You own everything I build.

→ [whystrohm.com/pricing](https://whystrohm.com/pricing?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)

See client proof → [whystrohm.com/results](https://whystrohm.com/results?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)
