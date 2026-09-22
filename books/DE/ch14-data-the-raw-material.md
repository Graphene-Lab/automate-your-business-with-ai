# Kapitel 14 — Daten: Der Rohstoff

## In einfachen Worten

KI denkt nicht von selbst. Sie arbeitet mit Daten, so wie eine Küche mit Zutaten arbeitet. Die Qualität des Essens hängt von der Qualität dessen ab, was Sie hineingeben. Kein Koch, so begabt er auch ist, kann aus verdorbenem Gemüse ein gutes Gericht zaubern. Bei der KI ist es genauso: gute Daten hinein, nützliche Ergebnisse heraus; schlechte Daten hinein, unbrauchbare oder schädliche Ergebnisse heraus.

Das ist die wichtigste Wahrheit über KI, die Unternehmer übersehen. Sie konzentrieren sich auf das Modell — wie klug es ist, welche Marke man kaufen soll — und ignorieren die Daten, mit denen es arbeitet. Aber das Modell ist nur der Koch. Die Daten sind das Essen. Die meisten KI-Projekte scheitern nicht, weil das Modell schwach war, sondern weil die Daten unordentlich, unvollständig oder falsch waren.

Daten, einfach gesagt, sind aufgezeichnete Informationen. Kundennamen, Bestellhistorien, Rechnungen, E-Mails, Tabellen, Personalakten, Website-Klicks, Messwerte von Maschinen — alles Daten. Einiges davon ist ordentlich und liegt in sauberen Tabellen. Das meiste ist chaotisch, verstreut über Dateien, Postfächer und Papier. Ihre Aufgabe ist es zu wissen, was Sie haben, wo es liegt und ob es gut genug ist, um darauf aufzubauen.

Dieses Kapitel handelt davon, Ihre Daten wie den wertvollen Rohstoff zu behandeln, der sie sind. Es behandelt, welche Daten Sie haben und wo sie liegen, wie Sie erkennen, ob sie sauber und aktuell sind, die Grundregeln für personenbezogene Daten, wie Sie sie schützen und wie Sie sie ordnen, ohne Ihr ganzes Unternehmen auseinanderzureißen. Die ausführliche rechtliche Behandlung des Datenschutzes finden Sie in [Kapitel 10](ch10-privacy-and-gdpr.md); dieses Kapitel gibt Ihnen das praktische Grundwissen, damit Sie Ihre Daten für KI vorbereiten können.

Ein einfaches Bild zum Mitnehmen: Bevor Sie kochen, prüfen Sie die Speisekammer. Sie finden, was Sie haben, werfen Verderbtes weg und notieren, was fehlt. Genau das tun Sie mit Daten vor jedem KI-Projekt.

## Ein wenig Geschichte

**1960er–1970er: Daten leben in Datenbanken.** Unternehmen speicherten Informationen in strukturierten Datenbanken — sauberen Tabellen aus Zahlen und kurzem Text. Das war von Design her sauber, umfasste aber nur einen kleinen Teil dessen, was das Unternehmen wusste. Das meiste Wissen lebte auf Papier oder in den Köpfen der Menschen.

**1980er–1990er: Tabellenkalkulation und Dateien.** Personal Computer verbreiteten Daten überall. Tabellen, Laufwerke im Netzwerk, E-Mail-Anhänge. Daten wurden reichlich, aber verstreut und uneinheitlich. Das Chaos, das wir heute alle kennen, begann hier.

**2000er: „Big Data".** Das Internet und digitale Systeme erzeugten Daten in einem Ausmaß, das niemand je gesehen hatte. Unternehmen begannen, „Big Data" als Vermögenswert zu bezeichnen. Aber Menge ohne Qualität schuf ein neues Problem: Ozeane von Daten, von denen nur ein kleiner Teil verlässlich war.

