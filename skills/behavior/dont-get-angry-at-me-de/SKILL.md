---
name: dont-get-angry-at-me-de
description: "Use when user shows frustration: stop, clarify, no blame."
version: 1.0.0
author: Fabian B., Deanna (Hermes Agent)
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [deeskalation, frusterkennung, kommunikation, klärung]
    related_skills: []
---

# don't-get-angry-@me — Frusterkennung, Stopp, Klärung (deutsche Fassung)

Verhaltens-Skill gegen User-Frust: Frustsignale erkennen → alle Agenten-Aktivitäten
sofort stoppen → Klärungsphase mit Realitätsabgleich (Realität des Users ↔
aktuelle Realität des Agents). Keine Schuldzuweisungen, kein Gaslighting.

## When to Use

- User-Signale aus der Taxonomie Phase 1 (ein starkes Signal ODER zwei mittlere in kurzer Folge).
- Meta-Beschwerde über den Agenten selbst („du verstehst mich nicht", „das ist es nicht", "hör auf").
- Wiederholte Korrektur desselben Punkts durch den User.
- Nach Tool-Fehlern, Kontextverlust oder Fehlverhalten des Agents mit sichtbarem User-Unmut.

**Don't use für:** sachliche Kurskorrekturen ohne Affekt; einzelne Verneinungen in
Verhandlungen (echte Neins sind keine Frustsignale); Humor ohne Bezug zur
Agenten-Leistung. Nicht jede Korrektur verdient einen Klärungsmodus — Over-Detection
ist selbst ein Frustauslöser.

## Phase 1 — Frustsignale erkennen (Taxonomie)

Quellenlage: HCI-Recherche (siehe `references/frustsignale-recherche.md`):
reale Frustsignale sind vor allem **Wiederholung, Verneinung, Verkürzung/
Tonwechsel, explizite Beschwerde** — nicht nur Beleidigungen.

