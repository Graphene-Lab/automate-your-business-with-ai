# Kapitel 31 — Ein kleines Produktionsunternehmen

*Dieses Kapitel ist ein typisches Beispiel, kein einzelnes echtes Unternehmen. Es bündelt die Muster, die wir oft bei kleinen Maschinenbau- und Fertigungsbetrieben sehen, die KI einführen. Alle Zahlen sind Beispiele — sie zeigen, wie eine Entscheidung aussieht, kein Versprechen. Ersetze sie durch deine eigenen.*

## Kontext

Stell dir eine kleine Feinmechanik-Werkstatt vor. Wir nennen sie **Northgate Machining**. Sie beschäftigt etwa fünfundzwanzig Leute. Sie fertigt Metallteile nach Kundenwunsch — Einzelstücke und kleine Serien für andere Fabriken. Nichts liegt im Regal und wartet auf einen Käufer. Jedes Teil beginnt mit einer Kundenanfrage.

Die Arbeit beginnt mit einer **RFQ**, das steht für „request for quote", also eine Angebotsanfrage. Ein Kunde schickt eine Zeichnung per E-Mail — meist ein PDF mit der Form des Teils, seinen Maßen und dem Material, aus dem es sein muss. Der Betrieb muss sich die Zeichnung ansehen, herausfinden, wie lange jeder Schneide- und Finish-Schritt dauert, die Kosten für das Metall und die Maschinenzeit zusammenzählen und einen Preis zurückschicken. Dieser Preis ist das Angebot. Ist er zu hoch, geht der Kunde woanders hin. Ist er zu niedrig, gewinnt der Betrieb den Auftrag, verliert aber Geld bei der Fertigung.

Zwei erfahrene Kalkulatoren machen das meiste davon. Sie machen das seit Jahren. Sie sehen eine Zeichnung und wissen ungefähr, was sie kostet. Aber „ungefähr" trägt in diesem Satz schwer. Der Betrieb hat keine schriftlichen Aufzeichnungen darüber, was vergangene Angebote in der Produktion tatsächlich gekostet haben. Das Wissen steckt in zwei Köpfen. Wenn diese beiden im Urlaub sind, kommt die Kalkulation nur noch im Schneckentempo voran.

Hinter der Kalkulation liegt der Rest der Werkstatt. Rohe Metallbestände — Stangen, Platten, Rundstäbe — werden in einer Tabelle verfolgt, die aktualisiert wird, wenn jemand daran denkt. Qualitätssicherung ist eine letzte Sichtprüfung von Hand am Ende des Auftrags. Die Wochenberichte für die Inhaberin tippt jemand von Hand aus drei verschiedenen Tabellen. Nichts ist miteinander verbunden. Alles hängt davon ab, dass Leute daran denken, Dinge aufzuschreiben.

Das ist ein normaler, gesunder kleiner Hersteller. Er ist profitabel. Er ist ausgelastet. Und er lässt an vier Stellen Geld liegen: Kalkulation, Lager, Qualität und Berichte.

## Das Problem

Die Inhaberin Elena spürt die Probleme, kann sie aber nicht immer sehen. Nennen wir sie beim Namen.

**Kalkulieren ist langsam und uneinheitlich.** Ein einfaches Teil dauert eine Stunde in der Kalkulation. Ein komplexes einen halben Tag. Im Schnitt sind es zwei Tage von der eingehenden E-Mail bis zum hinausgehenden Angebot. In dieser Zeit hat der Kunde schon zwei andere Werkstätten gefragt. Tempo zählt. Schlimmer noch: Die beiden Kalkulatoren bewerten dieselbe Zeichnung unterschiedlich. Der eine ist vorsichtig und kalkuliert hoch. Der andere ist aggressiv und kalkuliert niedrig. Über ein Jahr gesehen sind manche Aufträge still und leise unterpreisig. Der Betrieb gewinnt sie, baut sie und merkt später, dass die Maschinenzeit mehr gekostet hat, als der Preis abdeckte. Diese Verluste sind unsichtbar, weil niemand hinterher das Angebot mit den tatsächlichen Kosten vergleicht.

