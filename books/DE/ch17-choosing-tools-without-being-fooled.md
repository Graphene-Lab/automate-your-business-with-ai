# Kapitel 17 — Werkzeuge wählen, ohne sich täuschen zu lassen

## In einfachen Worten

Jeder KI-Anbieter wird dir sagen, sein Werkzeug sei einfach, billig und revolutionär. Manche davon sagen die Wahrheit. Viele nicht. Dieses Kapitel ist deine Abwehr. Es bringt dir bei, über die glänzende Demo und den selbstbewussten Verkäufer hinwegzusehen und ein Werkzeug zu wählen, das wirklich zu deinem Unternehmen passt.

Die wichtigste Idee hier ist einfach: **Du kaufst kein Werkzeug, du kaufst ein Ergebnis.** Ein Werkzeug ist nur so viel wert, wie es für dich tut. Ein schönes Produkt, das dein Problem nicht löst, ist ein teures Spielzeug. Deine Aufgabe ist es, jede Wahl zurück zu einem echten Problem und einer echten Zahl zu verbinden.

Ein gutes Bild ist ein Autokauf. Das Autohaus lässt jedes Auto großartig aussehen. Das Leder glänzt, der Motor schnurrt, der Verkäufer ist charmant. Aber du kaufst ein Auto nicht für das Autohaus. Du kaufst es für die Straße, die du tatsächlich fährst, die Passagiere, die du tatsächlich beförderst, und den Kraftstoff, den du dir leisten kannst. Also stellst du harte Fragen, machst eine Probefahrt auf *deinen* Straßen, und liest die laufenden Kosten. KI-Werkzeuge wählen ist dieselbe Disziplin.

Dieses Kapitel behandelt, wie du zwischen fertiger Software, etwas Eigengebautem oder Selbstmachen wählst. Es gibt dir die genauen Fragen, die du einem Anbieter stellen musst. Es zeigt dir, wo versteckte Kosten lauern. Es erklärt, warum eine Demo nicht reicht und wie du stattdessen einen kleinen Piloten fährst. Und es schaut Open-Source-Werkzeuge an — Software, deren Code frei zu nutzen und zu ändern ist — als echte, erschwingliche Option.

Eine Regel, die du bei dir tragen sollst: **werde langsam.** Der Verkäufer will Dringlichkeit. „Dieser Preis endet Freitag." „Nur noch zwei Lizenzen." Dringlichkeit ist ein Trick, um dich am Denken zu hindern. Ein gutes Werkzeug überlebt eine Woche sorgfältigen Nachdenkens. Ein schlechtes verlässt sich darauf, dass du nicht denkst. Nimm dir die Woche.

## Ein bisschen Geschichte

**1960er–1970er: Software ist maßgeschneidert.** In den frühen Tagen ließ eine Firma, die Software wollte, Spezialisten sie von Grund auf schreiben. Es gab keine „von der Stange"-Option. Software war ein Maßanzug, auf Maß gefertigt, teuer und langsam in der Lieferung.

**1980er: die Revolution der Paketsoftware.** Produkte wie Tabellenkalkulation und Textverarbeitung kamen in einer Schachtel. Zum ersten Mal konnte ein Unternehmen ein allgemeines Werkzeug kaufen und es an viele Aufgaben anpassen. Das war billiger und schneller als Eigenbauten. Der moderne Softwaremarkt wurde geboren.

**1990er–2000er: große Suiten und die Lock-in-Falle.** Große Anbieter verkaufen riesige integrierte Suiten — ein Produkt für alles. Sie funktionierten gut, aber der Wechsel weg war schmerzhaft und teuer. Firmen entdeckten, dass die leichte Wahl von heute morgen ein teures Gefängnis werden konnte. Das Wort **Vendor Lock-in** — bei einem Lieferanten festhängen, weil Gehen zu schwer ist — zog in den Geschäfts-Wortschatz ein. (Lock-in wird vollständig in [Kapitel 9](ch09-third-party-services-and-shadow-ai.md) behandelt.)

**2000er: Open-Source wird Mainstream.** Linux, Apache und später Tausende freier Projekte bewiesen, dass Software von Gemeinschaften gebaut und verschenkt werden kann und trotzdem die größten Websites der Welt antreibt. Open-Source hörte auf, ein Hobby zu sein, und wurde eine ernsthafte, vertrauenswürdige Option.

