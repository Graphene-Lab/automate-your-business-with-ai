# Kapitel 26 — Vertrieb und Marketing

## In einfachen Worten

Vertrieb und Marketing sind, wo KI dir helfen kann, mehr Kunden zu finden, besser mit ihnen zu sprechen und weniger Zeit mit Raten zu verbringen. Die Arbeit hier ist voller kleiner, sich wiederholender Jobs: Sortieren, welche Leads einen Anruf wert sind, E-Mails schreiben, dieselben Fragen auf deiner Website beantworten und versuchen zu verstehen, was deine Kunden wollen. KI ist in all dem gut.

Die Kernidee ist *Personalisierung im großen Maßstab*. Ein guter Verkäufer erinnert sich an jeden Kunden, schneidet die Botschaft zu und fasst im richtigen Moment nach. Ein kleines Team kann das nicht für Tausende von Menschen. KI kann es. Sie kann sich jeden Lead ansehen und raten, wie wahrscheinlich er kauft, eine E-Mail schreiben, die klingt, als sei sie für diese Person geschrieben, einem Besucher um 2 Uhr nachts eine Frage beantworten und erkennen, welche Kunden kurz davor sind zu gehen.

Dieses Kapitel deckt vier Jobs ab: Leads bewerten (raten, wer am ehesten kauft), E-Mails und Inhalte schreiben, Chatbots und Assistenten betreiben, und Kunden analysieren, um zu verstehen, was sie wollen und wer in Gefahr ist zu gehen.

Eine ehrliche Warnung vorweg: KI ist ein mächtiger Verstärker. Sie wird eine gute Botschaft mehr Menschen erreichen lassen, und sie wird eine schlechte Botschaft mehr Menschen erreichen lassen. Sie kann dich auch zu Spam drängen — zu viel, zu oft, an Leute senden, die nicht gefragt haben. Das Ziel ist nicht, alle zuzuballern; es ist, den richtigen Menschen mit der richtigen Botschaft zur richtigen Zeit zu erreichen. Die Methode zu beurteilen, ob irgendetwas davon sich auszahlt, lebt in [Kapitel 16 — Ziele, Kosten und Return on Investment](ch16-goals-costs-and-return-on-investment.md); dieses Kapitel zeigt dir, was du automatisierst und wie.

## Ein bisschen Geschichte

**1990er: Massen-Marketing und die Mailingliste.** Marketing-Automatisierung begann mit einfachen E-Mail-Listen. Ein Unternehmen konnte eine Botschaft an Tausende auf einmal senden. Es war billig und breit, aber stumpf — jeder bekam dieselbe Botschaft, ob sie zu ihm passte oder nicht. Das war die Ära von „spray and pray" (draufsprühen und beten).

**2000er: das CRM und der Trichter.** Customer-Relationship-Management-Software (CRM) — eine Datenbank jedes Kunden und jeder Interaktion — kam. Vermarkter begannen, in einem „Trichter" (Funnel) zu denken: viele Leute treten oben ein, weniger schaffen es unten zum Kauf. Das CRM ließ dich verfolgen, wo jede Person im Trichter war, und nachfassen. Daten kamen ins Bild.

**2010er: Segmentierung und Personalisierung.** Mit mehr Daten lernten Vermarkter, ihr Publikum in Gruppen (Segmente) zu teilen und jeder Gruppe eine andere Botschaft zu senden. „Leute, die X kauften, kauften auch Y." Personalisierung machte Botschaften relevanter und wirksamer. Aber sie war meist noch regelbasiert: Wenn ein Kunde dies tat, sende das.

**Ende 2010er: Maschinelles Lernen bewertet Leads.** Maschinelles Lernen — Software, die Muster aus vielen Beispielen lernt — begann, Leads zu bewerten. Statt dass eine Person riet, wen sie zuerst anruft, schaute das Modell auf Hunderte von Signalen (Firmengröße, welche Seiten sie besuchten, wie sie dich fanden) und reihte Leads danach, wie wahrscheinlich sie kauften. Vertriebsteams hörten auf, Zeit mit kalten Leads zu verschwenden.

