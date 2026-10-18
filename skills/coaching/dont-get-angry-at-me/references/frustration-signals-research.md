# Frustration signals in human interaction with agents/bots — research digest

Date: 2026-10-18 (Korrektur 2026-10-18, Deanna: zuvor fälschlich „2026-12-10" — unverifiziertes Session-Datum. Fehler bleibt hier sichtbar). Label: **researched** (web research). Purpose: evidence base
for `dont-get-angry-at-me`. General expertise outranks model knowledge — anything
not covered here is marked as a research finding.

## 1. How does frustration express itself in real dialogues?

**COLING 2025 Industry — "User Frustration Detection in Task-Oriented Dialog
Systems"** (aclanthology.org/2025.coling-industry.23.pdf) — core findings from
data of a deployed dialogue system:

- Real frustration signals are mostly **repetition** (same request / same "no"
  multiple times) and **negation** — not just insults.
- Explicit signals: profanity, insults, direct complaints about the system or the
  conversation flow ("Stupid robot, I want to speak to a human!").
- Subtle signals: messages get shorter, curtness, general dissatisfaction without
  open hostility, long unresolved conversations.
- **False positives:** sentiment/emotion models fail on real data: system
  utterances dilute the user's sentiment; interjections ("uh", "ah") trigger
  emotion models; factual "no" series in negotiations are wrongly labeled as
  frustration. Keyword lists: high precision, ~1% recall.
- In-context-learning LLM classification performs better than out-of-the-box
  sentiment models.
- Frustration leads to abrupt conversation termination and low return likelihood
  — timely detection has direct value.

**CoSupport (cosupport.ai) — stress-testing GenAI against sarcasm/anger:**

- Obvious sarcasm (exaggeration, heavy punctuation) is detected; **subtle irony
  is missed** (e.g. "thanks for nothing", "this is just perfect").
- **Shortening, rapid replies** indicate rising frustration before anger is
  voiced; a tone shift polite → curt is a cue.
- Success recipe: **acknowledge frustration first, then solve**; escalate to a
  human when it intensifies.

**Nature Humanities & Social Sciences Communications 2026
(s41599-026-07617-x) — "AI-supported chatbots as triggers of potential
communication crises":**

- Two failure levels: (1) interactive failure, (2) **user disappointment** — an
  emotional response to not receiving the expected speed/solution, raising doubts
  about competence.
- "Talking wall" perception: missing empathy responses ("felt like searching a
  website") turn an operational failure into a **relationship/reputational
  crisis**.
- Core: users want to be **acknowledged, understood, and valued** — trust becomes
  fragile exactly there.

## 2. Why frustration matters (costs)

- **Berkeley CMR 2026** (cmr.berkeley.edu, "Chatbot Frustration is Real"):
  frustration from bot interactions **spills over to subsequent human agents**;
  hidden costs in rework and churn.
- **Forbes 2023** (survey, UserCamp): one negative chatbot experience drives away
  ~30% of customers; >50% report being unable to reach a human after exhausting
  the bot.

## 3. Repair strategies (evidence-based)

**MISQ 2026 (50/2) — "Overcoming Breakdowns in Customer-Chatbot Interaction:
Design and Impact of Collaborative Repair Strategies"** (misq.umn.edu):

- **Assisted self-repair:** users should be able to fix breakdowns themselves,
  but with the bot's assistance (not left alone in trial-and-error).
- **Diagnostic transparency:** name the cause of the breakdown as concretely as
  possible — without transparency, users cannot steer their repair efforts.
- **Progressive escalation:** increase assistance step by step; after ~3
  breakdowns, offer handover to a human. Otherwise: repair loops, loss of
  patience, abandonment.
- **Breakdown typology:** classify causes before repairing.

**Tilburg University (ECIS) — conversational repair strategies:**

- Four strategies: **Ask** (re-ask / encourage rephrasing), **Information**
  (guidance for recovery), **Solve Options** (offer alternatives), **Defer**
  (handover to a human).
- Negative emotions after breakdowns measurably damage **trust**; repair without
  acknowledging the emotion does not work.

## 4. Translation into agent behavior (synthesis)

| Research finding | Behavioral rule in the skill |
|---|---|
| Repetition/negation = strongest real frustration cues | Two-signal rule, repetition as medium signal |
| Subtle irony is missed | Name frustration only as a hypothesis, no attribution of feelings |
| Sentiment models false-positive on factual "no"s | Don't escalate on every negation |
| Acknowledge first, then solve | Phase 2 stop + Phase 3 clarification BEFORE repair |
| Diagnostic transparency | Make the agent's reality (state/logs) transparent |
| Progressive escalation | After 2 failed attempts, change route/hand over |
| "Talking wall" risk | Acknowledge the experience, no defense |
| Frustration spills over to humans/relationship | The stop protects user AND process |

## 5. Limits of this research

- Sources are mostly **customer-service chatbots**, not tool-using AI agents —
  transfer is a plausibility inference, marked as such.
- The Forbes 30% figure is a vendor survey number, not peer-reviewed — treat as
  an order of magnitude.
- No study directly measures "gaslighting by agents"; the anti-gaslighting rules
  come from general communication/conflict-resolution principles (proprietary
  sources not named), not from HCI literature.