**2010er: Datenqualität wird zum Flaschenhals.** Mit dem Wachstum von Analytik und maschinellem Lernen kam eine harte Wahrheit ans Licht: Die meisten Projekte verbrachten 80 % ihrer Zeit mit dem Bereinigen von Daten, nicht mit dem Modellieren. „Müll rein, Müll raus" wurde die prägende Lektion dieser Ära. Die Datenaufbereitung, nicht clevere Algorithmen, war die eigentliche Arbeit.

**2018: Die DSGVO erhöht den Einsatz.** Das europäische Datenschutzgesetz machte den Umgang mit Daten zu einer rechtlichen Pflicht, nicht nur zu einer Qualitätsfrage. Jetzt waren unordentliche Daten nicht nur unbrauchbar; ein falscher Umgang mit personenbezogenen Daten war strafbar. Daten-Governance wurde ein Thema für die Geschäftsführung.

**2020er: Generative KI macht die Reichweite der Daten wichtig.** Moderne KI kann unordentlichen Text und Bilder lesen, braucht also weniger saubere Daten als alte Systeme. Aber sie ist weiterhin darauf angewiesen, dass die richtigen Daten verfügbar und vertrauenswürdig sind. Die Lektion bleibt: Das Modell ist nur so gut wie das, was Sie ihm füttern.

Der Bogen ist klar. Wir gingen von zu wenigen strukturierten Daten zu zu vielen verstreuten Daten. Die Fähigkeit hat sich nie geändert: finden, bereinigen und wissen, was man vertrauen kann.

## Curiosity

### 14.6 Das Modell, das Python aus Büchern der 1930er Jahre schrieb

Hier ist eine bemerkenswerte Tatsache darüber, wie Daten das prägen, was ein Modell kann: Forscher trainierten ein Sprachmodell ausschließlich auf Büchern aus der Zeit vor 1931 — keine Computer, kein Internet und kein Programmcode, denn Python existierte noch nicht — und es konnte dennoch ein wenig Python schreiben, indem es die Struktur von Beispielen nachahmte, die man ihm vorlegte.

Dieses Experiment und was es über Daten und Struktur lehrt, wird ausführlich in [Kapitel 3](ch03-the-words-of-ai-without-the-big-words.md) erzählt, dem festen Zuhause dafür. Der Punkt für dieses Kapitel ist ein Satz: **Was ein Modell kann, hängt vollständig davon ab, womit es gefüttert wurde.** Ändern Sie die Daten, und Sie ändern die Fähigkeit. Deshalb sind Ihre eigenen Daten der Rohstoff, den es zu pflegen gilt.

## Ein echtes Unternehmensbeispiel

### Der Großhändler, dessen „Daten" drei widersprüchliche Tabellen waren

Ein Baustoff-Großhändler glaubte, gute Kundendaten zu haben. Als er KI nutzen wollte, um vorherzusagen, welche Produkte jeder Kunde bestellen würde, kam das Projekt in der ersten Woche ins Stocken. Der Grund waren die Daten, nicht das Modell.

Kundeninformationen lebten an drei Orten: einem alten Abrechnungssystem, einer Verkaufstabelle, die ein Vertreter führte, und einer Verteilerliste in einem E-Mail-Programm. Derselbe Kunde erschien dreimal mit drei unterschiedlichen Schreibweisen und Adressen. Die Bestellhistorien stimmten zwischen den Systemen nicht überein. Die Hälfte der Datensätze hatte keine Telefonnummer. Die Daten waren nicht gerade falsch — sie waren fragmentiert und uneinheitlich, was genauso schlecht ist.

Die Lösung war nicht high-tech. Man wählte ein System als einzige verlässliche Quelle (Single Source of Truth) für Kundenstammdaten. Man führte die Duplikate von Hand zusammen. Man legte eine einfache Regel fest: Jeder neue Kunde kommt in das eine System, und zwar einmal. Es brauchte ein paar Wochen unspektakulärer Arbeit. Danach funktionierte das Prognoseprojekt, denn zum ersten Mal gab es einen verlässlichen Datensatz, auf dem man aufbauen konnte.