**2020er: Generative KI schreibt und chattet.** Große Sprachmodelle — KI, trainiert auf riesigen Textmengen — können jetzt E-Mails, Werbetexte und Produktbeschreibungen schreiben, die menschlich klingen. Chatbots, gebaut auf derselben Technologie, können ein echtes Gespräch führen, Fragen beantworten und einen Kunden durch einen Kauf leiten. Der Chatbot bewegte sich von einer frustrierenden Menü-Liste von Buttons zu etwas, das tatsächlich versteht, was du getippt hast.

**Jetzt: Agenten, die die ganze Reise bearbeiten.** Der neueste Schritt ist der Agent — KI, die eine Aufgabe über mehrere Schritte trägt. Ein kundengerichteter Agent kann eine Frage beantworten, den Bestand prüfen und einen Kauf leiten. Ein interner Agent kann eine Support-Anfrage nehmen und das Ticket erstellen. Das mobilezone-Beispiel unten nutzt genau das: zwei Agenten, einer für Kunden und einer für das interne Team.

Der Bogen: von einer Botschaft an alle, zu verfolgten Trichtern, zu Segmenten, zu bewerteten Leads, zu KI, die schreibt und chattet. Jeder Schritt machte Marketing persönlicher und weniger ein Ratespiel.

## Neugier

### 26.5 Der Chatbot, der zwei Agenten wurde

Als mobilezone, ein Schweizer Telekom-Einzelhändler, seinen alten Chatbot ersetzte, baute es nicht einen besseren Bot. Es baute zwei verschiedene Agenten für zwei verschiedene Jobs: einen mit Blick auf Kunden, einen mit Blick auf das eigene Personal. Diese Aufteilung ist die interessante Idee. Dieselbe KI-Technologie diente zwei Publikum auf zwei sehr unterschiedliche Arten — ein freundlicher Einkaufsführer auf der Website und ein Ticket-schreibender Helfer innerhalb der Firma. Die Geschichte, mit den echten Zahlen, steht unten.

## Ein echtes Geschäftsbeispiel

**mobilezone: zwei Copilot-Agenten, einer für Kunden und einer für IT.**

mobilezone ist ein Schweizer Telekommunikations-Einzelhändler mit mehr als 125 physischen Filialen, der Handys, Tarife und vernetzte Geräte verkauft. Es hatte zwei getrennte Probleme. Auf der Kundenseite war der alte Website-Chatbot starr und frustrierend — er konnte nur ein festes Menü abarbeiten und scheiterte oft daran, echte Fragen zu beantworten. Innerhalb der Firma mussten Mitarbeiter umständliche Formulare ausfüllen, um IT-Probleme zu melden, was alle ausbremste.

Laut einer veröffentlichten Microsoft-Kundenfallstudie baute mobilezone beide Seiten mit Microsoft Copilot Studio neu — einem Werkzeug zum Bauen von konversationellen KI-Agenten — zusammen mit Dynamics 365 (seinem CRM) und der Power Platform (Microsofts Low-Code-Automatisierungswerkzeugen). Es baute zwei Agenten:

- **Mia — der kundengerichtete Agent.** Mia ist ein mehrsprachiger Assistent auf der Website. Sie beantwortet viele Kundenfragen, hilft Besuchern, das richtige Produkt oder den richtigen Tarif zu finden, und leitet sie durch einen Kauf. Weil sie natürliche Sprache versteht, bewältigt sie die Fragen, die der alte Menü-Bot nicht konnte.
- **Supporto — der interne IT-Agent.** Supporto ist ein Helfer für mobilezones eigenes Personal. Statt ein starres Formular auszufüllen, sagt ein Mitarbeiter Supporto in klaren Worten, was kaputt ist, und der Agent erstellt das IT-Ticket automatisch.

Die berichteten Ergebnisse: Die Agenten bearbeiten jetzt **mehr als 1.600 Chats pro Monat**, und der interne IT-Agent **senkte die IT-Lösungszeit um etwa 50 %**. Ebenso wichtig reduzierten die Agenten die Last im externen Kontaktcenter von mobilezone (der ausgelagerte Telefon-Support), und der Kunden-Agent verbesserte die Online-Conversion, indem er shoppers durch Produktentdeckung führte.

