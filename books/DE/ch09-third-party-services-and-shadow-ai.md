# Kapitel 9 — Dienste von Drittanbietern und Shadow-KI

## In einfachen Worten

Ein KI-Dienst eines Drittanbieters ist jede KI, die Sie nutzen und die auf den Computern von jemand anderem läuft. Sie tippen eine Frage ein oder laden eine Datei hoch. Sie reist über das Internet zu deren Rechnern. Deren Software macht die Arbeit. Die Antwort kommt zurück. Das Innere sehen Sie nie.

So benutzen die meisten Firmen heute KI. Es ist einfach, der Einstieg ist billig, und es ist leistungsstark. Deshalb nutzt es fast jeder.

Es hat auch einen versteckten Preis. In dem Moment, in dem Ihr Text Ihr Gebäude verlässt, verlieren Sie die direkte Kontrolle darüber. Sie sind jetzt abhängig von einer Firma, die Sie nicht entworfen haben, von Regeln, die Sie nicht geschrieben haben, von einem Server, den Sie nicht prüfen können.

„Shadow-KI" ist die zweite Hälfte dieser Geschichte. Shadow-KI bedeutet, dass Mitarbeiter KI-Werkzeuge benutzen, ohne dass die Firma es weiß, es genehmigt oder kontrolliert. Eine Marketing-Assistentin fügt eine Kundenliste in einen kostenlosen Chatbot ein. Ein Buchhalter wirft eine Rechnung in eine Web-App, um sie zusammenzufassen. Niemand Zuständiges weiß, dass das passiert. Die Daten sind weg, und es gibt kein Protokoll, keinen Vertrag und keine Kontrolle.

Stellen Sie es sich wie den Bürodrucker vor zwanzig Jahren vor. Alle haben ihn benutzt. Niemand wusste, dass er von jeder Seite eine Kopie behielt. Shadow-KI ist dieselbe Überraschung, nur sind die Seiten Ihre Kundenlisten, Ihre Verträge und Ihre Preise.

In diesem Kapitel geht es um zwei Dinge: was tatsächlich mit Ihren Daten passiert, wenn Sie einen Dienst eines Drittanbieters nutzen, und wie Sie verhindern, dass Ihre eigenen Mitarbeiter still und leise Risiken schaffen. Das gegenteilige Muster — KI auf eigenen Rechnern betreiben — behandelt [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md). Die rechtliche Seite personenbezogener Daten ist das Kernthema von [Kapitel 10](ch10-privacy-and-gdpr.md). Die größere Frage, die eigenen Werkzeuge zu kontrollieren, ist [Kapitel 11](ch11-digital-sovereignty.md).

## Ein wenig Geschichte

**1990er bis 2000er: Software wandert aus dem Regal.** Früher kauften Sie ein Programm auf einer CD und ließen es auf Ihrem eigenen Computer laufen. Dann wanderten E-Mail, Kalender und Dateispeicher ins Internet. Sie hörten auf, die Software zu besitzen, und begannen, Zugang zu ihr zu mieten.

**2000er bis 2015: SaaS wird normal.** „Software as a Service" bedeutete, eine monatliche Gebühr zu zahlen, um die Software von jemand anderem über das Web zu nutzen. Salesforce, Google Workspace und Microsoft 365 machten es alltäglich. Die Bequemlichkeit gewann. Die meisten kleinen Firmen hörten auf, eigene Server zu betreiben.

**2016 bis 2022: Die Daten wandern mit der Software.** Als Ihre Kundenakten, Dokumente und Nachrichten in der Cloud eines Anbieters lebten, waren Ihre Geschäftsdaten dauerhaft außerhalb Ihrer Mauern. Die meisten Menschen akzeptierten das, weil die Werkzeuge gut und der Preis niedrig war.

