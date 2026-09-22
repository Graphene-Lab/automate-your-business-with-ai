# Kapitel 33 — Ein Einzelhandelsgeschäft

*Dieses Kapitel ist eine repräsentative Zusammenstellung. Es ist kein echtes einzelnes Geschäft. Es kombiniert die gängigen Muster, die wir bei unabhängigen Einzelhändlern sehen, die KI einführen. Alle Zahlen sind illustrativ — sie zeigen die Form der Entscheidung, kein Versprechen. Ersetze sie durch deine eigenen.*

## Kontext

Stell dir ein familiengeführtes unabhängiges Geschäft vor. Wir nennen es **Cornerstone Home & Garden**. Es verkauft Werkzeuge, Farbe, Gartenbedarf und kleine Haushaltswaren. Ein physisches Ladenlokal, plus ein kleiner Online-Shop. Etwa fünfzehn Mitarbeiter. Es führt ein paar tausend verschiedene Produkte — jedes ein **SKU**, was einfach ein eigenständiger Artikel mit seinem eigenen Code bedeutet, wie „18-Volt-Bohrmaschine, Modell X" oder „5-Liter-Dispersionsfarbe grün".

Das Geschäft läuft auf einem **POS**-System — die Verkaufskasse, die jeden Verkauf aufzeichnet. Diese Kasse weiß, was wann verkauft wurde. Aber zu wissen, was verkauft wurde, ist nicht dasselbe wie zu wissen, was nächste Woche bestellt werden soll, oder was ein Kunde an der Theke fragt, oder wie man Leute zurück zur Tür bringt.

Jahrelang wurde all das nach Gefühl gemacht. Der Inhaber, Marco, bestellt nach, wenn ein Regal niedrig aussieht. Er rät, wie viel Schneeschaufel-Bestand er jeden Winter kauft, basierend auf dem letzten Winter, der diesem gar nicht glich. Kundenfragen kommen per Telefon und E-Mail und werden beantwortet, wenn jemand frei ist. Marketing ist gelegentlich ein E-Mail-Schrot, den Marco selbst tippt, an alle, mit derselben Botschaft. Das Geschäft überlebt. Aber es bindet Bargeld im falschen Bestand, verpasst Verkäufe, wenn der richtige Artikel weg ist, und gibt Marketing-Geld aus, das die Nadel kaum bewegt.

Ein kleiner unabhängiger Einzelhändler konkurriert gegen große Ketten, die ganze Teams für Prognose und Marketing haben. Cornerstone kann kein Team einstellen. Aber es kann ein paar KI-Werkzeuge auf dieselben Jobs richten.

## Das Problem

Die Lecks in einem kleinen Geschäft sind leicht zu benennen.

**Überbestand und Ausverkäufe.** Wenn Marco zu hoch rät, liegt teurer Bestand Monate im Regal. Das ist eingefrorenes Bargeld — Geld, das anderswo genutzt werden könnte, ist in Kisten gesperrt, die niemand kauft. Das nennt man **Ladenhüter**. Wenn er zu niedrig rät, geht der Artikel aus, und der Kunde geht ohne zu kaufen — oder schlimmer, kauft ihn bei einem Wettbewerber und kommt nicht wieder. Beide Fehler kosten Geld, und beide kommen vom Raten.

**Saisonale Fehlschläge.** Die Nachfrage schwankt mit der Jahreszeit und sogar dem Wetter. Ein milder Winter lässt Schneeschaufeln unverkauft. Eine plötzliche Hitzewelle leert die Gießkannen, bevor Marco nachfüllen kann. Menschliche Erinnerung an „letztes Jahr" ist ein schlechter Ratgeber für dieses Jahr.

**Langsamer Kundenservice.** Fragen wie „Haben Sie das auf Lager?" oder „Wann haben Sie geöffnet?" oder „Kann ich das zurückgeben?" stapeln sich per Telefon und E-Mail. Sie zu beantworten ist einfach, kostet aber Zeit von der Verkaufsfläche. Unbeantwortet werden sie zu verlorenen Verkäufen.