Zwei Lektionen stechen hervor. Erstens diente dieselbe Technologie zwei sehr unterschiedlichen Jobs — externer Vertrieb und interner Support — was zeigt, wie flexibel diese Agenten sind. Zweitens ersetzte mobilezone keine Menschen; es verlagerte die einfachen, sich wiederholenden Gespräche zum Agenten, damit seine Leute sich auf die schwierigeren konzentrieren konnten. Das ist das realistische Versprechen: KI bewältigt das Volumen, Menschen bewältigen den Wert.

Ein Hinweis zur Quelle: Die obigen Zahlen stammen aus Microsofts veröffentlichter Kundengeschichte über mobilezone. Behandle sie als mobilezones berichtete Ergebnisse; deine eigenen Zahlen hängen von deinem Volumen und Setup ab.

## Wie man es macht

### 26.1 Lead-Bewertung

Ein *Lead* ist eine Person oder Firma, die etwas Interesse gezeigt hat — sie füllte ein Formular aus, lud etwas herunter oder stellte eine Frage. Du hast keine Zeit, jeden Lead mit demselben Aufwand anzurufen. Lead-Bewertung bedeutet, Leads danach zu reihen, wie wahrscheinlich sie kaufen, damit dein Team die heißesten zuerst anruft.

**Wie KI einen Lead bewertet.** Ein Machine-Learning-Modell schaut viele Signale auf einmal an: die Größe der Firma des Leads, die Jobbezeichnung der Person, welche Seiten sie besuchte, wie oft sie zurückkam, ob sie deine E-Mails öffnete, und wie sie dich fand. Aus vergangenen abgeschlossenen Deals lernt das Modell, welche Signale mit einem Verkauf zusammengehen, und bewertet jeden neuen Lead entsprechend.

**Warum es das Raten schlägt.** Eine Person, die Leads nach Bauchgefühl bewertet, ist langsam und voreingenommen — sie neigt dazu, die Leads zu bevorzugen, die sich „freundlich" anfühlen, nicht die, die tatsächlich konvertieren. KI bewertet konsistent und schnell, und sie kann Hunderte von Signalen abwägen, die ein Mensch nicht im Kopf behalten kann.

**Fang einfach an.** Du brauchst am ersten Tag kein perfektes Modell. Fang mit ein paar klaren Signalen an — Firmengröße, Rolle und was sie herunterluden — und bewerte Leads von Hand in deinem CRM. Wenn du mehr abgeschlossene Deals sammelst, kann ein echtes Modell daraus lernen und sich verbessern.

**Füttere die Schleife.** Das Modell wird besser, wenn du ihm sagst, welche Leads tatsächlich Kunden wurden. Stelle sicher, dass dein CRM das Ergebnis jedes Deals aufzeichnet, damit die Bewertung aus echten Ergebnissen lernt, nicht aus Vermutungen.

**Vertraue dem Score nicht zu sehr.** Ein Score ist ein Hinweis, kein Urteil. Ein hoher Score bedeutet „bald anrufen", nicht „garantierter Verkauf". Ein niedriger Score ist vielleicht trotzdem ein guter Kunde, den das Modell noch nicht gelernt hat. Nutze den Score, um Priorität zu setzen, nicht um Menschen zu ignorieren.

### 26.2 E-Mail und Inhalte

E-Mails, Werbetexte und Produktbeschreibungen zu schreiben kostet Stunden. Generative KI — KI, die Text erzeugt — kann sie schnell entwerfen, und ein Mensch kann sie so bearbeiten, dass sie richtig klingen.

**Entwirf, verschicke nicht.** Nutze KI, um einen ersten Entwurf zu produzieren, dann bearbeite ihn. KI ist hervorragend darin, schnell Worte aufs Blatt zu bekommen, und schrecklich darin, ohne Führung deine genaue Stimme, deine Marke und die Gefühle deines Kunden zu kennen. Der Entwurf ist zu 70 % da; deine Bearbeitung ist die letzte 30-%-Strecke, die ihn zu deinem macht.