**November 2022: ChatGPT öffnet die Tür für alle.** Eine leistungsstarke KI wurde in einem kostenlosen Web-Feld verfügbar. Sie brauchten keinen Anbietervertrag mehr, um KI zu nutzen. Sie brauchten nur eine E-Mail-Adresse. Das ist der Moment, in dem Shadow-KI begann, denn jetzt konnte ein einzelner Mitarbeiter Firmendaten an ein Spitzenmodell schicken, ohne jemanden zu fragen.

**2023: die ersten Alarme in Firmen.** Firmen entdeckten, dass Mitarbeiter vertrauliches Material in öffentliche Chatbots fügten. Der Samsung-Fall im Abschnitt „Kuriosität" ist der berühmteste. Mehrere Banken und professionelle Firmen verboten oder beschränkten in dem Jahr öffentliche KI-Werkzeuge.

**2023 bis 2026: Anbieter legen „Enterprise"-Stufen zu.** Als Reaktion verkauften KI-Anbieter Geschäftspläne, die versprachen, nicht mit Ihren Daten zu trainieren, die Daten getrennt zu halten und Verwaltungskontrollen hinzuzufügen. Die Bequemlichkeit blieb; die Versprechen wurden besser. Aber ein Versprechen ist nicht dasselbe wie Kontrolle — deshalb ist dieses Kapitel wichtig.

## Kuriosität

### 10.9 Der Halbleiterkonzern, der seine Geheimnisse in ChatGPT fügte

Anfang 2023 stellte Samsung Electronics — eines der größten Technologieunternehmen der Welt — fest, dass eigene Mitarbeiter vertrauliches Material in einen öffentlichen KI-Chatbot gesteckt hatten.

Die Berichte, erstmals von der koreanischen Finanzzeitung *Korea Economic Daily* im April 2023 veröffentlicht und breit wiederholt, beschrieben drei getrennte Vorfälle in der Halbleitersparte. Im ersten fügte ein Ingenieur fehlerhaften Quellcode aus einem Programm ein, mit dem Messdaten aus einer Chipfabrik heruntergeladen werden, in der Hoffnung, der Chatbot finde den Fehler. Im zweiten luden Mitarbeiter Code hoch, der mit Halbleiterausrüstung und Fehlererkennung zu tun hatte. Im dritten fütterten Mitarbeiter aufgenommene Meeting-Protokolle in das Werkzeug, um Zusammenfassungen zu erhalten. All das geschah innerhalb von etwa drei Wochen, nachdem die Sparte den Zugang zu dem Werkzeug erstmals erlaubt hatte.

Als die Daten einmal im Chatbot waren, lagen sie auf Rechnern, die Samsung nicht gehörten. Das Unternehmen konnte sie nicht leicht zurückholen und konnte nicht sicher sein, dass sie nicht von anderen genutzt oder gesehen würden.

Samsungs Reaktion war unmissverständlich. Es verbot generative KI-Werkzeuge, einschließlich ChatGPT, auf firmeneigenen Computern, Tablets, Handys und im internen Netzwerk. Ein Verstoß konnte bis zur Entlassung führen. Mitarbeitern, die solche Werkzeuge auf privaten Geräten nutzten, wurde gesagt, niemals Firmeninformationen oder personenbezogene Daten einzureichen, die Samsungs geistiges Eigentum preisgeben könnten. Eine interne Umfrage ergab, dass 65 % der Befragten KI-Dienste für ein Sicherheitsrisiko hielten. Gleichzeitig sagte Samsung, es baue eigene interne KI-Werkzeuge für Übersetzung, Dokumentenzusammenfassung und Softwareentwicklung, und arbeite an Wegen, das Hochladen sensibler Informationen an externe Dienste zu blockieren.

Die Lehre ist nicht, dass Samsung nachlässig war. Sie ist: Wenn eine Firma mit Milliarden an Sicherheitsbudget von einem kostenlosen Chatbot überrumpelt wurde, hat eine kleine Firma ohne Sicherheitsteam noch weniger Schutz. Die Bequemlichkeit ist real, und die Leckage ist es auch.

## Ein echtes Geschäftsbeispiel

### Die Agentur, die ihre Kundenliste zweimal verlor