**2010er: das Abo-Zeitalter.** Software wechselte von „einmal kaufen" zu „jeden Monat zahlen". Das senkte den Einstiegspreis, fügte aber eine neue Art nie endender Kosten hinzu. Abos machten es leicht zu starten und leicht, den Überblick zu verlieren, wofür man bezahlte.

**2020er: der KI-Goldrausch.** Hunderte KI-Werkzeuge tauchten fast über Nacht auf, viele mit großer Finanzierung und noch größeren Versprechen. Die Lücke zwischen dem, was eine Demo zeigt, und dem, was ein Werkzeug in echter Arbeit liefert, war nie größer. Gut zu wählen ist heute eine Kern-Geschäftsfähigkeit, kein nettes Extra.

Der Bogen: von maßgeschneidert, zu verpackt, zu abonniert, zu überflutet. Die Werkzeuge ändern sich weiter. Die Notwendigkeit, sorgfältig zu wählen, nie.

## Neugier

### 17.6 Das Buch „Headcount Zero" — eine Firma ohne Angestellte

Wie weit kann die Idee „keine Menschen nötig" gehen? Es gibt ein Buch, das sie ins Extrem treibt. Es heißt **„Headcount Zero: How to Build an AI-Run Company with Paperclip"**, von **Anthony David Adams**. Es ist als Open-Source-Buch auf GitHub veröffentlicht (das Repository `AnthonyDavidAdams/zero-employee-company-book`), sodass jeder es kostenlos lesen kann.

Die Frage, die das Buch stellt, ist: *Was, wenn du nie jemanden einstellen müsstest?* Statt Angestellten führt der Gründer eine Firma aus **KI-Agenten** — Programmen, die Aufgaben allein ausführen können. Der Gründer wird eine Art Manager eines Organigramms voller KI-Arbeiter, koordiniert von einer Open-Source-Plattform, die das Buch **Paperclip** nennt.

Das ist kein Plan, den die meisten kleinen Unternehmen morgen befolgen sollten. Eine Firma mit buchstäblich null Menschen ist ein extremes Gedankenexperiment, und es hat offensichtliche Grenzen: Wer ist verantwortlich, wenn etwas schiefgeht? Wer trägt die rechtliche Verantwortung? Wer versteht das unausgesprochene Bedürfnis eines Kunden? (Das sind genau die menschlichen Rollen, die in [Kapitel 15](ch15-people-roles-and-culture.md) besprochen werden.)

Aber als Linse ist „Headcount Zero" nützlich. Es erzwingt eine ehrliche Frage: **Wie viel deiner Arbeit ist wirklich menschlich, und wie viel ist Routine, die eine Maschine tragen könnte?** Die meisten Firmen finden, dass ein überraschender Anteil der täglichen Aufgaben Routine ist. Das heißt nicht, alle zu entlassen. Es heißt, Menschen von den langweiligen Teilen zu befreien, damit sie das Urteilsvermögen, die Beziehungen und die kreative Arbeit tun können, die Maschinen nicht können. Lies das Buch als Provokation, nicht als Anleitung. Es zeigt dir den Rand des Möglichen, und am Rand wohnen die interessanten Fragen.

## Ein echtes Geschäftsbeispiel

*Das Folgende ist ein illustratives Composite häufiger realer Muster, keine einzelne genannte Firma.*

Eine kleine Steuerberatungsfirma wollte „mit KI automatisieren". Ein Anbieter gab eine schillernde Demo: Das Werkzeug las einen Stapel Quittungen und erzeugte in Sekunden eine saubere Zusammenfassung. Der Inhaber unterschrieb auf der Stelle, geblendet, einen Zweijahresvertrag.

Sechs Monate später sah die Realität anders aus. Die Demo hatte ein paar saubere, perfekte Quittungen benutzt. Die echten Quittungen der Firma waren zerknüllt, verschwommen, in drei Sprachen und voller Randfälle. Das Werkzeug lag oft genug falsch, dass das Mitarbeiter alles nachprüfen mussten, was bedeutete, dass die „Ersparnis" winzig war. Der Zweijahresvertrag hielt sie gefangen. Das Abo rechnete weiter ab. Das Werkzeug wurde ein teures Zierstück.