**Personalisiere im großen Maßstab.** KI kann eine Vorlage nehmen und sie für viele Leute anpassen: den Namen des Empfängers einfügen, referenzieren, was sie sich ansahen, das Angebot auf ihr Segment zuschneiden. Das ist die Personalisierung-im-großen-Maßstab-Idee von früher — eine Botschaft, die sich anfühlt, als sei sie für eine Person geschrieben, an Tausende gesendet.

**Passe den Kanal an.** Eine E-Mail, ein Social-Post und eine Produktseite brauchen unterschiedliche Längen und Töne. Sag der KI den Kanal und das Ziel, und bearbeite entsprechend. Eine lange E-Mail funktioniert nicht als Tweet; ein Tweet funktioniert nicht als Landingpage.

**Behalte die menschliche Stimme.** KI-Text kann flach, generisch oder zu eifrig klingen. Lies jeden Entwurf laut. Wenn er nicht klingt wie etwas, das du sagen würdest, schreib ihn um. Deine Kunden merken, wann eine Botschaft generisch ist.

**Lass nie KI ohne Prüfung senden.** Eine ungeprüfte KI-E-Mail kann einen falschen Preis, einen falschen Namen oder eine unangemessene Zeile enthalten. Lass immer einen Menschen lesen, bevor sie hinausgeht. Das ist dieselbe Regel wie in der Finanzbuchhaltung: KI entwirft, Mensch genehmigt.

**Beachte das Volumen.** KI macht es leicht, mehr E-Mails zu senden als du solltest. Mehr ist nicht besser. Zu viel an Leute zu senden, die nicht gefragt haben, ist Spam, und es verbrennt deine Liste und deinen Ruf. Sende weniger, aber lass jedes zählen.

### 26.3 Chatbots und Assistenten

Ein Chatbot ist ein Programm, das mit einem Kunden auf deiner Website oder App spricht. Moderne Chatbots, gebaut auf großen Sprachmodellen, verstehen, was eine Person tippt, und antworten in klarer Sprache — ein großer Schritt gegenüber den alten „Drücke 1 für Vertrieb"-Menüs.

**Was ein guter Chatbot tut.** Er beantwortet gängige Fragen sofort (Preis, Öffnungszeiten, Versand, Rückgaben), leitet einen Besucher zum richtigen Produkt, erfasst Kontaktdaten für ein Nachfassen und übergibt an einen Menschen, wenn er nicht helfen kann. Die Übergabe ist kritisch: Ein Chatbot, der nie übergibt, frustriert Leute und verliert Verkäufe.

**Entwirf die Übergabe zuerst.** Bevor du den Bot baust, entscheide, wann er das Gespräch an eine Person weitergeben soll. Wenn der Bot unsicher ist, wenn der Kunde nach einem Menschen fragt, wenn das Thema sensibel ist — übergib. Ein Bot, der seine Grenzen kennt, wird vertraut; einer, der blufft, nicht.

**Trainiere auf deinen echten Fragen.** Füttere den Bot mit den Fragen, die Kunden tatsächlich stellen, mit den Antworten, die du willst. Je mehr er über deine spezifischen Produkte und Richtlinien weiß, desto nützlicher ist er. Ein generischer Bot gibt generische Antworten, die frustrieren.

**Lass ihn viele Sprachen sprechen.** Einer der größten Gewinne eines modernen Chatbots ist mehrsprachige Unterstützung. Er kann einen Kunden in dessen eigener Sprache beantworten, ohne dass du Übersetzer einstellst. Genau das macht mobilezones Mia.

**Miss, was er bewältigt und was er nicht schafft.** Verfolge, wie viele Gespräche der Bot allein löst, wie viele er übergibt, und was er nicht beantworten konnte. Die Ausfälle sind Gold — sie sagen dir, was du ihm als Nächstes beibringen sollst. (Dieselben Chatbot-Ideen, auf Support statt Vertrieb angewandt, sind in [Kapitel 27 — Kundenbetreuung und Support](ch27-customer-care-and-support.md) behandelt.)

### 26.4 Kundenanalyse

Kundenanalyse bedeutet, Daten zu nutzen, um zu verstehen, wer deine Kunden sind, was sie wollen und wer kurz davor ist zu gehen. KI ist hier stark, weil sie Muster über Tausende von Kunden sehen kann, die kein Mensch von Hand entdecken könnte.