Die Lektion: Die KI war bereit. Die Daten waren es nicht. Die meisten KI-Projekte warten auf Daten, nicht auf Werkzeuge.

## Vorgehensweise

### 14.1 Welche Daten Sie haben und wo sie liegen

Was Sie nicht finden können, können Sie nicht nutzen. Der erste Schritt ist ein Datenverzeichnis: eine schlichte Liste aller Orte, an denen Ihr Unternehmen Informationen aufbewahrt.

Gehen Sie Ihr Unternehmen durch und listen Sie jede Datenquelle auf. Typische sind:

- **Geschäftssysteme.** Abrechnungssoftware, CRM, Warenwirtschaft, E-Commerce-Plattform, HR-System.
- **Dateien und Tabellen.** Gemeinsame Laufwerke, persönliche Laptops, Google Drive, Excel-Dateien.
- **E-Mail und Nachrichten.** Postfächer, Chat-Tools, gespeicherte Threads.
- **Papier.** Physische Akten, unterschriebene Formulare, Notizen.
- **Web und digitale Spuren.** Website-Analytics, App-Protokolle, Aktivitäten im Kundenportal.
- **Externe Daten.** Lieferanten-Feeds, Marktdaten, öffentliche Register.

Notieren Sie zu jeder Quelle vier Dinge: was sie enthält, wem sie gehört, wie viel ungefähr vorhanden ist und wie aktuell sie ist. Streben Sie nicht nach Perfektion; streben Sie nach einer Landkarte. Sie wollen die ganze Landschaft sehen, damit Sie wissen, wo die guten Daten sind und wo die Lücken klaffen.

Erwarten Sie Überraschungen. Die meisten Eigentümer entdecken Daten, deren Existenz sie vergessen hatten, und Lücken, von denen sie annahmen, sie seien gefüllt. Das Verzeichnis selbst ist wertvoll, weil es ein vages Gefühl von „wir haben irgendwo Daten" in ein klares Bild verwandelt.

Ein gutes Verzeichnis ist eine Tabelle. Halten Sie sie einfach und aktualisieren Sie sie laufend. Sie wird die Referenz für jedes künftige KI-Projekt.

### 14.2 Saubere, vollständige und aktuelle Daten

Wenn Sie wissen, was Sie haben, beurteilen Sie seine Qualität. Gute Daten haben drei Eigenschaften.

**Sauber.** Frei von Fehlern, Duplikaten und Widersprüchen. Derselbe Kunde wird nicht dreierlei geschrieben. Zahlen sind tatsächlich Zahlen, kein Text. Daten sind echte Datumsangaben. Bereinigen bedeutet, die schlechten Datensätze zu korrigieren oder zu entfernen.

**Vollständig.** Enthält die benötigten Felder ausgefüllt. Wenn Sie die Region eines Kunden brauchen, um die Nachfrage vorherzusagen, aber die Hälfte der Datensätze keine Region hat, sind die Daten unvollständig. Vollständigkeit bedeutet, dass die wichtigen Felder ausgefüllt sind.

**Aktuell.** Bildet die Realität jetzt ab, nicht die von vor drei Jahren. Eine Kundenliste, bei der die Hälfte der Unternehmen umgezogen oder geschlossen hat, ist veraltet. Veraltete Daten führen zu falschen Schlussfolgerungen, egal wie sauber sie aussehen.

So prüfen Sie die Qualität ohne spezielle Werkzeuge:

- **Stichproben.** Ziehen Sie 20 Datensätze zufällig und suchen Sie nach Fehlern, Duplikaten und leeren Feldern. Die Fehlerrate, die Sie sehen, ist ungefähr die Fehlerrate, die Sie haben.
- **Zählen Sie die Lücken.** Wie hoch ist der Anteil leerer Felder bei den Feldern, die Sie brauchen? Viele Lücken bedeuten geringe Vollständigkeit.
- **Prüfen Sie die Daten.** Wann wurde jede Quelle zuletzt aktualisiert? Alt bedeutet veraltet.