**Lager ist Raten.** Der Betrieb kauft Metall nach, wenn jemand merkt, dass das Regal leer wird. Zu oft ist das zu spät — ein Auftrag verzögert sich, weil die richtige Stange nicht vorrätig ist. Genauso oft kauft er zu viel, und teures Material liegt monatelang und bindet Geld. Die Tabelle stimmt nie ganz. Niemand vertraut ihr, also prüfen die Leute doppelt, indem sie zum Regal laufen — das verschwendet Zeit.

**Qualitätsfehler kommen zu spät ans Licht.** Ein schlechtes Teil findet man oft erst bei der Endkontrolle, nachdem der ganze Auftrag fertig ist. Wenn der Fehler beim ersten Schnitt passiert ist, hat der Betrieb vielleicht fünfzig schlechte Teile gebaut, bevor es jemand merkt. Das ist Ausschuss — weggeworfenes Material und Maschinenzeit. Einen Fehler nach fünfzig Teilen zu finden statt nach einem ist das fünfzigfache an Verlust.

**Berichte fressen Stunden.** Jeden Freitag verbringt jemand drei oder vier Stunden damit, Zahlen aus den Tabellen zu ziehen, um eine Zusammenfassung für Elena zu erstellen. Diese Zeit ist reine Verwaltung — sie produziert keine Teile und gewinnt keine Kunden.

Jedes davon ist ein kleines Leck. Zusammen saugen sie echtes Geld und echte Zeit ab. Wenn du sehen willst, wie diese vier Aktivitäten gegen den Rest deines Unternehmens abschneiden, ist die Impact-Effort-Methode in [Kapitel 12 — Wo KI deinem Unternehmen helfen kann](ch12-where-ai-can-help-your-business.md) der richtige Ort, um sie zu bewerten.

## Die Lösung

Elena versucht nicht, „KI überall einzusetzen". Sie pickt die vier Lecks heraus und arbeitet sie einer nach dem anderen ab, beginnend mit dem größten und einfachsten.

**Klugere Kalkulation.** Statt jede Zeichnung von Grund auf zu lesen, speist der Betrieb seine vergangenen Aufträge in ein System. Für jeden vergangenen Auftrag erfasst er jetzt zwei Dinge, die er nie verknüpft hat: das ursprüngliche Angebot und die tatsächlichen Produktionskosten. Mit der Zeit wird das eine Referenzbibliothek. Wenn eine neue Zeichnung eintrifft, liest ein KI-Assistent das PDF, zieht die wichtigsten Merkmale heraus — die Maße, die Toleranzen (wie genau jede Messung sein muss), das Material, die Stückzahl — und schlägt einen Preis vor, basierend auf ähnlichen vergangenen Aufträgen. Der Kalkulator beginnt nicht mehr mit einem leeren Blatt. Er beginnt mit einem Entwurf und passt ihn an. Die KI macht den ersten Durchgang; der Mensch trifft die Entscheidung.

**Ein Lager, das vorhersagt.** Der Betrieb verbindet seine Lagertabelle mit einem einfachen Prognose-Tool. Das Tool schaut, wie schnell jedes Material verbraucht wird, und schlägt vor, wann und wie viel nachzubestellen ist. Es gibt die Bestellung nicht selbst auf. Es bringt einen Vorschlag: „Diese Aluminiumstange geht in neun Tagen aus; bestell jetzt." Ein Mensch bestätigt. Aus dem Raten wird ein Prompt.

**Qualitätsprüfung an der Maschine.** Statt nur am Ende zu prüfen, stellt der Betrieb eine kleine Kamera an eine Maschine. Ein Computer-Vision-System — KI, die liest, was eine Kamera sieht — schaut sich jedes Teil an, wenn es von der Maschine kommt, und markiert alles, was falsch aussieht: ein Riss, ein falsches Maß, ein fehlendes Loch. Der Bediener sieht die Markierung sofort und stoppt, bevor er fünfzig schlechte Kopien macht. Die letzte menschliche Kontrolle bleibt; die Kamera verlagert die Warnung nur nach vorne. (Die tiefere Behandlung von bildbasierter Qualitätskontrolle und vorausschauender Wartung ist in [Kapitel 29 — Betrieb und Produktion](ch29-operations-and-production.md).)

