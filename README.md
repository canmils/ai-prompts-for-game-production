# AI Prompts for Game Production

Editable prompt templates for communication, planning and documentation in game production.

**Status: documentation library.** Copy a template into your chosen AI tool, use fictional or permitted input and review the draft. No app, installation or API integration is included; time savings have not been measured.

---

## Why this exists

These templates focus on slot production tasks: certification dependencies, cross-functional coordination, release timelines and source-based reporting.

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
Review player-facing game rules for clarity against the supplied requirements.
1. Identify ambiguous wording and internal contradictions.
2. Compare the text to the supplied, dated jurisdiction requirements and approved math/specification.
3. Quote the source and rule-text location for every potential discrepancy.
4. If a requirement or specification is missing, label the topic UNVERIFIED and ask for it. Do not invent legal requirements or approve compliance.

Jurisdiction and version: [JURISDICTION / GAME VERSION]
Requirements and approved specification: [PASTE PERMITTED SOURCES]
Game rules: [PASTE GAME RULES HERE]

Output: issues for a human compliance reviewer, not a certification decision.
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

- **Always review AI output before sending.** Verify facts, owners, dates and source support. There is no measured percentage of work automated.
- **Supply relevant context.** Use fictional examples or material permitted by your organisation and provider settings. Flag missing facts rather than inviting guesses.
- **Record model and date when comparing results.** Outputs vary; no model-quality benchmark is provided here.

---

## Contributing

If you're a producer with prompts that actually work, open a PR. The goal is a practical, living document — not a comprehensive catalogue.

---

*Maintained by [Joan Casellas](https://github.com/canmils) — Senior Game Producer.*

## Start in five minutes

No installation or key is needed to read these prompts. Use your chosen AI tool under its own account/billing terms. Pick a prompt, replace bracketed placeholders and paste fictional or permitted input. Example: ask the status-update prompt to summarize “Art finished; QA starts Monday; audio approval pending with Alex.” Compare every output fact and owner to the source. Expected result: a draft you review and adapt; nothing is automatically sent.

Download ZIP or clone:

```sh
git clone https://github.com/canmils/ai-prompts-for-game-production.git
cd ai-prompts-for-game-production
```

Do not paste private company or personal data unless that provider/workflow is permitted. Prompts do not verify current law or certify game rules. To validate a change, include a fictional input/output example and inspect placeholders.

## Review, update and contribute

There is no server, runtime or dependency installation to troubleshoot. If a prompt produces an inaccurate draft, compare it with the supplied source, note the model/date and revise the instructions or context.

To update a local clone, inspect `git status`, preserve edits on your branch and run `git pull --ff-only`. You can also read the latest templates directly on GitHub.

For a change, include a fictional input, an illustrative output and the specific review criteria: correct facts, preserved uncertainty, clear owners and no invented approvals. Label sample outputs as authored or model-generated. Do not describe one example as proof of general quality.

Report suggestions at https://github.com/canmils/ai-prompts-for-game-production/issues. See [CONTRIBUTING.md](CONTRIBUTING.md) for the review workflow and [ONBOARDING_CHECKS.md](ONBOARDING_CHECKS.md) for verification limits.

## License

MIT; see [LICENSE](LICENSE). External inputs/content retain their own rights.