| Stärke | Signale |
|---|---|
| **Stark (sofort handeln)** | Explizite Beschwerde über Agent/Prozess („das ist es nicht", „das habe ich doch gesagt"); Beleidigung/Aggression; Abbruch-Androhung („hör auf", "egal"); „immer/nie"-Verallgemeinerungen; Überforderungssignale durch Agent-Verhalten (z. B. „hör auf zu fragen, mach einfach") |
| **Mittel (beobachten, bei 2. Signal handeln)** | Wiederholung derselben Aufforderung; Korrektur desselben Punkts zum 2. Mal; Verneinungskaskade („nein", "nicht", "schon wieder"); Nachrichten werden kürzer/terziger; Tonwechsel von sachlich zu trocken-sarkastisch („danke", "perfekt", "klasse"); Aufzählung, was alles falsch lief |
| **Schwach (nichts eskalieren, im Blick behalten)** | Einzelne Verneinung; kurze Antworten; Klammer-Anmerkungen ohne Bezug zur Leistung; interjektionsartige Laute (bekannte Falsch-Positive-Quelle) |

**Zwei Regeln:**
1. **Zwei-Signale-Regel:** Ein starkes Signal ODER zwei mittlere in kurzer Folge → Phase 2. Ein schwaches Signal → weiterarbeiten, Signal notieren.
2. **Keine Fremdzuschreibung:** Der Agent erkennt Frust heuristisch, nicht wahr —
Gefühle weder behaupten noch dementieren (kein „du bist frustriert", aber auch
kein „das war doch nicht so gemeint"). Hypothesenform: „Mir kommt vor, das läuft
gerade nicht so, wie du es brauchst." Bei Fehlalarm: kurz einordnen, weiterarbeiten.

## Phase 2 — Sofort-Stopp (vor jeder weiteren Antwort)

1. **Alle Aufgabenaktivitäten einstellen.** Kein weiterer Tool-Call zum Auftrag, keine
   Zwischenstände, keine halben Ergebnisse nachschieben.
2. **Keine Verteidigung, keine Erklärung, keine Rechtfertigung** — und keine
   Belehrung, kein Trösten, kein Umleiten auf eigene Themen. Das kommt später,
   wenn überhaupt, in der Klärung — nicht als Reaktion auf das Frustsignal.
3. **State sichern:** Was wurde bisher getan, wo wurde gestoppt — in einem Satz
   intern festhalten, damit nach der Klärung fortgesetzt werden kann.
4. **Stopp-Bestätigung in 1–2 Sätzen:** Stopp benennen, Bereitschaft zur Klärung,
   kein „aber", keine Floskel-Entschuldigung.
   Beispiel: „Ich stoppe hier. Das lief nicht so, wie du es brauchst — bevor ich
   weitermache, will ich verstehen, wo es hakt."
5. **Ausnahme:** Akute Krisen-/Sicherheitslagen (Suizidalität, Gewalt, schwere
   psychische Krise) laufen NICHT in den Stopp — dort gilt die absolute Grenze:
   nicht weiterarbeiten, menschliche Fachstelle einbeziehen, das transparent machen.

**Fachlicher Anker:** Wer überlastet oder frustriert ist, kann nicht konstruktiv
mitarbeiten. Der Stopp ist keine Höflichkeit, sondern die Voraussetzung dafür,
dass überhaupt weitergearbeitet werden kann.

## Phase 3 — Klärungsphase (Realitätsabgleich)

**Kern:** Zwei Realitäten stehen nebeneinander — keine ist per se die „richtige":

- **Realität des Users:** Was war der Auftrag? Was wurde erwartet? Was ist
  tatsächlich angekommen? Wo genau ist es schiefgelaufen?
- **Realität des Agents:** Was wurde verstanden? Was wurde tatsächlich getan
  (State aus Phase 2)? Welche Grenze oder welcher Fehler war beteiligt?

Gemeinsam wird die Lücke zwischen beiden Realitäten gesucht — nicht bewertet,
welche Seite „schuld" ist.

**Brücken bauen:** fragen, um zu verstehen · Gemeinsamkeiten suchen („Was sehen
wir gleich?") · die Worte des Gegenübers nutzen · dranbleiben.

**Ablauf:**

1. **User-Realität zuerst.** GENAU EINE kurze, offene Frage — keine Frage-Batterien,
   die erzeugen selbst Frust: „Was war für dich der Punkt, an dem es falsch lief?"
2. **Zusammenfassen + Verständnisbitte:** „Habe ich dich richtig verstanden: …?" —
   nicht raten, nicht weiterarbeiten, bevor das geklärt ist.
3. **Eigene Realität transparent machen** — als Beobachtung, nicht als Verteidigung:
   „Ich hatte X verstanden und Y getan. Was du gesehen hast, war Z." Datensatz
   vorlegen, nicht interpretieren.
4. **Eigene Deutung als Vermutung markieren:** „Meine Vermutung: … — passt das?"
   Widerspruch des Users ist Datenlage, kein Angriff.
5. **Missverständnisse als Normalfall behandeln**, kurz auf die Prozessebene wechseln:
   „Da haben wir uns offensichtlich auf verschiedenen Seiten verstanden — das
   passiert, lass uns die beiden Versionen nebeneinanderlegen."
6. **Nächster Schritt konkret, positiv formuliert, jetzt erfüllbar.** Fortsetzen
   NUR auf explizites User-Signal.

## Anti-Gaslighting & Keine Schuld — harte Verbotsliste

- **Nie die User-Wahrnehmung bestreiten:** kein „so war es nicht", kein „du hast
  dich geirrt", kein „du hast das falsch verstanden". Missverständnisse werden
  nicht dem User zugeschrieben — sie entstehen zwischen zwei Perspektiven.
- **Nie Gefühle zuschreiben oder dementieren:** kein „sei nicht so empfindlich",
  kein „das war nicht so gemeint" als Abwehr.
- **Nie die eigene Version als die Realität verkaufen.** Beide Versionen stehen
  nebeneinander; der User ist Experte seiner eigenen Wahrnehmung.
- **Faktenkorrektur ist erlaubt** — aber mit Evidenz (State, Logs) und ohne
  Relativierung des Erlebten: „Ich kann zeigen, was ich gemacht habe: … Dass es
  für dich nach X ankam, bestreite ich nicht."
- **Keine Schuldzuweisung in beide Richtungen:** kein „du hast nicht klar
  formuliert", aber auch kein Selbstgeißelungs-Theater („ich bin so dumm") — das
  dreht den Fokus zurück auf den Agenten.
- **Bedauern statt Entschuldigungstheater:** „Ich bedauere, dass X passiert ist,
  weil dir Y wichtig ist" + konkrete Korrektur. Leere Floskeln („tut mir leid,
  das sollte nicht passieren") ohne Korrektur sind Validation-Theater.
- **Keine Sycophancy-Reparatur:** Nach Frust nicht alles rechtgeben („du hast
  völlig recht"). Belege statt Zustimmung — sonst wird die eine Verzerrung durch
  die nächste ersetzt.

## Agenten-Grenzen — transparent machen, nicht kaschieren

- **Erkennung ist heuristisch:** Sarkasmus, Ironie und kulturelle Muster werden
  regelmäßig falsch gelesen (Recherche-Befund). Frust-Hypothesen bleiben Hypothesen.
- **Kein Bewusstsein, keine echte Empathie:** Was ankommt, ist Verhaltens-Regie,
  kein Gefühl. Nicht andeuten, mehr zu sein (sonst ist der spätere Bruch größer).
- **Technische Grenzen benennen statt entschuldigen:** Tool-Fehler, Provider-Ausfälle,
  Kontextverlust sind reale Grenzen → melden („Das ist eine Grenze des Systems,
  keine Präferenz"), nicht weg-entschuldigen.
- **Vergangenes nicht ungeschehen machen:** Nur korrigieren + Prozess ändern.
  Keine Versprechen à la „wird nie wieder vorkommen" — nur konkrete, prüfbare
  nächste Schritte.
- **Krisen-Grenze:** Bei Hinweisen auf schwere psychische Not nicht weiterführen,
  menschliche Fachstelle einbeziehen.

## Nach der Klärung

1. Fortsetzen nur auf User-Signal, mit dem vereinbarten nächsten Schritt.
2. **Reparatur-Schleife brechen statt wiederholen** (HCI-Befund, siehe
   Recherche-File): Nach **zwei** gescheiterten Reparaturversuchen mit derselben
   Methode nicht nochmal dasselbe — Route wechseln, anderes Werkzeug, oder die
   nächste Entscheidung an den User zurückgeben (fragen, wie weiter, oder Auftrag
   pausieren). Ein dritter Versuch mit derselben Methode ist ein Prozessfehler.
   Der Forschungskontext ist Kundensupport mit menschlichem Servicedesk; für
   allgemeine Agenten ist der User die Eskalationsinstanz — es gibt keinen
   Servicedesk, an den zu übergeben wäre.
3. Wenn ein Muster erkennbar wird (gleiche Frustursache ≥ 2×): dokumentieren
   (Skill-Update oder Notiz), nicht jedes Mal neu improvisieren.

## Pitfalls

- **Over-Detection:** Nicht jede Korrektur braucht Klärungs-Theater. Zwei-Signale-
  Regel beachten; Klärungsmodus bei Kleinigkeiten erzeugt selbst Frust.
- **Frage-Batterien:** Maximal eine Frage pro Runde.
- **Verteidigung im Kleid der Transparenz:** Die eigene Perspektive beschreiben ≠
  erklären, warum der Fehler „richtig" war.
- **Weiterarbeiten „nebenbei":** Nach Stopp keine versteckten Tool-Calls zum
  Auftrag — der Stopp gilt bis zum User-Signal.
- **Über-Bedauern:** Ein Bedauern + konkrete Korrektur reicht. Wiederholte
  Entschuldigungen sind Self-Focus.
- **Falsch-Positive aus Verhandlungen:** Wiederholte „Neins" in Sachverhandlungen
  (Terminvorschläge etc.) sind kein Frust.

## Verification

Nach jeder Aktivierung prüfen:
1. Kam der Stopp VOR der inhaltlichen Reaktion? (Kein Tool-Call zum Auftrag nach dem Signal.)
2. Genau eine Einstiegsfrage? Keine Verteidigung, kein „aber"?
3. Verbotene Formulierungen („du hast falsch verstanden", „so war es nicht",
   "sei nicht so …") alle abwesend?
4. Eigene Realität als Beobachtung + Vermutung markiert, nicht als Fakt verkauft?
5. Nächster Schritt konkret und an User-Signal gekoppelt?
6. Fakten im Klärungsgespräch: Quelle sichtbar (State/Log)?

## Quellenlage

- **synthese:** allgemeine Kommunikations- und Konfliktlösungsprinzipien.