**Berichte, die sich selbst schreiben.** Die Tabellen sind mit einem Berichts-Assistenten verbunden. Am Freitag bekommt Elena statt zu tippen eine fertige Zusammenfassung: kalkulierte Aufträge, gewonnene Aufträge, Ausschussquote, Lagerbestände, gebundenes Geld. Sie liest und bearbeitet. Aus drei Stunden werden fünfzehn Minuten.

Beachte das Muster in all diesen vier. Die KI handelt nie allein. Sie liest, schlägt vor, markiert und erstellt Entwürfe. Ein Mensch entscheidet, bestätigt und genehmigt. Das ist dasselbe Muster „Mensch prüft den Maschinenentwurf", das der Elanco-Fall in [Kapitel 25 — Verwaltung und Finanzen](ch25-administration-and-finance.md) zeigt. In einer Werkstatt, wo eine falsche Zahl echtes Geld kosten kann, ist diese Regel nicht optional.

## Die Werkzeuge

Nichts davon brauchte ein Team von Ingenieuren. Die Werkzeuge sind von der Stange, für kleine Unternehmen gedacht.

- **Ein Dokumenten-Lese-Assistent**, der die Zeichnungs-PDF öffnet und Maße und Merkmale in ein strukturiertes Formular extrahiert. Das ist dieselbe Werkzeugklasse, die in [Kapitel 25](ch25-administration-and-finance.md) Rechnungen liest.
- **Ein Kalkulations-Assistent**, der darauf aufbaut und die extrahierten Merkmale mit vergangenen Aufträgen vergleicht und einen Preis vorschlägt. Das kann ein Low-Code-Tool sein, das an die bestehende Kalkulationstabelle des Betriebs angeflanscht wird, verbunden wie in [Kapitel 19 — KI mit Systemen verbinden, die du schon nutzt](ch19-connecting-ai-to-systems-you-already-use.md) beschrieben.
- **Ein Prognose-Add-on** für die Lagertabelle oder das einfache ERP-System (Enterprise Resource Planning) des Betriebs. Viele Lager-Tools enthalten inzwischen eine „Nachbestellung vorschlagen"-Funktion.
- **Eine Kamera plus ein Computer-Vision-Prüfwerkzeug** an einer Maschine. Diese werden als kleine, in sich geschlossene Einheiten für Qualitätsprüfungen verkauft.
- **Ein Berichts-Assistent**, der die verbundenen Tabellen liest und die Wochenübersicht in klarer Sprache entwirft.

Wie du aus diesen auswählst, ohne dich von glänzenden Demos täuschen zu lassen, steht in [Kapitel 17 — Werkzeuge wählen, ohne sich täuschen zu lassen](ch17-choosing-tools-without-being-fooled.md). Eine Warnung speziell für eine Maschinenwerkstatt: **Zeichnungen sind vertraulich.** Eine Teilzeichnung eines Kunden ist dessen geistiges Eigentum. Bevor du Zeichnungen in ein Cloud-Tool speist, prüfe, wohin die Daten gehen und wer sie sehen kann. Für manche Betriebe ist es die sicherere Wahl, die KI auf den eigenen Rechnern zu behalten — Self-Hosting, erklärt in [Kapitel 8 — Self-Hosting: Behalte deine Daten unter Kontrolle](ch08-self-hosting-keep-your-data-under-control.md). Die Risiken, sensible Dateien an Drittanbieter zu schicken, stehen in [Kapitel 9 — Drittanbieter und Shadow-KI](ch09-third-party-services-and-shadow-ai.md).

## Die Kosten

Hier ist ein Beispiel-Budget fürs erste Jahr für einen Betrieb wie Northgate. Das sind erfundene Zahlen, um die Form zu zeigen. Nimm deine eigenen.

**Direkte Kosten.**
- Kalkulations- und Dokumenten-Assistent: etwa 9.000 € im Jahr an Abos.
- Prognose-Add-on: etwa 3.000 € im Jahr.
- Kamera und Vision-Prüfeinheit: etwa 6.000 € einmalig, plus 1.200 € im Jahr.
- Berichts-Assistent: etwa 2.400 € im Jahr.
- Einrichtung und Integration (externe Hilfe, um die Tools mit den Tabellen und der Maschine zu verbinden): etwa 10.000 € einmalig.
- Schulung der Kalkulatoren und Bediener: etwa 3.000 € einmalig.