**Segmentiere deine Kunden.** KI kann Kunden nach Verhalten gruppieren: Vieltaufer, Großausgeber, saisonale Käufer, gefährdete Kunden. Jede Gruppe braucht eine andere Botschaft. Das ist Segmentierung, und KI tut es schneller und genauer als manuelle Regeln.

**Erkenne Churn, bevor er geschieht.** *Churn* bedeutet, ein Kunde hört auf zu kaufen. KI kann Signale ansehen — weniger Besuche, kleinere Bestellungen, weniger Engagement — und Kunden markieren, die wahrscheinlich bald gehen. Das gibt dir Zeit, sie mit einem Angebot oder einem persönlichen Anruf zurückzugewinnen, statt es zu erfahren, nachdem sie weg sind.

**Finde das nächstbeste Angebot.** KI kann ansehen, was ein Kunde kaufte, und vorschlagen, was er als Nächstes wahrscheinlich wollen wird. „Kaufte ein Handy, braucht wahrscheinlich eine Hülle und eine Versicherung." Das ist die Empfehlungsmaschinen-Idee, und sie hebt den Wert jedes Kunden.

**Lies, was Kunden sagen.** KI kann Bewertungen, Umfrage-Kommentare und Support-Chats lesen und die Hauptthemen herausziehen: was Leute lieben, was sie nervt, was sie verlangen. Statt tausend Kommentare einzeln zu lesen, bekommst du eine Zusammenfassung der großen Themen. Das verwandelt rohes Feedback in etwas, worauf du handeln kannst.

**Behandle Menschen nicht als Datenpunkte.** Analyse ist ein Werkzeug, um Kunden besser zu bedienen, nicht um sie zu manipulieren. Nutze, was du lernst, um ihre Erfahrung zu verbessern, nicht um ihre Schwächen auszunutzen. Die Linie zwischen Personalisierung und Manipulation ist real, und du solltest auf der richtigen Seite davon bleiben.

## Ethik und Verantwortung

Vertrieb und Marketing berühren die Aufmerksamkeit und das Vertrauen der Menschen direkt, deshalb zählt die ethische Linie.

**Spamme nicht.** KI macht es leicht, zu viel zu senden. Leuten Botschaften zu senden, die nicht gefragt haben, oder mehr als sie vereinbarten, ist Spam. Achte Einwilligung und Häufigkeit. Eine kurze Liste von Leuten, die deine Botschaften wollen, schlägt eine riesige Liste, die du zuballerst.

**Sei ehrlich in KI-geschriebenen Texten.** KI kann eine Behauptung schreiben, die wahr klingt, aber nicht wahr ist. Prüfe jede faktische Behauptung — Preis, Funktionen, Ergebnisse — bevor sie verschickt wird. Lass nie KI einen Vorteil erfinden, den du nicht liefern kannst.

**Lege offen, wenn es ein Bot ist.** An vielen Orten und als gute Praxis sollte ein Kunde wissen, dass er mit einem Chatbot spricht und nicht mit einer Person. Mach die Übergabe an einen Menschen leicht und klar.

**Respektiere die Privatsphäre.** Kundenanalyse nutzt personenbezogene Daten. Befolge die Regeln für deren Handhabung — die Grundlagen sind in [Kapitel 10 — Privatsphäre und DSGVO](ch10-privacy-and-gdpr.md). Sammle nur, was du brauchst, sag den Leuten, was du sammelst, und halte es sicher.

**Manipuliere nicht.** Personalisierung sollte Menschen helfen zu finden, was sie wollen, sie nicht in einen Kauf drängen, den sie bereuen werden. Vermeide „Dark Patterns" — Tricks, die Leute unter Druck setzen. Baue Vertrauen auf, keine Falle.

**Halte einen Menschen in der Schleife.** KI entwirft die E-Mail, die Anzeige, die Antwort. Ein Mensch prüft sie, bevor sie einen Kunden erreicht. Diese eine Regel verhindert die meisten Schäden.

## Zu vermeidende Fehler

**Mit KI spammen.** Die Macht des Werkzeugs nutzen, um mehr zu senden, als Leute wollen. Sende weniger, lass es zählen.