Betrachten Sie eine kleine Marketingagentur, zwanzig Leute, keine IT-Abteilung. Das ist eine zusammengesetzte Geschichte, aber jeder Teil passiert jede Woche in echten Firmen.

Erste Leckage: Eine erfahrene Account-Managerin will schnell ein Angebot umschreiben. Sie öffnet einen kostenlosen KI-Chatbot auf ihrem Laptop und fügt den Entwurf ein, der den noch unveröffentlichten Produktnamen eines Kunden, Budgetzahlen und Kontaktdaten enthält. Sie bekommt eine hübschere Textstelle. Sie denkt nie darüber nach, wohin der Text gegangen ist.

Zweite Leckage: Dieselbe Managerin meldet sich einen Monat später für einen bezahlten „KI-Schreibassistenten" an, der bessere Ergebnisse verspricht. Zum Einrichten verbindet sie ihn mit der E-Mail und dem Laufwerk der Agentur, damit er „die Firmenstimme lernt". Jetzt kann der Anbieter alles lesen: jeder Kunde, jeder Vertrag, jeder interne Scherz, der zur Strategienotiz wird.

Dann kommt das Problem der Weiterentwicklung. Ein Jahr später ändert der Anbieter seinen Plan. Die Funktionen, für die sie bezahlt hat, wandern in eine höhere Stufe. Der Preis verdoppelt sich. Das Modell hinter dem Werkzeug wird gegen ein neueres ausgetauscht, und der Schreibstil, den sie ihr Team trainiert hat, ändert sich still und leise. Sie will weg, aber alles ist in dieses Werkzeug verdrahtet. Ein Wechsel bedeutet, die ganze Agentur woanders anzuschließen und alle neu einzuarbeiten. Das ist Lock-in, und er geschah ohne eine einzige schlechte Entscheidung — nur eine Reihe bequemer.

Nichts davon brauchte böse Absicht. Es brauchte Bequemlichkeit und das Fehlen einer Regel. Die Lösung ist nicht, KI zu fürchten. Sie besteht darin, vorab zu entscheiden, welche Daten wohin dürfen, und den Leuten ein gutes Werkzeug zu geben, damit sie nicht nach einem riskanten greifen.

## So machen Sie es

### 9.1 Die Bequemlichkeit von Cloud-Diensten: warum alle sie nutzen

KI von Drittanbietern ist aus ehrlichen Gründen beliebt, und Sie sollten sie benennen, bevor Sie dagegen argumentieren.

Es gibt kein Einrichten. Sie kaufen keine Hardware, stellen keinen Ingenieur ein und installieren nichts. Sie öffnen eine Webseite und legen los. Für eine kleine Firma ohne technisches Personal ist das die ganze Anziehungskraft.

Es gibt keine Vorabkosten. Die meisten Werkzeuge haben eine kostenlose Stufe oder eine niedrige Monatsgebühr. Sie können eine Idee zum Preis eines Kaffees ausprobieren statt einer Kapitalanschaffung.

Die Qualität ist hoch. Die besten Modelle der Welt sitzen hinter diesen Diensten. Eine Zwei-Personen-Firma kann dieselbe Leistung nutzen wie ein Großkonzern.

Es skaliert sofort. Heute zehnmal so viel Arbeit erledigen? Die Rechner des Anbieters fangen das auf. Sie tun nichts.

Deshalb verbreitete sich Cloud-KI schneller als jede Technologie vor ihr. Der Punkt dieses Kapitels ist nicht, Ihnen das wegzunehmen. Er ist, dass Sie es mit offenen Augen nutzen, denn jede dieser Bequemlichkeiten erkaufen Sie mit einem Stück Kontrolle, von dem Sie nicht merkten, dass Sie es verkauften.

### 9.2 Was mit Ihren Daten passiert, wenn sie das Unternehmen verlassen

Wenn Sie Text in eine KI von Drittanbietern einfügen, können mehrere Dinge geschehen, und Sie sehen meist nicht, welche.