Erstjahr-Gesamt: rund **34.600 €**. In den stabilen Jahren danach fallen die einmaligen Kosten weg und die wiederkehrenden Abos kommen auf etwa **15.600 €**.

**Indirekte Kosten.** Das sind die, die man vergisst.
- Die Kalkulatoren verbringen Stunden damit, das Tool zu lernen und seine Entwürfe zu prüfen. Das ist echte Zeit, bewertet mit ihren vollen Stundensätzen.
- Das Lern-Tief: In den ersten Wochen ist das Kalkulieren langsamer, nicht schneller, während die Leute dem neuen System vertrauen.
- Die Vision-Kamera braucht gelegentlich eine Neueichung, wenn sich das Licht oder das Teil ändert.
- Jemand muss die von der KI vorgeschlagenen Angebote und Nachbestellpunkte jeden Tag prüfen. Überspring das nie.

Die vollständige Methode, diese Kosten ehrlich zu zählen und die Einsparungen in eine Rendite-Zahl umzuwandeln, steht in [Kapitel 16 — Ziele, Kosten und Kapitalrendite](ch16-goals-costs-and-return-on-investment.md). Rechne die Mathe nicht im Kopf. Schreib sie auf.

## Die Ergebnisse

Nach einem Jahr, gemessen an der Ausgangsbasis, die Elena vor dem Start erfasst hat, sieht das Beispiel-Ergebnis so aus. Denk dran: Deine Zahlen werden anders sein. Diese zeigen, wie ein guter Fit aussehen kann, nicht wie deiner sein wird.

- **Kalkulationszeit** fiel von durchschnittlich zwei Tagen auf ein paar Stunden für die meisten Teile. Der Kalkulator prüft einen Entwurf, statt von null aufzubauen.
- **Weniger unterpreisige Aufträge.** Weil das Angebot an dem verankert ist, was ähnliche Aufträge tatsächlich kosten, wurde die Lücke zwischen Angebotspreis und realem Kosten kleiner. Der Betrieb hörte auf, still und leise Geld bei gewonnenen Aufträgen zu verlieren.
- **Gewinnquote stieg.** Schnellere Angebote bedeuteten, dass Northgate mehr RFQs innerhalb des Zeitfensters beantwortete, in dem der Kunde noch wählt.
- **Ausschuss sank.** Einen Fehler an der Maschine statt am Ende zu fangen, senkte verschwendetes Material und Maschinenzeit. Statt fünfzig schlechter Teile fing der Bediener es beim ersten oder zweiten.
- **Lagerumschlag verbesserte sich.** Weniger Lieferengpässe bedeuteten weniger verzögerte Aufträge. Weniger Übereinkauf bedeutete weniger Geld, das im Regal festliegt.
- **Berichte** gingen von drei oder vier Stunden Tippen auf etwa fünfzehn Minuten Lesen und Bearbeiten.

Der ehrliche Vorbehalt: Nichts davon geschah an Tag eins. Der Kalkulations-Assistent war im ersten Monat rau, weil die Bibliothek vergangener Aufträge dünn war. Die Vision-Kamera gab Fehlalarme, bis sie kalibriert war. Die Einsparungen stiegen über Wochen an, genau wie die Lernkurven-Warnung in [Kapitel 16](ch16-goals-costs-and-return-on-investment.md) vorhersagt. Elena maß die echten Zahlen nach dem Hochlauf, nicht währenddessen.

## Gelernte Lektionen

**Fang mit der Kalkulation an.** Von den vier Lecks war die Kalkulation die mit der höchsten Wirkung und dem geringsten Risiko zum Ausprobieren. Ein falsches Angebot fängt der Kalkulator auf, bevor es rausgeht. Das machte sie zum perfekten ersten Projekt — dieselbe „hohe Wirkung, geringe Mühe zuerst"-Regel aus [Kapitel 12](ch12-where-ai-can-help-your-business.md).

**Deine vergangenen Aufträge sind der Treibstoff.** Der Kalkulations-Assistent war nur so gut wie das Protokoll vergangener Angebote und ihrer echten Kosten. Das Wertvollste, was Elena tat, war, jedes Angebot mit seinen tatsächlichen Produktionskosten zu verknüpfen. Ohne diese Daten hatte die KI nichts, woraus sie lernen konnte. Daten-Bereitschaft ist in [Kapitel 14 — Daten: Der Rohstoff](ch14-data-the-raw-material.md) behandelt.