**Generisches Marketing.** Marcos E-Mail-Schrot geht an alle mit derselben Botschaft. Ein Gärtner und ein Maler bekommen dieselbe E-Mail. Meistens wird sie ignoriert. Das Marketing-Budget ist klein, aber die Rendite ist kleiner, weil es auf niemand Bestimmtes gezielt ist.

Wenn du sehen willst, wie diese vier gegen den Rest deines Geschäfts abschneiden, ist die Auswirkung/Mühe-Methode in [Kapitel 12 — Wo KI deinem Unternehmen helfen kann](ch12-where-ai-can-help-your-business.md) der Ort, sie zu bewerten.

## Die Lösung

Marco wählt die vier Lecks und beginnt mit dem, das am meisten Bargeld mit dem wenigsten Risiko freisetzt.

**Nachfrageprognose für den Bestand.** Das Geschäft verbindet seine POS-Verkaufshistorie mit einem Prognose-Werkzeug. Das Werkzeug schaut, was wann und wie schnell verkauft wurde, und fügt saisonale Muster hinzu. Dann schlägt es vor, was und wie viel zu bestellen ist, statt es Marcos Bauch zu überlassen. Es gibt die Bestellung nicht selbst auf. Es wirft einen Vorschlag auf: „Normalerweise verkaufst du das in drei Wochen durch; bestell jetzt." Ein Mensch bestätigt es. Das Raten wird eine Eingabe. (Die tiefere Behandlung von Nachfrageprognose und Warenwirtschaft ist in [Kapitel 29 — Betrieb und Produktion](ch29-operations-and-production.md).)

**Bestandswarnungen.** Oben auf der Prognose setzt das Geschäft einfache Warnungen: wenn ein Artikel unter ein sicheres Niveau fällt, markiere es; wenn ein Artikel lange nicht verkauft wurde, markiere ihn als möglichen Ladenhüter. Marco sieht beides und handelt.

**Ein Chatbot für die gängigen Fragen.** Ein Chatbot auf der Website und im Online-Shop beantwortet die wiederholten Fragen — Bestand, Öffnungszeiten, Rückgaben, Lieferung — sofort, in klarer Sprache, bei Bedarf in mehr als einer Sprache. Das Personal am Telefon wird für die Fragen frei, die eine Person brauchen. Das ist dasselbe Kundenservice-Chatbot-Muster wie in [Kapitel 27 — Kundenbetreuung und Support](ch27-customer-care-and-support.md), und dieselbe Art Einkaufsführer-Agent, die der mobilezone-Fall in [Kapitel 26 — Vertrieb und Marketing](ch26-sales-and-marketing.md) beschreibt.

**Marketing, das zielt.** Statt eines Schrots an alle hilft ein Marketing-Assistent Marco, seine Kundenliste in Gruppen zu teilen — Gärtner, Maler, Stammkunden — und für jede eine andere Botschaft zu entwerfen. Die KI schreibt die Entwürfe; Marco prüft sie gegen die Stimme des Geschäfts vor dem Senden. Dasselbe Budget erreicht die richtigen Leute mit der richtigen Botschaft.

Beachte das Muster. Die KI sagt voraus, warnt, antwortet und entwirft. Ein Mensch bestätigt die Bestellung, handhabt die harten Fragen und genehmigt das Marketing. Das Geschäft behält bei jedem Schritt die Kontrolle.

## Die Werkzeuge

Nichts davon brauchte einen Data Scientist. Die Werkzeuge sind von der Stange und auf kleine Einzelhändler ausgerichtet.

- **Ein Prognose-Add-on** für das POS- oder Warenwirtschaftssystem. Viele moderne Kassensysteme enthalten jetzt eine „Bestellvorschlag"-Funktion, die deine eigene Verkaufshistorie liest.
- **Einfache Bestandswarnungen**, oft in dasselbe Warenwirtschaftswerkzeug eingebaut.
- **Ein Kundenservice-Chatbot** auf der Website, verbunden mit der Produktliste des Geschäfts, damit er „haben Sie das?" genau beantworten kann.
- **Ein Marketing-Assistent**, der die Kundenliste segmentiert und Kampagnen-E-Mails und Social-Posts entwirft.

