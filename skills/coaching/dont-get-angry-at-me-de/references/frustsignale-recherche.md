# Frustsignale bei Usern im Umgang mit Agenten/Bots — Recherche-Digest

Stand: 2026-10-18 (Korrektur 2026-10-18, Deanna: zuvor fälschlich „2026-12-10" — unverifiziertes Session-Datum. Fehler bleibt hier sichtbar). Label: **recherchiert** (Web-Recherche). Nutzung: Evidenz-
Grundlage für `dont-get-angry-at-me-de`. Allgemeine Fachgrundlage schlägt
Modellwissen — dort nicht Abgedecktes ist hier als Recherche-Befund markiert.
Keine Coaching-Methoden nennen (Urheberrecht).

## 1. Wie äußert sich Frust in realen Dialogen?

**COLING 2025 Industry — "User Frustration Detection in Task-Oriented Dialog
Systems"** (aclanthology.org/2025.coling-industry.23.pdf) — Kernbefunde aus
Daten eines produktiven Dialogsystems:

- Reale Frustsignale sind vor allem **Wiederholung** (gleiche Anfrage/gleiches
  "No" mehrfach) und **Verneinung/Negation** — nicht nur Beleidigungen.
- Explizite Signale: Profanity, Beleidigungen, direkte Beschwerden über System
  oder Gesprächsverlauf („Stupid robot, I want to speak to a human!").
- Subtile Signale: Verkürzung der Nachrichten, Terzigkeit, allgemeine
  Unzufriedenheit ohne offene Feindseligkeit, lange ungelöste Verläufe.
- **Falsch-Positive:** Sentiment-/Emotion-Modelle versagen in realen Daten:
  System-Utterances verwässern das Sentiment des Users; Interjektionen („uh",
  „ah") triggern Emotion-Modelle; sachliche Nein-Serien in Verhandlungen werden
  fälschlich als Frust gelabelt. Keyword-Listen: hohe Precision, ~1% Recall.
- In-Context-Learning-LLM-Klassifikation schneidet besser ab als Out-of-the-box-
  Sentiment-Modelle.
- Frustration führt zu abruptem Gesprächsabbruch und geringer Rückkehrwahrschein-
  lichkeit — rechtzeitige Erkennung hat direkten Nutzen.

**CoSupport (cosupport.ai) — Stress-Test GenAI gegen Sarkasmus/Wut:**

- Offener Sarkasmus (Übertreibung, schwere Zeichensetzung) wird erkannt, **subtile
  Ironie wird verfehlt** (z. B. „thanks for nothing", „this is just perfect").
- **Verkürzende, schnelle Antworten** deuten auf steigenden Frust, bevor Wut
  ausgesprochen wird; Tonwechsel höflich → terzig ist ein Indiz.
- Erfolgsrezept: **Frust zuerst anerkennen, dann lösen**; bei Eskalation an
  Menschen übergeben.

**Nature Humanities & Social Sciences Communications 2026
(s41599-026-07617-x) — „AI-supported chatbots as triggers of potential
communication crises“:**

- Zwei Ausfall-Ebenen: (1) interaktives Versagen, (2) **User-Enttäuschung** —
  emotionale Reaktion auf nicht erhaltene Geschwindigkeit/Lösung, die Zweifel
  an der Kompetenz weckt.
- „Talking wall"-Wahrnehmung: fehlende Empathie-Antworten („fühlte sich an wie
  eine Websuche") lassen aus einer operativen Störung eine **Beziehungs-/Reputations-
  krise** werden.
- Kern: User wollen **anerkannt, verstanden und wertgeschätzt** werden —
  Vertrauen wird genau dort fragil.

## 2. Warum Frust ernst nehmen (Kosten)

- **Berkeley CMR 2026** (cmr.berkeley.edu, „Chatbot Frustration is Real“):
  Frust aus Bot-Interaktionen **schlägt auf nachfolgende menschliche Agenten
  durch**; versteckte Kosten in Nachbearbeitung und Fluktuation.
- **Forbes 2023** (Umfrage, UserCamp): eine negative Chatbot-Erfahrung vertreibt
  ca. 30% der Kunden; >50% berichten, nach ausgereiztem Bot keinen Menschen
  erreicht zu haben.

## 3. Reparatur-Strategien (Evidence-based)

**MISQ 2026 (50/2) — „Overcoming Breakdowns in Customer-Chatbot Interaction:
Design and Impact of Collaborative Repair Strategies“** (misq.umn.edu):

- **Assisted Self-Repair:** User soll Breakdowns selbst beheben können, aber mit
  Unterstützung des Bots (nicht im Trial-and-Error allein lassen).
- **Diagnostic Transparency:** Ursache des Breakdowns so konkret wie möglich
  benennen — ohne Transparenz können User ihre Reparatur nicht steuern.
- **Progressive Escalation:** Assistenz stufenweise erhöhen; nach ~3 Breakdowns
  Übergabe an einen Menschen anbieten. Sonst: Reparatur-Schleifen, Geduldverlust,
  Abbruch.
- **Breakdown-Typologie:** Ursachen klassifizieren, bevor repariert wird.

**Tilburg University (ECIS) — Conversational repair strategies:**

- Vier Strategien: **Ask** (nachfragen/rephrasieren anregen), **Information**
  (Anleitung zur Wiederherstellung), **Solve Options** (Alternativen anbieten),
  **Defer** (Übergabe an Menschen).
- Negative Emotionen nach Breakdowns beschädigen **Vertrauen** messbar; Reparatur
  ohne Anerkennung der Emotion wirkt nicht.

## 4. Übersetzung in Agenten-Verhalten (Synthese)

| Recherche-Befund | Verhaltensregel im Skill |
|---|---|
| Wiederholung/Negation = stärkste reale Frustindizien | Zwei-Signale-Regel, Wiederholung als Mittel-Signal |
| Subtile Ironie wird verfehlt | Frust nur als Hypothese benennen, keine Gefühlszuschreibung |
| Sentiment-Modelle falsch-positiv bei sachlichen Neins | Nicht jede Verneinung eskalieren |
| Erst anerkennen, dann lösen | Phase 2 Stopp + Phase 3 Klärung VOR Reparatur |
| Diagnostic Transparency | Eigene Realität (State/Logs) transparent machen |
| Progressive Escalation | Nach 2 Fehlversuchen Route wechseln/übergeben |
| „Talking wall"-Risiko | Anerkennung des Erlebten, keine Verteidigung |
| Frust kippt auf Menschen/Beziehung | Stopp schützt User UND Prozess |

## 5. Grenzen der Recherche

- Quellenlage überwiegend **Customer-Service-Chatbots**, nicht KI-Agenten mit
  Tool-Executive — Übertragung ist Plausibilitäts-Schluss, markiert als solche.
- Die 30%-Forbes-Zahl ist eine Umfrage-Zahl eines Anbieters, kein Peer-Review-
  Ergebnis — als Größenordnung behandeln.
- Keine Studie misst „Gaslighting durch Agenten" direkt; die Anti-Gaslighting-
  Regeln stammen aus allgemeinen Kommunikations- und Konfliktlösungsprinzipien
  (keine proprietären Quellen), nicht aus der HCI-Literatur.