Eine zweite Firma wählte anders. Bevor sie irgendetwas unterschrieb, bat sie den Anbieter um einen **Test mit ihren eigenen chaotischen Daten**, nicht mit dem sauberen Demo-Set des Anbieters. Sie fuhr einen zweiwöchigen Piloten mit echten Quittungen. Das Werkzeug bewältigte etwa 70 % gut und scheiterte am Rest. Diese Zahl — 70 % — erlaubte der Firma eine klare Entscheidung: das Werkzeug für die leichte 70 % behalten, Menschen bei der schweren 30 % behalten, und nur einen Einjahresvertrag mit klarem Ausstieg unterschreiben. Dasselbe Werkzeug, mit Disziplin statt Blendung gewählt, wurde eine echte Hilfe.

Der Unterschied war nicht die Software. Er war, dass die zweite Firma sich nicht von einer Demo täuschen ließ und zuerst mit ihrer eigenen Realität testete.

## Wie man es macht

### 17.1 Fertige Software, maßgeschneidert oder selbst gemacht

Wenn du ein Werkzeug brauchst, hast du drei breite Wege. Jeder hat seinen Platz.

**Fertig (von der Stange kaufen).** Das ist Software, die du abonnierst oder wie sie ist kaufst, wie ein Chatbot-Dienst oder eine App zum Zusammenfassen von Dokumenten. Es ist der schnellste und normalerweise billigste Weg zu starten. Du bekommst sie heute, sie funktioniert out of the box, und jemand anderes wartet sie. Der Kompromiss: Sie tut, wofür *sie* gebaut wurde, nicht genau das, was *du* wolltest. Wenn dein Bedarf üblich ist, ist ein Fertiges-von-der-Stange-Werkzeug fast immer die richtige erste Wahl.

**Maßgeschneidert (jemanden fürs Bauen bezahlen).** Ein Entwickler schreibt Software nur für dich. Das passt perfekt zu deinen Bedürfnissen. Aber es ist langsam, teuer, und du besitzt jetzt etwas, das für immer Wartung braucht. Eigenbauten ergeben nur Sinn, wenn dein Bedarf speziell ist und kein fertiges Werkzeug ihn abdeckt — und wenn der Wert hoch genug ist, um die Kosten zu rechtfertigen. Für die meisten kleinen Unternehmen ist Maßgeschneidert selten der erste Zug.

**Selbst machen (du baust es, mit No-Code- oder leichten Werkzeugen).** Werkzeuge wie Automatisierungs-Apps lassen dich Dienste selbst verbinden, ohne Code zu schreiben. Das ist billig und flexibel, und du lernst viel. Der Kompromiss: Es kostet deine Zeit, und wenn du gehst, kann das, was du gebaut hast, für jemand anderen schwer zu warten sein. Selbst machen ist großartig für kleine Automatisierungen, die du besitzen und einfach halten kannst.

Eine einfache Faustregel: **Starte fertig von der Stange. Geh zu Selbst-machen für kleine Kleinarbeit zwischen Werkzeugen. Geh nur zu maßgeschneidert, wenn sonst nichts passt und der Gewinn groß ist.** Die meisten Firmen leben glücklich mit den ersten beiden.

### 17.2 Fragen an den Anbieter

Nimm niemals das Wort eines Anbieters hin. Stelle direkte Fragen und höre die Antworten genau an — besonders das, was sie umgehen. Halte diese bereit:

- **Was genau tut dieses, und was tut es NICHT?** Zwing sie über das Marketing hinaus. Ein selbstbewusstes „es handhabt alles" ist ein Warnsignal.
- **Wie sieht es aus, wenn es versagt?** Jedes Werkzeug versagt irgendwo. Ein ehrlicher Anbieter kann seine Schwachstellen benennen. Ein Anbieter, der sagt „es versagt nie", lügt oder ahnt nichts.
- **Was sind die Gesamtkosten über drei Jahre, nicht nur im ersten Monat?** Lass sie die volle Zahl laut sagen.
- **Was passiert mit meinen Daten?** Wo werden sie gespeichert, wer kann sie sehen, und trainiert ihr eure KI damit? (Das ist wichtig für den Datenschutz — siehe [Kapitel 10](ch10-privacy-and-gdpr.md).)
- **Kann ich meine Daten herausbekommen, und in welchem Format?** Das ist dein Ausstieg. Wenn du nicht sauber gehen kannst, bist du eingesperrt.
- **Welchen Support bekomme ich, und wie schnell?** Reaktionszeiten, Kanäle, und ob Support enthalten ist oder extra kostet.
- **Wer sonst nutzt das in meiner Branche, und kann ich mit ihnen sprechen?** Eine echte Referenz ist zehn Demos wert.
- **Was ist eure Roadmap, und wie stabil ist die Firma?** Ein Werkzeug aus einer wackeligen Start-up kann verschwinden. Frag, wie lange sie im Geschäft sind und wer sie finanziert.
- **Was ist der Vertrag, und wie kündige ich?** Lies die Ausstiegsbedingungen, bevor du unterschreibst, nicht danach.

