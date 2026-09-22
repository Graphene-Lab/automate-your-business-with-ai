# Anhang H — KI-Risikobewertung

Bevor du ein KI-Projekt startest, frag, was schiefgehen könnte und wie schlimm es wäre. Diese Tabelle macht Risiken sichtbar, damit du sie verringern kannst, statt sie zu ignorieren. Fülle sie mit deinem Team. Tue es früh, und kehre oft dazu zurück.

## So bewertest du

Bewerte jedes Risiko auf zwei Skalen:

- **Wahrscheinlichkeit** — Wie wahrscheinlich ist es? **Niedrig / Mittel / Hoch**
- **Auswirkung** — Wie schlimm, wenn es eintritt? **Niedrig / Mittel / Hoch**

Kombiniere sie zu einem **Risikograd**:

| | Auswirkung niedrig | Auswirkung mittel | Auswirkung hoch |
|---|---|---|---|
| **Wahrscheinlichkeit hoch** | Mittel | Hoch | **Kritisch** |
| **Wahrscheinlichkeit mittel** | Niedrig | Mittel | Hoch |
| **Wahrscheinlichkeit niedrig** | Niedrig | Niedrig | Mittel |

Behandle **Kritisch** und **Hoch** als Muss-beheben vor dem Start.

## Leere Vorlage

| Risiko | Was könnte schiefgehen | Wahrscheinlichkeit | Auswirkung | Risikograd | Maßnahme | Verantwortlicher |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Ausgefüllte Beispiele

| Risiko | Was könnte schiefgehen | Wahrscheinlichkeit | Auswirkung | Risikograd | Maßnahme | Verantwortlicher |
|---|---|---|---|---|---|---|
| Falsche Daten in der KI | Mitarbeiter fügen personenbezogene Kundendaten in ein öffentliches Werkzeug ein | Hoch | Hoch | **Kritisch** | Nur freigegebene Werkzeuge; öffentliche Werkzeuge auf Firmengeräten sperren; Schulung | IT-Leitung |
| Falsche Ausgabe genutzt | KI entwirft eine Rechnung mit falschem Betrag, an Kunden gesendet | Mittel | Hoch | Hoch | Menschliche Prüfung vor dem Senden; automatische Prüfung der Summen | Buchhaltungsmitarbeiter |
| Verzerrung in Entscheidungen | Einstellungs-Werkzeug bevorzugt eine Gruppe wegen schiefer Trainingsdaten | Mittel | Hoch | Hoch | Mensch entscheidet; Ergebnisse auf Fairness prüfen; kein vollautomatisiertes Einstellen | HR-Leitung |
| Anbieter-Leck | Anbieter wird angegriffen, Kundendaten sind offen | Niedrig | Hoch | Mittel | Anbieter-Checkliste; Daten verschlüsseln; Vertragsklausel zur Panne-Benachrichtigung | IT-Leitung |
| Übermäßiges Vertrauen | Mitarbeiter hören auf zu prüfen und vertrauen der KI blind | Mittel | Mittel | Mittel | Menschliche Freigabe beibehalten; Stichproben-Prüfungen; Schulung zu den Grenzen | Teamleiter |
| Prompt-Injection | Ein Dokument versteckt Anweisungen, die die KI täuschen | Mittel | Mittel | Mittel | Fremden Text als nicht vertrauenswürdig behandeln; begrenzen, was die KI damit tun kann | IT-Leitung |
| Lock-in | Kann den Anbieter nicht verlassen oder Daten exportieren | Niedrig | Mittel | Mittel | Datenexport-Klausel im Vertrag; eine Kopie behalten | Inhaber |
| Kostenüberschreitung | Nutzung wächst, die Rechnung springt | Mittel | Mittel | Mittel | Nutzungs-Alarme setzen; Tarif monatlich prüfen; Kosten pro Aufgabe deckeln | Inhaber |
| Modell-Drift | Anbieter ändert das Modell, Ausgabequalität sinkt | Mittel | Mittel | Mittel | Ausgabe wöchentlich stichprobenartig prüfen; Testfälle zum Vergleich behalten | Teamleiter |

## Spaltenanleitung

- **Risiko** — Ein kurzer Name für das Risiko.
- **Was könnte schiefgehen** — Das konkrete Szenario, keine vage Sorge.
- **Wahrscheinlichkeit / Auswirkung** — Niedrig / Mittel / Hoch.
- **Risikograd** — Aus der Tabelle oben.
- **Maßnahme** — Was du tun wirst, um die Wahrscheinlichkeit oder die Auswirkung zu senken.
- **Verantwortlicher** — Die eine Person, die sicherstellt, dass die Maßnahme passiert.

## Übliche KI-Risiken zum Bedenken

Nutze diese Liste, um eigene Zeilen anzuregen:

- [ ] Personenbezogene oder sensible Daten an ein externes Werkzeug geleakt.
- [ ] Falsche Ausgabe ohne Prüfung vertraut.
- [ ] Verzerrung oder Unfairness in automatisierten Entscheidungen.
- [ ] Sicherheitsverletzung beim Anbieter.
- [ ] Prompt-Injection aus nicht vertrauenswürdigen Dokumenten.
- [ ] Shadow AI (Mitarbeiter nutzen nicht freigegebene Werkzeuge).
- [ ] Übermäßiges Vertrauen und Kompetenzverlust.
- [ ] Kostenüberschreitung, wenn die Nutzung wächst.
- [ ] Bindung an einen Anbieter.
- [ ] Nicht-Einhaltung der DSGVO oder des EU AI Act.
- [ ] Vertrauensverlust der Kunden nach einem sichtbaren Fehler.
- [ ] Modell ändert sich stillschweigend, Ausgabequalität sinkt.

## Wann du diese Bewertung wiederholen solltest

Kehre zur Tabelle zurück, wenn eines davon passiert:

- Du fügst ein neues Werkzeug, eine neue Datenquelle oder einen neuen Prozess hinzu.
- Die Nutzung wächst stark, oder das Werkzeug berührt mehr Menschen.
- Ein Vorfall oder ein Beinahe-Unfall tritt auf.
- Ein Gesetz oder eine Kundenanforderung ändert sich.
- Ein Anbieter ändert seine Bedingungen, sein Modell oder wo er Daten speichert.

## Zwei Wege, ein Risiko zu senken

Jede Maßnahme zieht an einem von zwei Hebeln:

- **Wahrscheinlichkeit senken** — das schlimme Ereignis weniger wahrscheinlich machen. Beispiel: eine Nur-freigegebene-Werkzeuge-Liste macht ein Datenleck weniger wahrscheinlich.
- **Auswirkung senken** — den Schaden kleiner machen, wenn es eintritt. Beispiel: menschliche Prüfung bedeutet, dass eine falsche Rechnung aufgefangen wird, bevor sie den Kunden erreicht.

Ein guter Plan zieht oft an beiden. Frage bei jedem Risiko: „Was macht das weniger wahrscheinlich, und was begrenzt den Schaden, wenn es trotzdem passiert?"

Wenn ein Risiko auch nach der Maßnahme **kritisch** bleibt, starte nicht. Entferne den riskanten Schritt oder gestalte den Prozess neu.

## Regeln

- Jedes kritische oder hohe Risiko braucht vor dem Start eine Maßnahme **und** einen Verantwortlichen.
- Eine Maßnahme ohne Verantwortlichen ist keine Maßnahme.
- Wiederhole diese Bewertung bei jedem Meilenstein — Risiken ändern sich.
- Wenn ein kritisches Risiko nicht gesenkt werden kann, starte nicht. Sag das.