Ihre Daten überqueren das Internet zu den Servern des Anbieters, oft in ein anderes Land. Dort werden sie zumindest eine Zeit lang auf Hardware gespeichert, die Sie nicht kontrollieren und nicht prüfen können.

Sie können von automatisierten Systemen zur Sicherheitsprüfung gelesen werden. Sie können zum Debuggen protokolliert werden. Support-Mitarbeiter in einem anderen Land können sie sehen. Nichts davon ist ungewöhnlich; so arbeiten große Dienste.

Am wichtigsten: Sie können zum Trainieren des Modells des Anbieters genutzt werden. „Training" bedeutet, die Firma füttert Ihren Text in ihr System, damit das Modell daraus lernt. Wenn das passiert, kann ein Fragment Ihres vertraulichen Textes Antworten formen, die anderen Kunden gegeben werden. Das ist der einzelne größte Grund, vorsichtig zu sein.

Manche Geschäftspläne versprechen, nicht mit Ihren Daten zu trainieren. Dieses Versprechen ist etwas wert, aber es ist eine Vertragsklausel, keine Mauer. Sie vertrauen dem Anbieter, dass er es über jedes Produkt und jedes Land hinweg einhält. Die sichere Regel ist einfach: Behandeln Sie jede KI von Drittanbietern so, als könnte alles, was Sie schicken, öffentlich werden. Wenn dieser Gedanke für eine bestimmte Datei inakzeptabel ist, schicken Sie diese Datei nicht.

### 9.3 Das Transparenzproblem: Sie wissen nie wirklich, wie Ihre Daten genutzt werden

Sie können nicht in einen KI-Dienst eines Drittanbieters hineinschauen. Das ist das Kernproblem, und es wird nicht verschwinden.

Sie wissen nicht, welches Modell Ihnen geantwortet hat. Anbieter tauschen Modelle aus, ohne es Ihnen zu sagen. Sie wissen nicht, wo Ihre Daten gespeichert wurden, wer darauf zugreifen konnte oder wie lange sie aufbewahrt wurden. Sie wissen nicht, ob ein Unterauftragnehmer in einem anderen Land sie verarbeitet hat. Sie wissen nicht, ob sie zum Training genutzt wurde, selbst wenn Sie denken, dass nicht.

Die Datenschutzrichtlinie des Anbieters ist von Anwälten geschrieben, nicht von Ingenieuren, und sie beschreibt, was sie tun *dürfen*, nicht was sie in Ihrem konkreten Fall tun *werden*. Sie zu selten gibt eine klare Antwort.

Deshalb ist der praktische Test so nützlich. Statt zu versuchen, das System zu verstehen, stellen Sie eine Frage über die Daten: *Wäre es annehmbar, wenn das morgen öffentlich würde?* Für einen öffentlichen Blogbeitrag, ja. Für die Gehaltsdatei eines Kunden, nein. Dieser eine Test ersetzt tausend Fragen, die Sie nicht beantworten können.

Wenn Sie echte Transparenz brauchen, ist die einzige ehrliche Quelle ein System, das Sie prüfen können — Ihr eigener Rechner oder offene Software, die jemand auditiert werden kann. Das ist das Thema von [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) und [Kapitel 11](ch11-digital-sovereignty.md).

### 9.4 Das Weiterentwicklungsproblem: Modelle ändern sich, Verträge ändern sich, Preise ändern sich

Ein Dienst eines Drittanbieters ist nichts, was Sie kaufen; er ist eine Beziehung, die sich unter Ihren Füßen ständig ändert.

Das Modell ändert sich. Das heutige Werkzeug läuft nächstes Quartal vielleicht auf einem anderen Modell. Die Antworten ändern sich. Der Stil ändert sich. Etwas, das in Ihrem Arbeitsablauf gut funktionierte, kann schlechter werden, oder einfach anders, ohne Warnung und ohne Möglichkeit, bei der alten Version zu bleiben.