Schreibe die Antworten auf. Vergleiche Anbieter anhand derselben Fragen. Der Anbieter, der klar und ehrlich antwortet, hebt sich von dem ab, der wedelt und charmant tut.

### 17.3 Versteckte Kosten und Abos

Der Aufkleberpreis ist die kleinste Kosten. Die echten Kosten verstecken sich an Orten, wohin die meisten nie schauen. (Die volle Kostenmethode lebt in [Kapitel 16](ch16-goals-costs-and-return-on-investment.md); hier ist die anbieterspezifische Version.)

Achte auf diese:

- **Preis pro Platz.** Viele Werkzeuge berechnen pro Nutzer. Ein „billiges" Werkzeug wird teuer, wenn du dein ganzes Team hinzufügst. Zähle die Plätze, bevor du unterschreibst.
- **Nutzungsabhängige Gebühren.** Manche KI-Werkzeuge berechnen pro Aufgabe, pro Nachricht oder pro Dokument. Ein belebter Monat kann eine Überraschungsrechnung erzeugen. Frag genau, wie die Nutzung bemessen wird.
- **Einrichtungs- und Onboarding-Gebühren.** Der Start kann extra kosten, manchmal mehr als das erste Abojahr.
- **Integrationskosten.** Das Werkzeug mit deinen bestehenden Systemen zu verbinden, kann bezahlte Hilfe brauchen.
- **Premium-Funktionen hinter einer Bezahlschranke.** Die Funktion, die dir den Verkauf abgerungen hat, liegt vielleicht auf einer höheren Stufe. Prüfe, welche Stufe du wirklich brauchst.
- **Schulung und Support als Zusatz.** „Support enthalten" bedeutet oft einen Hilfeartikel, keine Person. Echte Hilfe kann mehr kosten.
- **Das nie endende Abo.** Eine Monatsgebühr sieht klein aus, hört aber nie auf. Multipliziere sie mit drei oder fünf Jahren, um das wahre Gewicht zu sehen.
- **Ausstiegs- und Wechselkosten.** Zu kündigen kann schwer sein, und deine Daten woandershin zu bewegen kann bezahlte Arbeit brauchen.

Bevor du unterschreibst, baue eine **Dreijahres-Gesamtkostenzahl** für jede Option. Addiere jede einzelne davon. Die Monatspreis des Anbieters ist oft nur ein Drittel der echten Dreijahreszahl.

### 17.4 Demos und Pilotprojekte

Eine Demo ist eine Vorführung. Sie zeigt das Werkzeug von seiner besten Seite, auf Daten, die ausgewählt sind, um dich zu gewinnen. Entscheide nie allein nach einer Demo.

Ein **Pilotprojekt** ist die ehrliche Alternative. Ein Pilot ist ein kleiner, zeitlich begrenzter Test des Werkzeugs auf *deiner* echten Arbeit, mit *deinen* echten chaotischen Daten, der ein *dein* echtes Ergebnis misst. Wo eine Demo dir eine Highlight-Reel zeigt, zeigt ein Pilot dir die Wahrheit.

So fährst du einen guten Piloten:

- **Nutze deine eigenen Daten, inklusive der chaotischen Fälle.** Akzeptiere nicht die saubere Stichprobe des Anbieters.
- **Halte es klein und kurz.** Zwei bis vier Wochen an einem Prozess reichen, um viel zu lernen.
- **Definiere den Erfolg, bevor du startest.** Welche Zahl muss das Werkzeug erreichen, um als Bestehen zu zählen? (Das verbindet zur Pilotmethode in [Kapitel 18](ch18-your-first-pilot-project.md).)
- **Teste das Versagen, nicht nur den Erfolg.** Stoße es absichtlich mit harten Fällen an.
- **Teste den Support.** Sende während des Piloten eine Support-Anfrage und sieh, wie schnell und hilfreich sie sind.
- **Teste den Ausstieg.** Versuche, deine Daten zu exportieren. Stelle sicher, dass du gehen kannst.

Ein Anbieter, der einen echten Piloten mit deinen Daten ablehnt, sagt dir etwas. Ein Anbieter, der ihn willkommen heißt, ist aus gutem Grund zuversichtlich.

### 17.5 Open-Source-Werkzeuge: eine erschwingliche und flexible Alternative

**Open-Source** bedeutet, dass der Quellcode der Software — die Anweisungen, die sie zum Laufen bringen — für jeden frei einzusehen, zu nutzen und zu ändern ist. Du „piratest" sie nicht; Open-Source ist eine legale, übliche und oft ausgezeichnete Art, wie Software gemacht wird. Das Web, das du gerade nutzt, läuft wahrscheinlich auf Open-Source-Software.

Warum es für KI in Betracht ziehen:

- **Niedrige oder keine Lizenzkosten.** Viele Open-Source-Werkzeuge sind frei zu nutzen.
- **Kein Lock-in.** Weil du den Code sehen und ändern kannst, bist du nicht bei einem Anbieter gefangen.
- **Du kannst es selbst betreiben.** Open-Source-KI-Modelle können auf deinen eigenen Maschinen laufen, was deine Daten unter deiner Kontrolle hält (das ist **Selbst-Hosting**, behandelt in [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md)).
- **Eine Gemeinschaft dahinter.** Beliebte Projekte verbessern sich schnell und haben viele Nutzer, von denen man lernen kann.

Die Kompromisse:

- **Du brauchst vielleicht mehr Können für die Einrichtung.** Open-Source setzt oft voraus, dass du Dinge konfigurieren kannst, oder jemanden einstellen kannst, der das kann.
- **Support ist gemeinschaftsbasiert.** Es gibt vielleicht niemanden zum Anrufen. Du verlässt dich auf Dokumentation und Foren.
- **Du trägst die Wartung.** Wenn du es selbst betreibst, liegt es an dir, es aktuell und sicher zu halten.

Die ehrliche Balance: Open-Source ist ein mächtiger, erschwinglicher Weg, besonders wenn Datenkontrolle zählt. Aber er tauscht Geld gegen Aufwand und Können. Wenn du keines von beiden hast, ist ein bezahltes Fertiges-von-der-Stange-Werkzeug vielleicht der klügere Start. Wenn du ein bisschen technische Hilfe hast, kann Open-Source dir eine Menge sparen und dich vom Lock-in befreien.

## Ethik und Verantwortung

Werkzeuge zu wählen ist nicht ethisch neutral. Deine Wahlen beeinflussen deine Kunden, deine Mitarbeiter und deine Daten.

**Schütze die Daten deiner Kunden schon in der Wahl selbst.** Bevor ein Werkzeug Kundendaten berührt, wisse, wohin es geht und wer es sehen kann. Ein Werkzeug, das seine KI mit den privaten Informationen deiner Kunden ohne Zustimmung trainiert, kann gegen das Gesetz verstoßen (siehe [Kapitel 10](ch10-privacy-and-gdpr.md)).

**Lass den Hype eines Anbieters keine Entscheidung treiben, die Menschen betrifft.** Wenn ein Werkzeug die Jobs deiner Mitarbeiter verändern wird, wähle es aus ehrlichen Gründen und binde deine Leute ein, nicht weil ein Verkäufer falsche Dringlichkeit erzeugt hat.

**Gib Werkzeugen den Vorzug, die du prüfen und verlassen kannst.** Ein Werkzeug, das verbirgt, wie es funktioniert, oder deine Daten fängt, ist eine schlechte ethische Wahl sowie eine schlechte geschäftliche. Transparenz und ein sauberer Ausstieg sind Zeichen eines Anbieters, der dich respektiert.