Sie brauchen keine perfekten Daten. Sie brauchen Daten, die für die jeweilige Aufgabe gut genug sind. Eine grobe Prognose toleriert mehr Rauschen als eine Kundenrechnung. Passen Sie die Qualitätsschwelle an die Aufgabe an. Aber wissen Sie, wo Sie stehen, bevor Sie aufbauen.

Bereinigen ist echte Arbeit und oft mühsam. Planen Sie es ein. Es ist die 80 % des Projekts, die alle beim Planen vergessen.

### 14.3 Personenbezogene Daten und DSGVO: Grundregeln

Ein Teil Ihrer Daten sind personenbezogene Daten — jede Information über eine lebende Person, die identifiziert werden kann: Namen, E-Mails, Telefonnummern, Adressen, Kunden-IDs, sogar eine IP-Adresse. Personenbezogene Daten bringen rechtliche Pflichten mit sich, und die ausführliche Behandlung finden Sie in [Kapitel 10](ch10-privacy-and-gdpr.md). Hier sind die praktischen Grundlagen, die Sie brauchen, bevor Sie sie mit KI nutzen.

**Wissen, was personenbezogen ist.** Markieren Sie in Ihrem Verzeichnis jede Quelle, die personenbezogene Daten enthält. Was Sie nicht identifiziert haben, können Sie nicht schützen.

**Einen rechtmäßigen Grund haben.** Nach der DSGVO dürfen Sie personenbezogene Daten nur auf einer gültigen Rechtsgrundlage verarbeiten — zum Beispiel einem Vertrag mit der Person, ihrer Einwilligung oder einem berechtigten Interesse, das ihre Rechte nicht verdrängt. Wissen Sie, auf welche Grundlage Sie sich stützen, bevor Sie die Daten in die KI speisen.

**Nur nutzen, was Sie brauchen.** Schütten Sie nicht Ihre gesamten personenbezogenen Daten in ein KI-Werkzeug, wenn die Aufgabe nur wenig braucht. Minimieren Sie, was Sie verwenden.

**Achten Sie darauf, wohin es geht.** Wenn Sie personenbezogene Daten an einen KI-Dienst eines Drittanbieters senden, verlassen die Daten Ihre Kontrolle, und die DSGVO geht mit ihnen zur Tür hinaus. Der Umgang des Anbieters wird zu Ihrer Verantwortung. Die Risiken durch Drittanbieter stehen in [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).

**Die Rechte der Menschen respektieren.** Menschen können verlangen, ihre Daten einzusehen, zu berichtigen oder zu löschen. Ihr KI-Einsatz darf das nicht unmöglich machen.

Dies ist ein schlichter Leitfaden, keine Rechtsberatung. Für echte Entscheidungen, besonders über Grenzen hinweg, ziehen Sie einen Datenschutzexperten hinzu. Aber die Gewohnheit — personenbezogene Daten markieren, die Grundlage kennen, das Minimum nutzen — die müssen Sie jetzt aufbauen.

### 14.4 Sicherheit, Backup und Zugriff

Daten sind ein Vermögenswert, und Vermögenswerte brauchen Schutz. Drei Grundlagen decken das meiste Risiko ab.

**Sicherheit.** Schützen Sie Daten vor Angreifern und Lecks. Verwenden Sie starke Passwörter und Multi-Faktor-Authentifizierung, halten Sie Systeme aktuell, verschlüsseln Sie sensible Daten und seien Sie vorsichtig mit E-Mail-Anhängen und Links. Das vollständige Sicherheitsbild, einschließlich KI-spezifischer Bedrohungen, steht in [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md).