Der Vertrag ändert sich. Bedingungen, denen Sie bei der Anmeldung zugestimmt haben, können aktualisiert werden. Funktionen, auf die Sie sich verließen, können hinter einen höheren Plan wandern. Das Versprechen über Trainingsdaten kann umformuliert werden.

Der Preis ändert sich. Ein billiges Werkzeug, das Sie jetzt in Ihr Geschäft verdrahtet haben, kann den Preis erhöhen, und Sie stehen vor einer schmerzhaften Wahl: mehr zahlen oder alles herausreißen.

Das ist das versteckte Risiko der Bequemlichkeit. Sie bauen auf Boden, den jemand anderes kontrolliert, und er kann den Boden verlagern, wann er will. Die Verteidigung besteht darin, Ihre wichtigen Daten und Ihre Kernarbeitsabläufe portabel zu halten und niemals einen einzelnen Anbieter zum einzigen Ort werden zu lassen, an dem Ihre Arbeit stattfinden kann.

### 9.5 Lock-in: wie schwer es später ist, den Anbieter zu wechseln

Lock-in bedeutet, dass ein Anbieterwechsel so kostspielig ist — an Zeit, Geld oder Störung —, dass Sie ihn realistisch nicht vollziehen können. Sie sind „eingesperrt".

Es geschieht auf drei Weisen. **Daten-Lock-in:** Ihre Daten sind in einem Format gespeichert, das nur dieser Anbieter gut liest, oder Sie können sie nicht sauber exportieren. **Arbeitsablauf-Lock-in:** Ihr Tagesprozess ist um dieses Werkzeug herum gebaut, ein Wechsel bedeutet also, alle neu einzuarbeiten und Vorlagen neu zu bauen. **Integrations-Lock-in:** Das Werkzeug ist mit Ihrer E-Mail, Ihrem CRM, Ihren Dateien verbunden, und es herauszuziehen bricht all diese Verknüpfungen.

Lock-in gibt dem Anbieter Macht über Sie. Er weiß, dass Gehen schwer ist, was Ihre Position schwächt, wenn er Preise erhöht oder Bedingungen ändert.

Um frei zu bleiben, bestehen Sie von Anfang an auf drei Dingen. Erstens müssen Ihre Daten in einem schlichten, gängigen Format exportierbar sein. Zweitens, bewahren Sie Ihre Kerndaten dort auf, wo Sie die Kontrolle haben, und lassen Sie den Anbieter mit einer Kopie arbeiten. Drittens, gestalten Sie Ihren Arbeitsablauf so, dass die KI ein Schritt ist, nicht die ganze Maschine, damit Sie den Schritt austauschen können. Das Ziel ist nicht, Anbieter zu vermeiden. Es ist, einen innerhalb einer Woche verlassen zu können, nicht erst in einem Jahr.

### 9.6 Shadow-KI: wenn Mitarbeiter nicht autorisierte Werkzeuge nutzen

Shadow-KI ist das Risiko, das Sie nicht sehen, weil es von Ihren eigenen vertrauenswürdigen Mitarbeitern geschaffen wird.

Es entsteht, weil gute offizielle Werkzeuge langsam freizugeben sind, riskante kostenlose aber sofort da. Ein Mitarbeiter unter Zeitdruck fügt eine Kunden-E-Mail in einen kostenlosen Chatbot ein, um eine Antwort zu entwerfen. Niemand hält ihn auf, weil niemand es weiß.

Warum es gefährlich ist: Die Daten gehen ohne Vertrag, ohne Prüfung und ohne Protokoll. Sie können dem Kunden nichts sagen, Sie können die Daten später nicht finden, und Sie können nicht beweisen, was geschah. Wenn das Werkzeug mit diesen Daten trainiert, können Ihre vertraulichen Informationen am Ende ein öffentliches Modell formen.

Wie man es erkennt: ungewöhnliche Abbuchungen auf Firmenkarten für KI-Abos; Mitarbeiter, die sich beschweren, freigegebene Werkzeuge seien zu langsam; plötzliche „magische" Verbesserungen bei Ausgaben, die kein freigegebenes Werkzeug erklärt.