**Sei ehrlich in deinen eigenen Behauptungen.** Wenn du ein KI-Werkzeug kaufst und Kunden sagst „unser Dienst nutzt KI", stelle sicher, dass das wahr und keine übertriebene Werbung ist.

**Bedenke die Ethik des Anbieters selbst.** Wo leben ihre Daten? Respektieren sie Datenschutzgesetze? Sind sie stabil und ehrlich? Du gehst eine Partnerschaft mit ihnen ein; wähle einen Partner, dem du deinen Namen anvertrauen würdest.

Ein Werkzeug ist eine Beziehung. Wähle den Partner so sorgfältig, wie du einen Geschäftspartner wählen würdest.

## Zu vermeidende Fehler

### 17.7 Häufige Fehler

**Nach der Demo kaufen.** Nach einer polierten Vorführung auf sauberen Daten entscheiden. Immer mit der eigenen chaotischen Realität pilotieren.

**Die Dreijahreskosten ignorieren.** Auf den Monatspreis schauen und nicht auf die Summe. Das Abo hört nie auf.

**Auf Dringlichkeit hereinfallen.** „Der Preis endet Freitag" ist ein Verkaufstrick. Ein gutes Werkzeug überlebt eine Woche des Nachdenkens.

**Kein Ausstiegsplan.** Unterschreiben, ohne zu prüfen, wie man die Daten herausbekommt. So entsteht Lock-in.

**Kaufen, bevor das Problem definiert ist.** Ein Werkzeug holen und dann nach einer Nutzung suchen. Definiere zuerst das Problem, dann finde das Werkzeug.

**Beliebtheit mit Passgenauigkeit verwechseln.** Ein Werkzeug, das Tausende nutzen, passt vielleicht trotzdem nicht in *deinen* Arbeitsablauf.

**Den Support-Test überspringen.** Nicht prüfen, wie sich der Anbieter nach dem Verkauf verhält. Teste den Support während des Piloten.

**Zu früh zu viel maßschneidern.** Für einen Eigenbau zahlen, wenn ein Fertiges-von-der-Stange-Werkzeug 80 % des Bedarfs decken würde.

**Die DIY-Wartung unterschätzen.** Es selbst bauen und vergessen, dass man es jetzt am Leben erhalten muss.

**„Es handhabt alles" vertrauen.** Kein Werkzeug tut das. Ein Anbieter, der das behauptet, sagt dir nicht die Wahrheit.

**Den Vertrag nicht lesen.** Unterschreiben, ohne die Kündigungs- und Datenbedingungen zu lesen. Vorher lesen, nicht nachher.

**Den billigsten Aufkleber wählen.** Der niedrigste Monatspreis kann die höchste Gesamtkosten verstecken.

## Praktische Übung

### 17.8 Übung: eine Bewertungsraster

Baue ein einfaches Bewertungsraster, um Werkzeuge nebeneinander zu vergleichen. Das verwandelt eine verschwommene Wahl in eine klare.

**Schritt 1 — Liste deine Optionen.** Schreibe zwei oder drei Kandidaten-Werkzeuge auf (oder Wege: fertig von der Stange, selbst gemacht, Open-Source).

**Schritt 2 — Liste die Kriterien.** Nutze diese, oder füge deine eigenen hinzu:

- Passt zu meinem echten Problem (0–5)
- Handhabt meine chaotischen Daten gut (0–5)
- Dreijahres-Gesamtkosten (niedriger ist besser — bewerte es)
- Bedienbarkeit für meine Mitarbeiter (0–5)
- Datenschutz und Kontrolle (0–5)
- Leichtigkeit des Ausstiegs / kein Lock-in (0–5)
- Support-Qualität (0–5)
- Anbieter-Stabilität (0–5)

**Schritt 3 — Bewerte jedes Werkzeug.** Gib eine Zahl für jedes Kriterium. Sei ehrlich, nicht hoffnungsvoll.

**Schritt 4 — Gewichte, was am meisten zählt.** Wenn Datenschutz für dich kritisch ist, verdopple sein Gewicht. Wenn Kosten am meisten zählen, gewichte es höher.

**Schritt 5 — Addiere es.** Das Werkzeug mit der höchsten gewichteten Punktzahl ist dein Favorit.