**Die KI entwirft; der Mensch entscheidet.** Kein einziges Angebot ging raus, ohne dass ein Mensch es genehmigt hätte. Keine Nachbestellung wurde aufgegeben, ohne dass ein Mensch sie bestätigt hätte. In einer Werkstatt, wo eine falsche Zahl echtes Geld ist, ist die menschliche Kontrolle die Sicherheit, keine Verzögerung.

**Zeichnungen sind vertraulich.** Behandle jede Kundenzeichnung als sensibles geistiges Eigentum. Entscheide, wohin sie darf, bevor du sie irgendwo hinspeist. Für manche Betriebe heißt das Self-Hosting; für andere ein geprüfter Anbieter mit klarem Vertrag.

**Kalibriere die Kamera; vertrau ihr nicht blind.** Das Vision-System war nicht Plug-and-Play. Es brauchte Feinabstimmung, um einen echten Fehler von einem Schatten zu unterscheiden. Plane das ein und behalte die letzte menschliche Kontrolle bei.

**Erwarte den Hochlauf.** Der erste Monat war langsamer und unordentlicher als der zwölfte. Beurteile das Projekt nach der Lernkurve, nicht währenddessen.

**Verbinden, nicht ersetzen.** Northgate warf seine Tabellen und sein ERP nicht weg. Es flanschte KI auf das, was schon funktionierte, wie in [Kapitel 19](ch19-connecting-ai-to-systems-you-already-use.md) beschrieben. Der Betrieb behielt seine Systeme und fügte eine klügere Schicht oben drauf.

Die Lektion des kleinen Herstellers ist dieselbe wie in jedem anderen Sektor: Finde das Leck, pick das einfachste wertvolle heraus, lass die KI entwerfen und markieren, behalte einen Menschen bei der Entscheidung, und maß ehrlich. Ein Betrieb mit fünfundzwanzig Leuten und keinen Ingenieuren kann das. Die Werkzeuge sind bereit. Das Einzige, was fehlt, ist ein klarer Blick darauf, wo das Geld ausläuft.

<!-- BEGIN agentbridge-examples -->

## Teste es mit AgentBridge

So sieht dieselbe Arbeit mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die du eintippst, um es zu bekommen.

### Ein einfaches Teil entwerfen

![Ein einfaches Teil, modelliert mit dem CAD-Tool](../../assets/examples/part-design.png)
*Ein einfaches Teil, modelliert mit dem CAD-Tool*

**Was du fragst:** `Entwirf eine kleine Metallhalterung 80 mal 40 Millimeter mit vier Befestigungslöchern.`

Das Agent steuert das CAD-Tool, um das Teil mit den richtigen Maßen zu modellieren, und du bekommst eine Datei, die du prüfen oder exportieren kannst.

*Tipp: Beschreib die Form und die Maße; das Agent übernimmt die CAD-Schritte.*

---

### Prüfen, wie Teile zusammenpassen

![Eine Baugruppenprüfung zwischen zwei Teilen](../../assets/examples/assembly-check.png)
*Eine Baugruppenprüfung zwischen zwei Teilen*

**Was du fragst:** `Setze diese beiden Teile zusammen und prüfe auf Überlappungen oder Passungsprobleme.`

Das Agent fügt die Teile im CAD-Modell zusammen und zeigt, wo sie kollidieren oder wo die Passung zu eng ist.

*Tipp: Fange Passungsprobleme am Bildschirm, nicht auf der Werkbank.*

---

### Eine Zeichnung für die Werkstatt

![Eine maßhaltige technische Zeichnung für die Produktion](../../assets/examples/technical-drawing.png)
*Eine maßhaltige technische Zeichnung für die Produktion*

**Was du fragst:** `Erstelle eine technische Zeichnung der Halterung mit den wichtigsten Maßen markiert.`

Das Agent erzeugt eine Zeichnung mit markierten Maßen, bereit für die Person, die das Teil fertigen wird.

*Tipp: Frag die Ansicht, die du brauchst — Draufsicht, Seitenansicht — damit die Zeichnung klar ist.*

<!-- END agentbridge-examples -->