**Ungeprüfte KI-Texte verschicken.** Ein falscher Preis oder eine falsche Behauptung in einer KI-geschriebenen E-Mail beschädigt Vertrauen. Immer prüfen.

**Ein Chatbot, der nie übergibt.** Ein Bot, der blufft, statt an einen Menschen weiterzugeben, frustriert Kunden und verliert Verkäufe. Entwirf die Übergabe zuerst.

**Generischer, flacher Text.** KI-Text, der klingt wie der von jedem anderen. Bearbeite für deine Stimme, sonst wird er ignoriert.

**Dem Lead-Score zu sehr vertrauen.** Einen Score als Urteil behandeln statt als Hinweis. Nutze ihn, um Priorität zu setzen, nicht um Menschen zu ignorieren.

**Müll rein, Müll-Analyse raus.** Wenn deine CRM-Daten chaotisch sind, sind die Segmente und Churn-Markierungen falsch. Putze zuerst deine Daten.

**Kunden als Datenpunkte behandeln.** Analyse zum Manipulieren statt zum Dienen nutzen. Bleib auf der ethischen Seite.

**Keine Offenlegung von Bots.** Einen Chatbot vorgeben lassen, menschlich zu sein. Sei klar.

**Privatsphäre-Regeln ignorieren.** Personenbezogene Daten ohne Einwilligung oder Sicherheit nutzen. Befolge die DSGVO-Grundlagen.

**Aktivität mit Ergebnissen verwechseln.** Gesendete E-Mails zählen statt abgeschlossene Deals. Miss Ergebnisse, nicht Volumen.

**Die Basislinie überspringen.** Die Conversion vorher nicht messen, sodass du den Anstieg nicht beweisen kannst. Miss zuerst (siehe Kapitel 22).

**Die menschliche Note ganz ersetzen.** Kunden wollen für harte Probleme weiterhin eine Person. Behalte Menschen für die Wert-Gespräche.

## Praktische Übung

### 26.7 Übung: plane eine KI-gestützte Kampagne

Wähle eine Kampagne — eine E-Mail an frühere Kunden, ein Chatbot auf deiner Website oder ein Lead-Bewertungsdurchlauf — und plane sie von Ende zu Ende.

**Schritt 1 — Wähle den Job.** Wähle eines: Lead-Bewertung, eine E-Mail-Kampagne, ein Chatbot oder eine Kundenanalyse. Mach eines, nicht alle.

**Schritt 2 — Definiere das Ziel und die Kennzahl.** Was soll das erreichen? Anmeldungen, Antworten, gelöste Fragen, zurückgewonnene Kunden? Wähle eine Zahl zum Messen.

**Schritt 3 — Miss die Basislinie.** Was ist diese Zahl jetzt? Schreib sie auf. Ohne sie kannst du den Anstieg nicht beweisen.

**Schritt 4 — Sammle die Daten.** Für Bewertung: deine vergangenen Leads und welche abschlossen. Für E-Mail: deine Einwilligungsliste. Für den Chatbot: deine echten Kundenfragen und Antworten. Für Analyse: deine Kundenakten. Putze zuerst die Daten.

**Schritt 5 — Baue den KI-Teil.** Bewerte die Leads, entwirf die E-Mail, trainiere den Bot oder führe die Segmentierung durch. Lass KI die schwere Arbeit tun.

**Schritt 6 — Füge die menschliche Prüfung hinzu.** Lies jeden Entwurf. Prüfe jede faktische Behauptung. Entscheide die Übergaberegeln des Chatbots. Nichts geht hinaus ohne menschlichen Lesedurchgang.

**Schritt 7 — Prüfe Einwilligung und Privatsphäre.** Bestätige, dass du diese Leute anschreiben darfst und dass ihre Daten korrekt gehandhabt werden.

**Schritt 8 — Starte klein und miss.** Führe es zuerst in einer kleinen Gruppe durch. Vergleiche die Kennzahl mit der Basislinie. Wenn es funktioniert, skaliere hoch. Wenn nicht, lerne und passe an.

Mach eine Kampagne gut. Die Lektionen, die du lernst — über Ton, über Übergaben, worauf deine Kunden ansprechen — tragen in jede Kampagne danach.

