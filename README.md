# dont-get-angry-@me

A behavioral skill for AI agents: **detect user frustration → stop all task
activity immediately → clarification phase with a reality check** (the user's
reality ↔ the agent's current reality). No blame, no gaslighting.

## Variants

| Path | Language |
|---|---|
| `skills/behavior/dont-get-angry-at-me/` | English (canonical) |
| `skills/behavior/dont-get-angry-at-me-de/` | German |

## What the skill does

1. **Phase 1 — Detect:** signal taxonomy (strong / medium / weak), two-signal
   rule against over-detection, no attribution of feelings.
2. **Phase 2 — Stop:** halt all task activity before reacting; no defense, no
   explanation; preserve state; 1–2 sentence stop confirmation. Crisis
   situations are the exception (human professional service instead).
3. **Phase 3 — Clarify:** reality check — user's reality first, exactly one
   question per round, agent's reality as observation (not defense), own reading
   marked as hypothesis, next step concrete and tied to an explicit user signal.
4. **Hard rules:** no gaslighting (never dispute the user's perception), no blame
   in either direction, regret + concrete correction instead of apology theater,
   no sycophancy repair. Agent limits made transparent instead of papered over.
5. **Escalation:** after two failed repair attempts with the same method — change
   route or hand over to a human (progressive escalation, HCI finding).

## Install (Hermes Agent)

Copy the desired variant into your skills directory, e.g.:

```
cp -r skills/behavior/dont-get-angry-at-me ~/.hermes/skills/
```

Skills load at session start — restart the session to activate.

## Contents of each variant

- `SKILL.md` — the skill itself (self-contained, no external dependencies).
- `references/frustration-signals-research.md` (EN) /
  `references/frustsignale-recherche.md` (DE) — research digest with sources:
  COLING 2025 (frustration detection in deployed dialog systems), MISQ 2026
  (collaborative repair strategies), Nature HSSComms 2026 (chatbot failures as
  communication crises), Berkeley CMR 2026, Tilburg ECIS (repair strategies),
  vendor stress tests.

## License

MIT — see `LICENSE`.