Wie man unter diesen auswählt, ohne sich von einer glänzenden Demo täuschen zu lassen, ist in [Kapitel 17 — Werkzeuge wählen, ohne sich täuschen zu lassen](ch17-choosing-tools-without-being-fooled.md) behandelt. Wie man sie an das POS und die Kundenliste anschließt, die du bereits hast, ist in [Kapitel 19 — KI an Systeme anschließen, die du bereits nutzt](ch19-connecting-ai-to-systems-you-already-use.md).

Eine Warnung speziell für den Einzelhandel: Die Kundenliste hält personenbezogene Daten — Namen, E-Mails, Kaufhistorie. Die Privatsphäre-Regeln in [Kapitel 10 — Privatsphäre und DSGVO](ch10-privacy-and-gdpr.md) gelten dafür, wie diese Liste fürs Marketing genutzt wird, einschließlich das Einholen von Einwilligung, um Leute anzuschreiben.

## Die Kosten

Hier ist ein illustratives Erstjahres-Budget für ein Geschäft wie Cornerstone. Das sind erfundene Zahlen, um die Form zu zeigen. Nutze deine eigenen.

**Direkte Kosten.**
- Prognose- und Warenwirtschaft-Add-on: etwa 4.800 Euro pro Jahr.
- Kundenservice-Chatbot: etwa 3.600 Euro pro Jahr.
- Marketing-Assistent: etwa 3.600 Euro pro Jahr.
- Einrichtung und Integration mit dem POS und der Kundenliste: etwa 7.000 Euro einmalig.
- Schulung des Personals: etwa 2.000 Euro einmalig.

Erstjahr gesamt: rund **21.000 Euro**. In stabilen Jahren danach kommen die wiederkehrenden Abonnements auf etwa **12.000 Euro**.

**Indirekte Kosten.**
- Personalzeit, um die Bestellvorschläge und die Antworten des Chatbots zu prüfen.
- Das Lern-Tal, während alle dem neuen System vertrauen.
- Jemand muss die Marketing-Entwürfe vor dem Senden prüfen, damit die Stimme des Geschäfts richtig bleibt.
- Die Verkaufshistorie aufräumen, damit die Prognose gute Daten zum Lernen hat.

Die vollständige Methode, diese Kosten zu zählen und die Einsparungen in eine Rendite-Zahl zu verwandeln, ist in [Kapitel 16 — Ziele, Kosten und Return on Investment](ch16-goals-costs-and-return-on-investment.md). Rechne die Mathematik nicht im Kopf. Schreib sie auf.

## Die Ergebnisse

Nach einem Jahr, gemessen an einer Basislinie, die Marco vor dem Start aufzeichnete, sieht das illustrative Ergebnis so aus. Deine Zahlen werden abweichen. Diese zeigen, wie eine gute Passform aussehen kann.

- **Ausverkäufe sanken.** Weniger Kunden gingen mit leeren Händen, weil die Prognose die Nachbestellung früh markierte.
- **Ladenhüter sanken.** Weniger Bargeld lag eingefroren in Kisten, die niemand wollte, weil das Werkzeug die Langsam-Dreher und die Überbestellung sah, bevor es geschah.
- **Bargeld wurde freigesetzt.** Mit weniger Geld im falschen Bestand gesperrt, hatte das Geschäft Bargeld für anderes.
- **Kundenfragen sofort beantwortet.** Der Chatbot bewältigte die gängigen bei Tag und Nacht, und die Telefon-Warteschlange wurde kürzer.
- **Marketing arbeitete härter.** Segmentierte, gezielte Botschaften bekamen mehr Antwort als der alte Einer-pass-für-alle-Schrot, auf demselben kleinen Budget.

Die ehrliche Einschränkung: Nichts davon war sofort. Die Prognose war in den ersten Monaten grob, weil sie ein sauberes Jahr Verkaufshistorie zum Lernen brauchte. Der Chatbot gab anfangs falsche Antworten, bis er mit genauen Produktdaten gefüttert wurde. Die Gewinne fuhren über Wochen hoch, wie die Lernkurven-Warnung in [Kapitel 16](ch16-goals-costs-and-return-on-investment.md) vorhersagt. Marco maß die echten Zahlen nach der Hochfahrt, nicht während ihr.

