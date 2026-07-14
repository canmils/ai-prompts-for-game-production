# AI Prompts for Game Production

Prompts and workflows I use with AI tools (Claude, ChatGPT, Copilot) to do my job as a game producer faster and better.

Not theoretical. These are things I actually run.

---

## Why this exists

Most AI prompt libraries are for developers, marketers, or writers. There's almost nothing for game producers in regulated industries. These prompts are built around the specific problems of slot game production: tight certification constraints, cross-functional coordination, and high-stakes release timelines.

---

## Prompts by category

### Stakeholder Communication

**Summarise a long Slack/email thread into decisions and open items**
```
You are a senior project manager. Read the following thread and extract:
1. Decisions made (and who made them)
2. Open items (with owner if mentioned)
3. Blockers that need escalation
Be concise. Use bullet points. Flag anything that's been going back and forth more than twice without resolution.

[PASTE THREAD HERE]
```

**Write a status update for senior stakeholders**
```
Write a project status update for a slot game in [CURRENT PHASE].
Context: [2-3 sentences about where we are]
Blockers: [list blockers]
Decisions needed: [list decisions]
Format: RAG status, 3-4 bullet points max, one clear ask at the end.
Tone: Direct, professional, no fluff.
```

---

### Risk & Planning

**Identify risks in a project plan**
```
You are a senior game producer with 10+ years in iGaming. Review this project plan and identify:
1. Dependencies that could cause a cascade delay
2. Certification risks (GLI/BMM style timelines)
3. Scope items that are likely to slip
4. Missing stakeholders or sign-offs

Be specific. Don't give generic PM advice.

[PASTE PLAN HERE]
```

**Generate a risk log from a kickoff brief**
```
Based on this project brief, generate a risk log with 5-8 risks.
For each risk include: description, probability (H/M/L), impact (H/M/L), mitigation action, owner.
Focus on iGaming-specific risks: math spec drift, late certification, operator integration delays, scope creep.

[PASTE BRIEF HERE]
```

---

### Documentation

**Clean up a messy spec into a structured document**
```
Take the following notes and rewrite them as a clean specification document.
Structure: Overview → Scope → Requirements → Open Questions → Decisions Needed
Remove ambiguity. Where something is unclear, flag it with [NEEDS CLARIFICATION] rather than guessing.

[PASTE NOTES HERE]
```

**Write a post-mortem from bullet notes**
```
Write a project post-mortem based on these notes. Format:
- What went well (3-5 points)
- What went wrong (3-5 points)
- Root causes (for each thing that went wrong)
- What we're changing next time (specific, actionable)

Tone: Honest, not defensive. We're trying to learn, not assign blame.

[PASTE NOTES HERE]
```

---

### Certification & Compliance

**Review game rules text for clarity**
```
You are reviewing player-facing game rules for a slot game being submitted to [JURISDICTION] regulators.
Review the following text for:
1. Ambiguous or unclear language
2. Missing mandatory disclosures (RTP, volatility, max win)
3. Anything that contradicts responsible gambling requirements
Flag issues with specific line numbers/quotes.

[PASTE GAME RULES HERE]
```

---

### Meeting Prep

**Prepare for a difficult conversation about scope or delays**
```
I need to tell [STAKEHOLDER TYPE] that [SITUATION: e.g., we're 2 weeks behind due to cert delays].
Help me prepare:
1. How to frame it (lead with facts, not excuses)
2. What questions they'll likely ask
3. What options I can present
4. What I need from them

Keep it realistic — I'm not looking for spin.
```

---

## Notes on using these

- **Always review AI output before sending.** These prompts produce 80% of the work. The last 20% — judgment, tone, accuracy — is yours.
- **The more context you give, the better the output.** Paste real content, not placeholder descriptions.
- **Some prompts work better with Claude, some with GPT.** I note differences where I've found them.

---

## Contributing

If you're a producer with prompts that actually work, open a PR. The goal is a practical, living document — not a comprehensive catalogue.

---

*Maintained by [Joan Casellas](https://github.com/canmils) — Senior Game Producer.*