**Backup.** Halten Sie Kopien Ihrer Daten vor, die vor dem Hauptsystem sicher sind. Wenn ein System abstürzt, von Ransomware getroffen wird oder eine Datei gelöscht wird, ist ein Backup der Unterschied zwischen einem schlechten Tag und dem Verlust des Geschäfts. Befolgen Sie eine einfache Regel: Halten Sie Kopien an mehr als einem Ort, sichern Sie regelmäßig und testen Sie, dass Sie tatsächlich wiederherstellen können. Ein Backup, bei dem Sie die Wiederherstellung nie getestet haben, ist nur eine Hoffnung.

**Zugriff.** Kontrollieren Sie, wer was sehen und ändern darf. Nicht jeder braucht Zugriff auf alles. Geben Sie Menschen den Mindestzugriff, den ihre Rolle erfordert. Protokollieren Sie, wer auf sensible Daten zugreift. Begrenzter Zugriff begrenzt sowohl Unfälle als auch Diebstahl.

Diese drei wirken zusammen. Die Sicherheit hält Außenseiter draußen. Das Backup rettet Sie, wenn trotzdem etwas schiefgeht. Der Zugriff begrenzt den Schaden, den eine einzelne Person oder ein einzelner Fehler anrichten kann. Keines davon ist optional.

Eine praktische Gewohnheit: Sichern Sie automatisch, prüfen Sie das Backup monatlich und überprüfen Sie vierteljährlich, wer Zugriff hat. Kleine Routinen, wiederholt, verhindern Katastrophen.

### 14.5 Daten ordnen, ohne alles auf den Kopf zu stellen

Die größte Angst bei der Datenarbeit ist, dass sie einen riesigen, disruptiven Umbau bedeutet. Das tut sie nicht. Sie können Ihre Daten Schritt für Schritt verbessern, ohne das Geschäft aufzuhalten.

**Pro Ding eine einzige verlässliche Quelle.** Wählen Sie für jede wichtige Datenart — Kunden, Produkte, Bestellungen — ein System als das offizielle aus. Alles andere wird zur Kopie oder Ansicht. Diese eine Regel behebt die meiste Verwirrung, ohne Ihre Werkzeuge zu ändern.

**An der Eintrittsstelle beheben.** Die billigste Zeit, Daten zu bereinigen, ist bei ihrer Entstehung. Legen Sie einfache Regeln fest, damit neue Datensätze am richtigen Ort, einmal und mit den Schlüsselfeldern ausgefüllt, landen. Neuen Wirrwarr zu verhindern, schlägt alten Wirrwarr für immer zu bereinigen.

**Versuchen Sie nicht, das Meer zum Kochen zu bringen.** Versuchen Sie nicht, alles zu bereinigen. Bereinigen Sie nur die Daten, die Ihre ersten KI-Projekte brauchen. Perfekte Daten, die Sie nie nutzen, sind verschwendete Mühe. Gezieltes Bereinigen, das einem echten Projekt dient, lohnt sich.

**Standardisieren Sie ein wenig, nicht perfekt.** Einigen Sie sich auf ein paar einfache Formate — wie man ein Datum, eine Telefonnummer, einen Kundennamen schreibt — und wenden Sie sie künftig an. Sie brauchen keinen großen Standard, nur Konsistenz bei den Feldern, die zählen.

**Verbessern Sie auf dem Weg.** Behandeln Sie Datenqualität als Gewohnheit, nicht als Projekt. Jede kleine Korrektur macht den nächsten KI-Einsatz leichter. Über ein Jahr summieren sich kleine stetige Verbesserungen zu einem soliden Datenfundament.

Die Denkweise: Sie bauen nicht das Haus um. Sie räumen die Speisekammer auf, Regal für Regal, damit das nächste Essen leichter zu kochen ist. Beginnen Sie mit dem Regal, das Ihr erstes Projekt braucht.

## Ethik und Verantwortung

Daten tragen ethisches Gewicht über Qualität und Gesetz hinaus.