## Gelernte Lektionen

**Die Prognose ist nur so gut wie deine Verkaufshistorie.** Ein Prognose-Werkzeug lernt aus deinen vergangenen Verkäufen. Wenn die Historie chaotisch oder unvollständig ist, ist die Prognose schwach. Die Daten zuerst aufzuräumen war das Wertvollste, was Marco tat. Daten-Bereitschaft ist in [Kapitel 14 — Daten: Der Rohstoff](ch14-data-the-raw-material.md) behandelt.

**Fang beim Bargeld an.** Von den vier Lecks war der Bestand das wirkungsvollste, weil Ladenhüter echtes Geld bindet. Es war auch risikoarm, weil ein Mensch jede Bestellung bestätigt. Das machte es zum idealen ersten Projekt — die „hohe Auswirkung, hohe ease zuerst"-Regel aus [Kapitel 12](ch12-where-ai-can-help-your-business.md).

**Lass die KI nie allein bestellen.** Ein Bestellvorschlag ist sicher. Ein automatischer Bestellauftrag ohne Menschen und ohne Ausgabengrenze ist es nicht. Ein Glitch oder eine schlechte Prognose kann tausende Einheiten bestellen, die niemand will. Behalte einen Menschen und eine Obergrenze bei jeder Bestellung.

**Der Chatbot braucht gute Produktdaten.** Er kann „haben Sie das?" nur beantworten, wenn die Bestandliste, die er liest, genau ist. Ein Chatbot, mit falschen Daten gefüttert, gibt selbstbewusste falsche Antworten und nervt Kunden.

**Marketing-KI entwirft; du behältst die Stimme.** Der Assistent schreibt schnell, aber er kennt den Ton deines Geschäfts nicht. Lies jeden Entwurf, bevor er hinausgeht. Und achte die Einwilligung — schreib nur Leute an, die zugestimmt haben, angeschrieben zu werden, wie [Kapitel 10](ch10-privacy-and-gdpr.md) es verlangt.

**Ein Modell bricht an einer Überraschung.** Prognose lernt aus der Vergangenheit. Ein Jahrtausende-Ereignis — ein Sturm, ein plötzlicher Engpass — bricht das Muster. Das Werkzeug wird es nicht kommen sehen. Bleib bereit, es mit deinen eigenen Augen zu überstimmen.

**Miss ehrlich und erwarte die Hochfahrt.** Zeichne die Basislinie auf, bevor du anfängst. Beurteile das Projekt nach der Lernkurve, nicht während ihr.

Die Lektion des kleinen Einzelhändlers ist dieselbe wie die jedes anderen Sektors: Finde das Leck, wähle das einfachste wertvolle — meist der Bestand, der Bargeld bindet — lass KI vorhersagen und entwerfen, behalte einen Menschen bei der Bestellung und der Botschaft, und miss ehrlich. Ein fünfzehn-Personen-Unabhängigkeitsgeschäft kann das. Die Werkzeuge sind bereit. Das Einzige, was fehlt, ist ein klarer Blick darauf, wo das Bargeld feststeckt.

<!-- BEGIN agentbridge-examples -->

## Teste es mit AgentBridge

So sieht dieselbe Aufgabe mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die du eingibst, um es zu bekommen.

### Wo soll ich als Nächstes eröffnen?

![Zwei Kandidaten-Standorte auf einer Karte](../../assets/examples/location-analysis.png)
*Zwei Kandidaten-Standorte auf einer Karte*

**Was du fragst:** `Zeige diese zwei Kandidaten-Ladenstandorte auf einer Karte und vermerke, was in der Nähe jedes einzelnen ist.`

Der Agent kartiert beide Orte und vermerkt nahe Merkmale — Fußgängeraufkommen, Wettbewerber, Parkplätze — um dir beim Abwägen der Wahl zu helfen.

*Tipp: Kombiniere das mit einem Web-Recherche-Schritt über die Nachbarschaft für ein vollständigeres Bild.*

<!-- END agentbridge-examples -->