**Schritt 6 — Teste den Favoriten mit einem Piloten.** Das Raster lichtet das Feld; der Pilot bestätigt es. Überspringe den Piloten nicht.

Setze das Raster auf eine Seite. Es macht die Entscheidung sichtbar und verteidigbar, und es hindert einen charmanten Verkäufer daran, dein Urteilsvermögen mit Charme zu überstimmen.

## Checkliste

### 17.9 Checkliste zur Bewertung eines Anbieters

Bevor du mit einem KI-Anbieter unterschreibst, hake jede Box ab.

- [ ] **Ich kann das genaue Problem benennen, das dieses Werkzeug für mich löst.**
- [ ] **Ich weiß, was das Werkzeug NICHT tut, und wo es versagt.**
- [ ] **Ich habe Dreijahres-Gesamtkosten, nicht nur den Monatspreis.**
- [ ] **Ich weiß, wie die Preisbildung funktioniert** — pro Platz, pro Nutzung, Stufen, Einrichtungsgebühren.
- [ ] **Ich weiß, wo meine Daten gespeichert sind und wer sie sehen kann.**
- [ ] **Ich weiß, ob der Anbieter seine KI mit meinen Daten trainiert, und ich stimme zu oder lehne ab.**
- [ ] **Ich habe das Werkzeug mit meinen eigenen chaotischen Daten getestet, nicht mit dem Demo-Set des Anbieters.**
- [ ] **Ich habe einen kleinen Piloten mit einer definierten Erfolgszahl gefahren.**
- [ ] **Ich habe den Support des Anbieters während des Tests getestet.**
- [ ] **Ich habe den Export meiner Daten aus dem Werkzeug getestet.**
- [ ] **Ich habe die Kündigungsbedingungen vor dem Unterschreiben gelesen.**
- [ ] **Ich habe eine Referenz aus einem anderen Unternehmen meiner Branche, oder habe versucht, eine zu bekommen.**
- [ ] **Ich habe die Stabilität des Anbieters geprüft und wie lange sie im Geschäft sind.**
- [ ] **Ich habe mich der Dringlichkeit widersetzt und mir Zeit zum Nachdenken genommen.**
- [ ] **Ich habe mindestens zwei Optionen nach denselben Kriterien verglichen.**

Wenn eine Box leer ist, hast du die Bewertung nicht abgeschlossen. Fülle sie, bevor du unterschreibst. Ein Werkzeug mit klarem Kopf gewählt, ist weit mehr wert als eines in Blendung gekauft.

## Wichtige Kernpunkte

- Du kaufst kein Werkzeug, du kaufst ein Ergebnis — verbinde jede Wahl zurück zu einem echten Problem und einer echten Zahl.
- Eine Demo ist eine Vorführung auf sauberen Daten; ein Pilot mit deinen eigenen chaotischen Daten ist der einzige ehrliche Test.
- Der Monatspreis ist nur ein Bruchteil der Kosten — baue immer eine Dreijahres-Gesamtsumme, die Plätze, Nutzung, Einrichtung, Support und Ausstieg einschließt.
- Open-Source ist ein echter, erschwinglicher, lock-in-freier Weg, aber er tauscht Geld gegen Aufwand und Können; wähle ihn, wenn du die Hilfe hast, ihn zu betreiben.
- Weise Dringlichkeit zurück: ein gutes Werkzeug überlebt eine Woche sorgfältigen Nachdenkens, und ein Anbieter, der einen echten Piloten willkommen heißt, ist aus gutem Grund zuversichtlich.

<!-- BEGIN agentbridge-examples -->

## Teste es mit AgentBridge

So sieht dieselbe Aufgabe mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die du eingibst, um es zu bekommen.

### Produkte vor dem Kauf vergleichen

![Ein Produktvergleich nebeneinander](../../assets/examples/product-compare.png)
*Ein Produktvergleich nebeneinander*

**Was du fragst:** `Vergleiche diese zwei Drucker für ein kleines Büro: Preis, laufende Kosten und Zuverlässigkeit.`

Der Agent recherchiert beide Produkte und legt einen klaren Vergleich dar, damit du die bessere Passung für dein Budget und deinen Einsatz wählst.

*Tipp: Frag nach den Gesamtbetriebskosten, nicht nur nach dem Aufkleberpreis.*

<!-- END agentbridge-examples -->