Wie man es stoppt: verbieten Sie nicht nur. Ein Verbot ohne gute Alternative drängt das Verhalten nur in den Untergrund. Geben Sie den Leuten ein freigegebenes Werkzeug, das schnell und gut genug ist, und sie werden es nutzen. Dann machen Sie die Regel klar, schulen Sie darin und überwachen Sie leicht. Die ganze Policy-Seite steht in Abschnitt 9.8 und in den KI-Policy-Vorlagen für Firmen in den Anhängen des Buches.

### 9.8 So mindern Sie die Risiken: Sorgfaltsprüfung, Verträge, interne Richtlinie

Sie reduzieren das Risiko mit drei Schichten. Machen Sie alle drei.

**Schicht 1: Sorgfaltsprüfung — prüfen Sie vor dem Kauf.**
Bevor Sie einen KI-Anbieter einführen, stellen Sie die harten Fragen. Wo werden Daten gespeichert, und in welchen Ländern? Trainieren Sie mit Kundendaten, und können Sie schriftlich garantieren, dass Sie es nicht tun? Wer kann darauf zugreifen, einschließlich Unterauftragnehmer? Wie lange werden sie aufbewahrt, und wie werden sie gelöscht? Sind sie bei der Übertragung und im Ruhezustand verschlüsselt? Welche Zertifizierungen haben Sie? Holen Sie die Antworten schriftlich, nicht in einem Verkaufsgespräch. Ein Anbieter, der nicht klar antworten kann, sagt Ihnen damit etwas. Eine bewertete Version dieser Fragen steht im Due-Diligence-Scorecard für Anbieter in den Anhängen.

**Schicht 2: Verträge — setzen Sie die Versprechen aufs Papier.**
Eine mündliche Zusage ist wertlos. Verlangen Sie im Vertrag: kein Training mit Ihren Daten; Speicherort der Daten in einem Land, das Sie akzeptieren; das Recht, alle Ihre Daten in einem nutzbaren Format zu exportieren; das Recht auf Löschung; die Pflicht, Sie über Datenschutzverletzungen und über große Modell- oder Bedingungsänderungen zu informieren; und Grenzen für Unterauftragnehmer. Wenn der Anbieter das nicht unterschreibt, ist das Ihre Antwort.

**Schicht 3: Interne Richtlinie — sagen Sie Ihren Leuten die Regeln.**
Schreiben Sie eine kurze, schlichte KI-Richtlinie. Legen Sie fest, welche Werkzeuge freigegeben sind. Legen Sie fest, welche Daten niemals in eine externe KI dürfen — personenbezogene Kundendaten, Finanzunterlagen, Verträge, Quellcode, Passwörter. Geben Sie den Mitarbeitern ein schnelles freigegebenes Werkzeug, damit sie nicht nach einem riskanten greifen. Schulen Sie alle in einer kurzen Sitzung in der Regel. Prüfen Sie die Liste der freigegebenen Werkzeuge jedes Quartal. Eine Vorlage steht im Anhang.

Die Reihenfolge zählt. Erst prüfen, zweit vertraglich festhalten, dritt Richtlinie. Die meisten Firmen überspringen die ersten beiden und wundern sich, warum sie sich exponiert haben.

## Ethik und Verantwortung

KI von Drittanbietern wirft eine Pflicht auf, die Sie zwei Gruppen schulden: den Menschen, deren Daten Sie haben, und Ihren eigenen Mitarbeitern.

**Ihren Kunden und Mitarbeitern.** Wenn ein Kunde Ihnen personenbezogene Daten gibt, vertraut er darauf, dass Sie sie schützen. Diese Daten an eine KI eines Drittanbieters zu schicken, die Sie nicht geprüft haben, kann dieses Vertrauen brechen, selbst wenn nichts Schlimmes passiert. Sie sind verantwortlich dafür, wohin deren Daten gehen. Die rechtlichen Pflichten stehen in [Kapitel 10](ch10-privacy-and-gdpr.md); das ethische Prinzip ist einfach — tun Sie die private Information jemandes nicht irgendwohin, wohin Sie Ihre eigene nicht tun würden.