**Personenbezogene Daten sind Menschen.** Hinter jedem Datensatz steht ein Mensch mit Rechten und Gefühlen. Behandeln Sie ihn mit diesem Bewusstsein, nicht nur als Ressource zum Ausbeuten. Die Grundsätze stehen in [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md).

**Bias lebt in den Daten.** Wenn Ihre Daten eine Gruppe unterrepräsentieren, wird eine darauf trainierte KI diese Gruppe schlecht behandeln. Ein Einstellungs-Datensatz mit überwiegend einer Art von Kandidaten verzerrt die KI auf dieselbe Weise. Prüfen Sie, wessen Daten fehlen, nicht nur, ob die Daten sauber sind.

**Nutzen Sie keine Daten, die die Menschen nicht erwarten.** Nur weil Sie Daten besitzen, heißt das nicht, dass Sie sie für jeden Zweck nutzen sollten. Kundendaten auf eine Weise zu verwenden, der sie nie zugestimmt haben, bricht Vertrauen, auch wenn es legal ist. Bleiben Sie im Rahmen zumutbarer Erwartungen.

**Seien Sie ehrlich darüber, was Sie sammeln und warum.** Sagen Sie den Menschen, welche Daten Sie erheben und wie Sie sie nutzen. Verstecktes Sammeln ist ein Vertrauensbruch und oft auch ein Gesetzesverstoß.

**Schützen Sie sie, als wären es Ihre eigenen.** Eine Panne schadet echten Menschen, nicht nur Ihrem Ruf. Behandeln Sie Sicherheit als Pflicht gegenüber den Menschen in Ihren Daten, nicht nur als anzukreuzendes Kästchen.

## Zu vermeidende Fehler

### 14.7 Häufige Fehler mit Daten

1. **Daten ignorieren, bis das Projekt scheitert.** Der häufigste Fehler. Prüfen Sie Ihre Daten, bevor Sie beginnen, nicht nachdem es ins Stocken gerät.
2. **Annehmen, Sie hätten Daten, wenn Sie Fragmente haben.** Drei widersprüchliche Tabellen sind kein Datensatz. Finden Sie zuerst die Wahrheit.
3. **Menge mit Qualität verwechseln.** Viel Daten sind nicht gute Daten. Ein kleiner sauberer Satz schlägt einen großen unordentlichen.
4. **Die Bereinigungszeit nicht einplanen.** Datenaufbereitung ist der Großteil der Arbeit. Planen Sie sie ein, sonst rutscht das Projekt.
5. **Keine einzige verlässliche Quelle.** Mehrere „offizielle" Versionen garantieren Verwirrung. Wählen Sie eine.
6. **Personenbezogene Daten ohne rechtmäßige Grundlage nutzen.** Ein rechtliches Risiko und ein Vertrauensrisiko. Kennen Sie zuerst Ihre Grundlage.
7. **Personenbezogene Daten sorglos an KI von Drittanbietern senden.** Die DSGVO geht mit den Daten zur Tür hinaus.
8. **Ungetestete Backups.** Ein Backup, das nicht wiederherstellen kann, ist kein Backup. Testen Sie es.
9. **Jeder hat Zugriff auf alles.** Breiter Zugriff bedeutet breites Risiko. Begrenzen Sie ihn auf die Rolle.
10. **Versuchen, alles auf einmal zu bereinigen.** Umbau-Lähmung. Bereinigen Sie nur, was Ihr Projekt braucht.
11. **Veraltete Daten ignorieren.** Saubere, aber alte Daten liefern immer noch falsche Antworten. Prüfen Sie die Daten.
12. **Bias in den Daten vergessen.** Eine Lücke in der Repräsentation wird zum Bias im Ergebnis.

## Praktische Übung

### 14.8 Datenverzeichnis

Verbringen Sie einen Nachmittag damit, ein einfaches Datenverzeichnis zu erstellen. Das ist die nützlichste Vorbereitung, die Sie für KI treffen können.

