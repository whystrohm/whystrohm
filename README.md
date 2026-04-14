### I become your brand's creative engine.

Your brand has a voice. It lives in your head — how you explain things on sales calls, in team meetings, to investors. The problem is that voice doesn't scale. It stays trapped in you.

I extract it, codify it as enforceable rules, and build a system that produces brand-consistent content without routing everything through the founder. Then I run it.

---

**Free tools** — install any of these and run them on your own content:

| Tool | What It Does | Install |
|-------|-------------|---------|
| [Digital Twin](https://github.com/whystrohm/digital-twin-of-yourself) | Reverse-engineer how you think and talk. Build a stress-tested AI System Prompt of yourself. | `git clone https://github.com/whystrohm/digital-twin-of-yourself.git ~/.claude/skills/digital-twin` |
| [Content Audit](https://github.com/whystrohm/whystrohm-audit) | Score your content against a 5-layer framework. See what's broken. Get one piece rewritten live. | `git clone https://github.com/whystrohm/whystrohm-audit.git ~/.claude/skills/whystrohm-audit` |
| [Voice Extract](https://github.com/whystrohm/whystrohm-voice-extract) | Extract a structured voice profile from any URL. 6 dimensions scored, 15+ guardrails generated. | `git clone https://github.com/whystrohm/whystrohm-voice-extract.git ~/.claude/skills/whystrohm-voice-extract` |
| [Voice Scorer](https://github.com/whystrohm/whystrohm-voice-scorer) | Measure voice drift between your website and social content. Find where the brand is leaking. | `git clone https://github.com/whystrohm/whystrohm-voice-scorer.git ~/.claude/skills/whystrohm-voice-scorer` |
| [media-tsunami](https://github.com/whystrohm/media-tsunami) | The empirical layer. Extracts brand voice as executable code — cadence, signature vocab, forbidden words, exemplar sentences — serialized as a drop-in `CLAUDE.md` any LLM can load. | `git clone https://github.com/whystrohm/media-tsunami.git && cd media-tsunami && pip install -e .` |

No API keys. No accounts. No email gates. First four install into Claude Code as skills. media-tsunami is a Python CLI that generates the files those skills consume.

---

### How they work together

```
 media-tsunami (Python CLI)
   │
   ▼  generates brand-config.json + CLAUDE.md
   │
   ├── Voice Extract .... quick conversational voice analysis
   ├── Content Audit .... scores new content against the extracted voice
   ├── Voice Scorer ..... measures social-vs-site drift using the forbidden list
   └── Digital Twin ..... layers personal voice on top of brand voice
```

**tsunami is the ground-truth layer.** It computes the empirical voice profile once — cadence statistics, vocabulary clusters, centroid-based exemplar sentences, forbidden words vs a wikitext baseline. Output is deterministic and reproducible.

**The four Claude skills are conversational operators.** They run inside Claude, fast and subjective, and can use the tsunami output as their shared reference point. Use them standalone for quick work, or chain them on top of a tsunami-generated `brand-config.json` for multi-brand consistency.

---

**Background:** 10+ years in defense systems engineering. Built production systems where the output had to be right every time. Now I apply that same discipline to content — brand voice enforced in code, not a PDF someone ignores.

**Currently serving:** 11 brands with fully automated content pipelines. Each brand has its voice codified as 40-60 enforceable rules, a video production engine, and multi-platform distribution.

[whystrohm.com](https://whystrohm.com) | [Score your content free](https://whystrohm.com/scan?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop) | [YouTube](https://youtube.com/@Whystrohm) | [LinkedIn](https://linkedin.com/in/yuri-strohm)

---

## Brand Infrastructure Consulting

This is one component of the full brand infrastructure I build for founder-led brands. The free skills extract the voice. Then I build the rest.

Voice guardrails encoded into every content pipeline. Programmatic video production. Automated publishing across all channels. One operator, full stack, 30 minutes of your time per week.

11 brands. 800+ videos. You own everything I build.

→ [whystrohm.com/pricing](https://whystrohm.com/pricing?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)

See client proof → [whystrohm.com/results](https://whystrohm.com/results?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)