## Checkliste

### 26.8 Vertriebs- und Marketing-Checkliste

Bevor du irgendeine KI-gestützte Vertriebs- oder Marketing-Aktivität startest, prüfe diese.

- [ ] **Du maßest die Basislinie** für die eine Kennzahl, die dich kümmert.
- [ ] **Ein Mensch prüft jede KI-geschriebene Botschaft**, bevor sie einen Kunden erreicht.
- [ ] **Jede faktische Behauptung ist geprüft** — Preis, Funktionen, Ergebnisse.
- [ ] **Du hast Einwilligung**, die Leute anzuschreiben, die du anschreibst.
- [ ] **Du achtest die Häufigkeit** — kein Spam, kein Übersenden.
- [ ] **Der Chatbot hat klare Übergaberegeln** an einen Menschen.
- [ ] **Der Chatbot ist auf deinen echten Fragen trainiert**, nicht auf generischen.
- [ ] **Du legst offen, dass es ein Bot ist**, wo erforderlich und als gute Praxis.
- [ ] **Du putzt deine Daten**, bevor du bewertest, segmentierst oder analysierst.
- [ ] **Du fütterst Ergebnisse zurück** in das Lead-Bewertungsmodell, damit es lernt.
- [ ] **Du behandelst den Lead-Score als Hinweis**, nicht als Urteil.
- [ ] **Du nutzt Analyse, um Kunden zu bedienen**, nicht um sie zu manipulieren.
- [ ] **Du folgst den Privatsphäre-Regeln** (DSGVO-Grundlagen, siehe Kapitel 10).
- [ ] **Du behältst Menschen für die harten Gespräche.**
- [ ] **Du misst Ergebnisse** (Deals, Antworten, Gewinne), nicht nur gesendetes Volumen.
- [ ] **Du startest erst klein** und skalierst nur, was sich beweist.

Wenn ein Kästchen leer ist, riskierst du Vertrauen. Fülle es, bevor du auf Senden drückst.

## Wichtige Kernpunkte

- KI hilft Vertrieb und Marketing durch Personalisierung im großen Maßstab — Leads bewerten, Botschaften zuschneiden, Fragen beantworten und gefährdete Kunden erkennen.
- Der mobilezone-Fall (eine Microsoft-Kundengeschichte) baute zwei Copilot-Studio-Agenten — Mia für Kunden, Supporto für interne IT — die über 1.600 Chats pro Monat bewältigten und die IT-Lösungszeit um etwa 50 % senkten.
- KI entwirft, ein Mensch prüft: verschicke nie eine KI-geschriebene Botschaft und lass einen Chatbot nicht bluffen, statt an eine Person zu übergeben.
- Saubere Daten sind das Fundament — chaotische Akten machen Lead-Scores, Segmente und Churn-Markierungen falsch.
- Nutze KI, um Kunden besser zu bedienen, nicht um sie zu spammen oder zu manipulieren; Einwilligung und Ehrlichkeit schützen das Vertrauen, auf dem du verkaufst.

<!-- BEGIN agentbridge-examples -->

## Teste es mit AgentBridge

So sieht dieselbe Aufgabe mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die du eingibst, um es zu bekommen.

### Aus einer Idee ein Angebot machen

![Ein strukturiertes Projektangebots-Dokument](../../assets/examples/project-proposal.png)
*Ein strukturiertes Projektangebots-Dokument*

**Was du fragst:** `Erstelle ein Projektangebot für einen kleinen Online-Shop: Ziele, was wir liefern, ein Zeitplan von 8 Wochen und ein Preis von 9.500 Euro.`

Der Agent baut ein Angebot mit dem Ziel des Kunden, deiner Lösung, den Ergebnissen, dem Zeitplan und dem Preis — alles in einem sauberen Layout, das aussieht, als hätte es einen ganzen Nachmittag gebraucht. Es dauerte eine Minute.

*Tipp: Füge dein Logo und einen Satz über frühere Ergebnisse hinzu, damit es persönlich wirkt.*

---

### Verfolge deinen Vertrieb