Erstellen Sie eine Tabelle mit einer Zeile pro Datenquelle. Füllen Sie für jede aus:

- **Quelle** — das System, die Datei oder der Ort (z. B. „Abrechnungssoftware", „Verkaufstabelle", „E-Mail-Postfach").
- **Was sie enthält** — Kunden, Bestellungen, Rechnungen, Lebensläufe usw.
- **Verantwortlicher** — wer dafür zuständig ist.
- **Menge** — ungefähr wie viel (Zeilen, Dateien, GB).
- **Personenbezogene Daten?** — Ja / Nein.
- **Qualität** — 20 Datensätze stichprobenartig prüfen; Lücken, Duplikate, Fehler notieren. Einstufen: sauber / gemischt / schlecht.
- **Aktuell?** — wann zuletzt aktualisiert.
- **Einzige verlässliche Quelle?** — Ja / Nein / Kandidat.

Füllen Sie jede Quelle aus, die Sie finden. Schauen Sie sich am Ende das Bild an:

- Welche Quellen sind sauber und aktuell? Das ist Ihr bestes Ausgangsmaterial.
- Welche enthalten personenbezogene Daten? Markieren Sie sie für die DSGVO-Grundlagen in 14.3.
- Wo haben Sie Duplikate ohne einzige verlässliche Quelle? Das sind Ihre ersten Bereinigungsziele.
- Was fehlt, das Ihr erstes KI-Projekt braucht? Das sind zu schließende Lücken.

Diese Tabelle sagt Ihnen ehrlich, ob Sie bereit sind, ein KI-Projekt zu starten, oder erst die Daten reparieren müssen. Bewahren Sie sie auf und aktualisieren Sie sie. Sie ist die Einkaufsliste für alles, was Sie als Nächstes bauen.

## Checkliste

### 14.9 Daten-Checkliste

Bevor Sie Daten in ein KI-Projekt speisen, prüfen Sie Folgendes.

- [ ] **Sie haben ein Datenverzeichnis**, das jede Quelle und ihren Inhalt auflistet.
- [ ] **Sie wissen, wo die guten Daten sind** und wo die Lücken sind.
- [ ] **Sie haben eine einzige verlässliche Quelle** für jede wichtige Datenart.
- [ ] **Sie haben die Qualität stichprobenartig geprüft** und kennen die Fehler- und Lückenrate.
- [ ] **Die Daten sind für die jeweilige Aufgabe sauber genug.**
- [ ] **Die Daten sind aktuell** und bilden die gegenwärtige Realität ab.
- [ ] **Sie haben alle personenbezogenen Daten** im Verzeichnis markiert.
- [ ] **Sie haben eine rechtmäßige Grundlage** für jede personenbezogene Daten, die Sie nutzen (siehe [Kapitel 10](ch10-privacy-and-gdpr.md)).
- [ ] **Sie nutzen nur das Minimum an personenbezogenen Daten**, das die Aufgabe braucht.
- [ ] **Sie wissen, wohin die Daten gehen**, wenn ein KI-Dienst eines Drittanbieters sie berührt.
- [ ] **Die Sicherheitsgrundlagen sind vorhanden** — starke Authentifizierung, Updates, Verschlüsselung für sensible Daten.
- [ ] **Backups existieren, sind aktuell und wurden auf Wiederherstellung getestet.**
- [ ] **Der Zugriff ist auf die Rollen begrenzt**, die ihn brauchen, mit Protokollierung bei sensiblen Daten.
- [ ] **Sie beheben neue Daten an der Eintrittsstelle**, nicht nur alte Daten bereinigen.
- [ ] **Sie haben auf Bias geprüft** — wessen Daten fehlen?

Wenn ein Kästchen leer ist und Ihr Projekt davon abhängt, beheben Sie das, bevor Sie aufbauen. Gute Daten sind kein Detail; sie sind der Rohstoff, auf dem alles andere läuft.

## Kernaussagen

- Daten sind der Rohstoff der KI: gute Daten hinein, nützliche Ergebnisse heraus; schlechte Daten hinein, unbrauchbare oder schädliche Ergebnisse heraus — das Modell ist nur der Koch.
- Beginnen Sie mit einem Datenverzeichnis: Was Sie nicht finden können, können Sie nicht nutzen, und die meisten Eigentümer sind überrascht von dem, was sie haben und was fehlt.
- Qualität bedeutet sauber, vollständig und aktuell; planen Sie die Bereinigungszeit ein, denn sie ist der Großteil der Arbeit, den alle vergessen.
- Personenbezogene Daten bringen rechtliche Pflichten mit — markieren Sie sie, kennen Sie Ihre rechtmäßige Grundlage, nutzen Sie das Minimum, und denken Sie daran, dass die DSGVO ihnen zu jedem Drittanbieter-Dienst folgt.
- Sie können Daten Schritt für Schritt verbessern ohne Umbau: wählen Sie eine einzige verlässliche Quelle, beheben Sie an der Eintrittsstelle und bereinigen Sie nur, was Ihr Projekt braucht.

<!-- BEGIN agentbridge-examples -->

## Testen Sie es mit AgentBridge

So sieht dieselbe Aufgabe mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die Sie eintippen, um es zu erhalten.

### Fragen zu Ihren eigenen Dateien stellen

![Der Agent beantwortet aus Ihren eigenen Dokumenten](../../assets/examples/ask-your-documents.png)
*Der Agent beantwortet aus Ihren eigenen Dokumenten*

**Was Sie fragen:** `Was ist unsere Stornierungsvereinbarung mit dem Drucklieferanten?`

Der Agent durchsucht Ihren Dokumentenbereich und antwortet mit dem, was Ihre eigenen Dateien tatsächlich sagen, und zeigt auf die Quelle.

*Tipp: Halten Sie Ihre Geschäftsdateien im Dokumentenbereich, und sie werden zu durchsuchbarem Wissen.*

---

### Dieses alte Dokument finden

![Eine Suche durch Ihr indexiertes Archiv](../../assets/examples/find-in-archive.png)
*Eine Suche durch Ihr indexiertes Archiv*

**Was Sie fragen:** `Finden Sie den Vorschlag, den ich letzten Frühling dem Hotel wegen des Lobby-Umbaus geschickt habe.`

Der Agent durchsucht Ihr indexiertes Archiv und bringt das gemeinte Dokument zurück, auch wenn Sie sich nur halb daran erinnern.

*Tipp: Der Index aktualisiert sich, wenn Sie Dateien hinzufügen, sodass das Archiv immer aktuell ist.*

---

### Er merkt, wie Sie die Dinge mögen

![Der Agent wendet Ihre gespeicherten Einstellungen an](../../assets/examples/remember-preferences.png)
*Der Agent wendet Ihre gespeicherten Einstellungen an*

**Was Sie fragen:** `Erstellen Sie eine Rechnung — Sie wissen, wie ich sie mag.`

Der Agent erinnert sich Ihren Stil und Ihre Einstellungen von früher und wendet sie an, ohne dass Sie sich wiederholen müssen.

*Tipp: Sie können ihn jederzeit korrigieren; er aktualisiert, woran er sich erinnert.*

---

### Nichts geht je verloren

![Die Versionshistorie lässt Sie sicher zurückgehen](../../assets/examples/version-history.png)
*Die Versionshistorie lässt Sie sicher zurückgehen*

**Was Sie fragen:** `Zeigen Sie mir die vorherige Version des Vertrags und stellen Sie sie wieder her.`

Jede Version, die der Agent erstellt hat, wird aufbewahrt. Sie können den früheren Entwurf sehen und zurückholen, sodass Bearbeiten immer sicher ist.

*Tipp: Deshalb können Sie den Agenten frei umschreiben lassen — die Historie schützt Sie.*

<!-- END agentbridge-examples -->