**Ihren Mitarbeitern gegenüber, wegen Shadow-KI.** Passen Sie auf, dass Sie Schutz nicht in Überwachung verwandeln. Wenn Sie die KI-Nutzung überwachen, sagen Sie den Leuten, was Sie überwachen und warum. Eine klare Regel plus ein gutes Werkzeug ist fair. Heimliche Überwachung vertrauenswürdiger Mitarbeiter schadet Moral und Vertrauen. Zielen Sie auf Leitplanken, nicht auf einen Überwachungsstaat.

**Seien Sie ehrlich darüber, was Sie nicht kontrollieren.** Wenn ein Kunde fragt, ob seine Daten ein externes Modell trainiert, sollten Sie wahrheitsgemäß antworten können. Wenn Sie es nicht wissen, sagen Sie das und beheben Sie es. Sicherheit überzubehaupten ist schlimmer, als eine Lücke einzugestehen.

## Zu vermeidende Fehler

1. **Die Demo lesen, nicht den Datenfluss.** Eine schicke Demo sagt Ihnen nichts darüber, wohin Ihre Daten gehen. Stellen Sie zuerst die Speicher- und Trainingsfragen.
2. **Einem mündlichen „wir trainieren nicht mit Ihren Daten" vertrauen.** Wenn es nicht im Vertrag steht, existiert es nicht.
3. **Ein Werkzeug mit Ihrem ganzen Laufwerk verbinden.** „Unsere Stimme lernen" bedeutet oft „alles lesen". Geben Sie dem Werkzeug das Wenigste, was es braucht.
4. **Shadow-KI ohne Alternative verbieten.** Ein Verbot ohne gutes freigegebenes Werkzeug versteckt das Verhalten nur.
5. **Keine schriftliche Richtlinie.** Wenn die Regel nicht geschrieben und geschult ist, ist sie keine Regel.
6. **Die Länderfrage ignorieren.** Daten, die unter einem anderen Rechtssystem liegen, können anders zugänglich sein. Wissen Sie, wo sie sitzen.
7. **Annehmen, ein Bezahlplan sei gleich sicher.** Ein bezahlter Verbraucherplan ist nicht dasselbe wie ein vertraglicher Enterprise-Plan mit den richtigen Bedingungen.
8. **Kein Exportplan.** Wenn Sie Ihre Daten nicht herausbekommen, sind Sie vom ersten Tag an eingesperrt.
9. **Die Datenschutzrichtlinie als Garantie behandeln.** Sie listet auf, was sie dürfen, nicht was sie für Sie tun werden.
10. **Den Menschen vergessen.** Die Leckage beginnt fast immer mit einer Person unter Zeitdruck. Beheben Sie den Druck und geben Sie einen sicheren Weg.

## Praktische Übung

### 9.9 Analysieren Sie Ihre jetzigen KI-Anbieter

Nehmen Sie eine Stunde und tun Sie das für jedes KI-Werkzeug, das Ihre Firma heute nutzt, auch für die, die Mitarbeiter still benutzen.

Machen Sie eine Tabelle. Eine Zeile pro Werkzeug. Spalten:

- **Werkzeugname** und wer sich dafür angemeldet hat.
- **Welche Daten hineingehen.** Konkret: Kunden-E-Mails, Rechnungen, Verträge, Code, öffentlicher Text.
- **Wo sie gespeichert sind,** wenn Sie es wissen. Wenn unbekannt, schreiben Sie „unbekannt".
- **Trainieren sie mit unseren Daten?** Ja / Nein / Unbekannt.
- **Gibt es einen Vertrag,** oder nur ein Durchklicken?
- **Können wir unsere Daten exportieren?** Ja / Nein / Unbekannt.
- **Risikostufe** für die Daten, die Sie tatsächlich hineingeben: Niedrig / Mittel / Hoch.