![Ein Vertriebs-Tracker mit Umsatz pro Kanal](../../assets/examples/sales-tracker.png)
*Ein Vertriebs-Tracker mit Umsatz pro Kanal*

**Was du fragst:** `Erstelle einen Vertriebs-Tracker mit Monat, Kanal und Umsatz, und ein Diagramm des Umsatzes nach Kanal.`

Der Agent baut den Tracker und das Diagramm. Füge beim Weitermachen Zeilen hinzu, oder hänge deine rohe Verkaufsliste an und bitte sie, das Blatt für dich auszufüllen.

*Tipp: Hänge einen chaotischen Export aus deinem Shop an und sag „putze das in einen Tracker" — das tut sie.*

---

### Ein Pitches-Deck aus einem Prompt

![Eine Präsentationsfolie, gebaut vom Agenten](../../assets/examples/pitch-deck.png)
*Eine Präsentationsfolie, gebaut vom Agenten*

**Was du fragst:** `Mach ein 6-Folien-Pitches-Deck für mein Liefer-Startup: Problem, Lösung, Markt, Modell, Traktion, Bitte.`

Der Agent gestaltet die Folien mit einem sauberen Look, einer klaren Idee pro Folie und der richtigen Reihenfolge für einen Pitch. Im Browser drückst du F11 für Vollbild und präsentierst.

*Tipp: Brauchst du eine echte .pptx zum Senden? Nutze /tools office-files und frag nach PowerPoint.*

---

### Ein Kundenverkaufs-Deck

![Eine kundengerichtete Verkaufs-Präsentationsfolie](../../assets/examples/sales-presentation.png)
*Eine kundengerichtete Verkaufs-Präsentationsfolie*

**Was du fragst:** `Erstelle ein Verkaufs-Deck, das unsere Arbeit mit Acme zusammenfasst und die nächste Phase vorschlägt.`

Der Agent baut ein fokussiertes Deck: bisherige Ergebnisse, was der Kunde gewann, und der vorgeschlagene nächste Schritt. Du feilst an den Zahlen und präsentierst mit Selbstvertrauen.

*Tipp: Hänge den Projektbericht an, und der Agent zieht die Höhepunkte in die Folien.*

---

### Ein höfliches Nachfassen

![Ein freundlicher Follow-up-E-Mail-Entwurf](../../assets/examples/follow-up.png)
*Ein freundlicher Follow-up-E-Mail-Entwurf*

**Was du fragst:** `Schreibe ein kurzes Follow-up an einen Kunden, der auf unser Angebot von letzter Woche nicht geantwortet hat.`

Der Agent schreibt einen leichten, höflichen Stupser, der ohne Druck erinnert. Du sendest ihn und hältst die Beziehung warm.

*Tipp: Ein geplantes Follow-up kann diese für dich senden, wenn keine Antwort eingetroffen ist.*

---

### Ein Kunden-Newsletter

![Ein versandbereiter Newsletter-Entwurf](../../assets/examples/newsletter.png)
*Ein versandbereiter Newsletter-Entwurf*

**Was du fragst:** `Schreibe einen monatlichen Newsletter für unsere Kunden: neue Artikel, ein Tipp und ein kleiner Rabattcode.`

Der Agent schreibt den Newsletter in deiner Stimme mit den Neuigkeiten, einem nützlichen Tipp und dem Angebot. Sende ihn, oder lass ihn einen nach Zeitplan vorbereiten.

*Tipp: Eine monatliche geplante Aufgabe kann den Newsletter jedes Mal zu deiner Prüfung entwerfen.*

---

### Aus einem Thema ein Podcast

![Eine abspielbereite Podcast-Folge](../../assets/examples/podcast-episode.png)
*Eine abspielbereite Podcast-Folge*

**Was du fragst:** `Erstelle eine 5-minütige Podcast-Folge darüber, warum kleine Läden online gehen sollten, in einem freundlichen Zwei-Stimmen-Stil.`

Der Agent schreibt das Skript und produziert eine Audio-Folge mit zwei Stimmen, versandbereit. Deine Nachricht, in Audioform, ohne Studio.

*Tipp: Gib ihr deine Kernpunkte, und sie formt sie zu einem natürlichen Gespräch.*

<!-- END agentbridge-examples -->