Lesen Sie nun die Hochrisiko-Zeilen. Fragen Sie für jede: Wäre es annehmbar, wenn diese Daten öffentlich würden? Wenn nein, haben Sie drei Möglichkeiten — hören Sie auf, diese Daten hineinzugeben, wechseln Sie zu einem Anbieter, der die richtigen Bedingungen unterschreibt, oder verlagern Sie diese Aufgabe auf ein Werkzeug, das Sie kontrollieren (siehe [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md)).

Fragen Sie abschließend herum. Senden Sie eine ehrliche Nachricht an Ihr Team: „Welche KI-Werkzeuge benutzt ihr für die Arbeit, über die wir nicht gesprochen haben?" Die Antworten sind Ihre echte Shadow-KI-Liste. Bestrafen Sie die Ehrlichkeit nicht; beheben Sie die Lücken, die sie aufdeckt.

## Checkliste

### 9.10 Fragen, die Sie jedem KI-Anbieter stellen sollten

Bevor Sie echte Daten in einen KI-Dienst eines Drittanbieters stecken, holen Sie zu jedem dieser Punkte eine schriftliche Antwort.

- [ ] **Wo werden unsere Daten physisch gespeichert,** und in welchen Ländern?
- [ ] **Trainiert ihr eure Modelle mit unseren Daten?** Können ihr im Vertrag „Nein" zusichern?
- [ ] **Wer kann auf unsere Daten zugreifen,** einschließlich Mitarbeiter und Unterauftragnehmer, und von wo?
- [ ] **Wie lange bewahrt ihr unsere Daten auf,** und wie lassen wir sie löschen?
- [ ] **Sind unsere Daten verschlüsselt,** sowohl bei der Übertragung als auch im Ruhezustand?
- [ ] **Können wir alle unsere Daten** jederzeit in einem gängigen, nutzbaren Format exportieren?
- [ ] **Werdet ihr uns** über eine Datenschutzverletzung informieren, und innerhalb welcher Zeit?
- [ ] **Werdet ihr uns sagen,** bevor ihr das Modell, den Preis oder die Bedingungen ändert?
- [ ] **Welche Sicherheitszertifizierungen** habt ihr, und könnt ihr sie vorzeigen?
- [ ] **Gibt es Unterauftragnehmer,** und sind sie an dieselben Bedingungen gebunden?
- [ ] **Welchen Rechtsbehelf haben wir,** wenn ihr unsere Daten missbraucht?
- [ ] **Gibt es eine Verwaltungskonsole,** damit wir die Nutzung sehen und steuern können?

Wenn ein Anbieter diese Fragen nicht klar und schriftlich beantworten kann, behandeln Sie das Werkzeug als Hochrisiko und halten Sie sensible Daten daraus heraus.

## Wichtige Punkte

- Ein KI-Dienst eines Drittanbieters läuft auf den Rechnern von jemand anderem, sodass Sie im Moment, in dem Ihre Daten gehen, Kontrolle gegen Bequemlichkeit eintauschen.
- Das größte Risiko ist, dass Ihre vertraulichen Daten zum Trainieren eines Modells genutzt werden könnten, das anderen dient, und Sie es oft weder sehen noch stoppen können.
- Anbieter tauschen Modelle, Verträge und Preise unter Ihren Füßen aus, und Lock-in macht das Verlassen teuer — halten Sie also Ihre Daten exportierbar und Ihren Arbeitsablauf austauschbar.
- Shadow-KI sind Ihre eigenen Mitarbeiter, die nicht freigegebene Werkzeuge nutzen; stoppen Sie sie mit einem guten freigegebenen Werkzeug plus einer klaren schriftlichen Regel, nicht mit Verboten allein.
- Schützen Sie sich in drei Schichten: prüfen Sie zuerst den Anbieter, setzen Sie zweit die Versprechen in einen Vertrag, und legen Sie dritt eine interne Richtlinie fest.
