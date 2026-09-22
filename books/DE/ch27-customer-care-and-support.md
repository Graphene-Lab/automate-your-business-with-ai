# Kapitel 27 — Kundenservice und Support

## In einfachen Worten

Kundenservice ist, wo ein Unternehmen beweist, dass es sich kümmert. Wenn etwas schiefgeht oder ein Kunde eine Frage hat, formt, wie schnell und wie gut du antwortest, ob er bleibt oder geht. Das Problem ist, dass Support voller derselben Fragen ist, die immer wieder gestellt werden, und ein kleines Team kann sie nicht alle sofort beantworten. KI hilft, indem sie die üblichen sofort beantwortet und die schwierigen schnell an die richtige Person weiterleitet.

Stell dir Support als eine Warteschlange vor. Jede Frage steht an und wartet auf eine Antwort. Je länger die Schlange, frustrierter werden die Leute. KI verkürzt die Schlange auf zwei Weisen: Sie beantwortet manche Fragen, bevor sie überhaupt einen Menschen erreichen, und sie sortiert den Rest, damit die richtige Person das richtige Problem zuerst sieht.

Dieses Kapitel behandelt vier Aufgaben: Chatbots und FAQs, die übliche Fragen beantworten, Ticket-Management, das Probleme sortiert und weiterleitet, Stimmungsanalyse, die liest, wie Kunden sich fühlen, und eine intelligente Wissensdatenbank, die alle Antworten an einem durchsuchbaren Ort hält.

Zuerst eine ehrliche Idee: Das Ziel von KI im Support ist nicht, Kunden vor deinen Leuten zu verstecken. Es ist, deine Leute von den repetitiven Fragen zu befreien, damit sie ihre Zeit den Fällen widmen können, die wirklich einen Menschen brauchen — dem wütenden Kunden, dem komplexen Problem, dem, der entscheidet, ob jemand zehn Jahre bleibt. KI bewältigt die Menge; Menschen bewältigt die Fürsorge. Die Methode zu beurteilen, ob es sich auszahlt, lebt in [Kapitel 16 — Ziele, Kosten und Return on Investment](ch16-goals-costs-and-return-on-investment.md); dieses Kapitel zeigt dir, was zu automatisieren ist und wie.

## Ein bisschen Geschichte

**1960er–1980er: das Callcenter.** Kundenservice bedeutete das Telefon. Ein Kunde rief an, wartete in der Warteschleife und sprach mit einem Agenten. Die ganze Disziplin drehte sich darum, genug Leute einzusetzen, um das Telefon zu beantworten. Es funktionierte, aber es war teuer, langsam und skalierte nur durch mehr Leute einstellen.

**1990er: E-Mail und das Ticket.** Support zog teilweise zu E-Mail, und das „Ticket" wurde geboren — jede Kundenanfrage wurde eine nummerierte Akte, die verfolgt, zugewiesen und geschlossen werden konnte. Tickets brachten Ordnung ins Chaos der Support-E-Mail. Werkzeuge wie frühe Helpdesk-Software machten es möglich, jede offene Anfrage an einem Ort zu sehen.

**2000er: die Wissensdatenbank und Self-Service.** Firmen erkannten, dass die meisten Support-Fragen dieselben wenigen Fragen waren. Sie bauten Wissensdatenbanken — durchsuchbare Bibliotheken von Antworten — damit Kunden sich selbst helfen konnten. Self-Service nahm etwas Last von Agenten, aber frühe Wissensdatenbanken waren schwer zu durchsuchen und verfehlten oft, was der Kunde brauchte.

**2010er: Chat und der regelbasierte Chatbot.** Live-Chat kam, und mit ihm der Chatbot. Frühe Chatbots waren regelbasiert: ein Entscheidungsbaum, der Schlüsselwörter mit vorgefertigten Antworten abglich. Sie waren billig, aber frustrierend — sie konnten nichts abseits des Skripts verstehen, und Kunden fühlten sich oft gefangen.

**Späte 2010er: KI liest Stimmung.** Maschinelles Lernen begann, den *Ton* einer Nachricht zu lesen — ob ein Kunde glücklich, frustriert oder wütend war — und konnte einen wütenden Kunden markieren, damit ein Senior-Agent zuerst antwortete. Stimmungsanalyse fügte dem Routing ein neues Signal hinzu: nicht nur was das Problem ist, sondern wie der Kunde darüber fühlt.

**2020er: große Sprachmodelle und agentischer Support.** Große Sprachmodelle — KI, trainiert auf riesigen Textmengen — machten Chatbots, die tatsächlich verstehen, was ein Kunde tippte, und in klarer Sprache antworten. Der neueste Schritt ist die agentische Plattform: KI, die nicht nur antwortet, sondern handelt — ein Ticket erstellen, einen Datensatz aktualisieren, einen Service terminieren. Das TridentCare-Beispiel unten ist genau das: KI, die die Planungsarbeit Ende-zu-Ende bewältigt, mit Menschen, die nur eingreifen, wenn Urteilsvermögen nötig ist.

Der Bogen: von Telefon-Warteschlangen, zu verfolgten Tickets, zu durchsuchbaren Antworten, zu Bots, die verstehen, zu Agenten, die handeln. Jeder Schritt verlagerte die Routinearbeit zu Software und ließ die menschlichen Agenten frei für die Fälle, die einen Menschen brauchen.

## Neugier

### 27.5 Die Disponentin, die das System die Arbeit machen ließ

In TridentCares alter Arbeitsweise wurde etwa die Hälfte aller Planung von Hand gemacht — eine Person, die die Anfrage eines Patienten mit einem Techniker, einer Zeit und einem Ort abglich. Nachdem das Unternehmen zu einer KI-gestützten Plattform wechselte, fiel manuelle Planung auf nur 4,3 %. Die Disponenten verschwanden nicht; sie wechselten die Jobs. Sie hörten auf, das Abgleichen selbst zu machen, und begannen, es zu beaufsichtigen, und griffen nur ein, wenn ein Fall wirklich menschliches Urteilsvermögen brauchte. Diese Verschiebung — vom Machen der Arbeit zum Beaufsichtigen der Arbeit — ist die stille Revolution in Support und Betrieb. Die ganze Geschichte ist unten.

## Ein echtes Geschäftsbeispiel

**TridentCare: 96 % Planungsautomatisierung mit einem KI-gestützten CRM.**

TridentCare ist der größte Anbieter von tragbaren medizinischen Diagnosediensten in den Vereinigten Staaten. Er schickt Techniker in Krankenhäuser, Pflegeheime und die Häuser von Patienten, um Tests wie Röntgen und Ultraschall durchzuführen — Dienste, die nicht warten können und über ein riesiges Gebiet zuverlässig geplant werden müssen. Diese Arbeit über hunderte Märkte von Hand zu planen, war langsam und schwer zu skalieren.

Laut einer ServiceNow-Pressemitteilung (getragen von Business Wire am 22. April 2026) wählte TridentCare die ServiceNow AI Platform, um seine Ende-zu-Ende-Operationen zu transformieren und manuelle Planung weitgehend durch Automatisierung zu ersetzen. Die berichteten Ergebnisse:

- **96 % Planungsautomatisierung über 127 Märkte.** Manuelle Planung tragbarer medizinischer Diagnosedienste fiel von **50 % auf nur 4,3 %**. Mit anderen Worten, das System bewältigt jetzt fast die gesamte Planung, und ein Mensch greift nur ein, wenn Urteilsvermögen es wirklich verlangt.
- **Patientenwartezeiten jenseits des Service-Level-Agreements (SLA) wurden um 57 % gesenkt.** Ein SLA ist die versprochene Serviceebene — zum Beispiel „ein Techniker kommt innerhalb von zwei Stunden". Weniger Patienten warteten länger als versprochen.
- **Die Effizienz im ersten Markt stieg um etwa 30 %.** Das Unternehmen bekam in den Märkten, wo es anfing, mehr erledigt.

Die Pressemitteilung beschrieb auch eine „Lead-to-Cash"-Transformation: Indem sie das Vertriebs-CRM direkt mit Felddaten verband, gewann TridentCare die Sichtbarkeit, genaue Serviceebenen festzulegen, zu sehen, wohin die Nachfrage sich verlagerte, und zu schärfen, wie es verkaufte.

Zwei Lektionen stechen hervor. Erstens wechselte die menschliche Rolle vom *Machen* zum *Beaufsichtigen*: Disponenten ließen das System die Routine bewältigen und griffen nur bei den Ausnahmen ein. Zweitens war der Gewinn nicht nur Geschwindigkeit — er war Zuverlässigkeit und Patientenversorgung. In einem Geschäft, wo ein verspäteter Techniker die Gesundheit eines Patienten betrifft, ist Automatisierung, die Wartezeiten senkt, nicht nur eine Kosteneinsparung; sie ist besserer Service.

Eine Anmerkung zur Quelle: Die obigen Zahlen stammen aus ServiceNow veröffentlichter Ankündigung. Behandle sie als TridentCares berichtete Ergebnisse; deine eigenen Zahlen hängen von deiner Operation und Menge ab.

## Wie man es macht

### 27.1 Chatbots und FAQs

Ein Chatbot auf deiner Website oder App kann die üblichen Support-Fragen sofort beantworten, damit Kunden nicht auf eine Person warten müssen. Eine FAQ-Seite (Frequently Asked Questions) ist die einfachere Cousine: eine Liste üblicher Fragen mit geschriebenen Antworten.

**Was ein Chatbot bewältigen sollte.** Die repetitiven, risikoarmen Fragen: „Was sind eure Öffnungszeiten?", „Wie setze ich mein Passwort zurück?", „Wo ist meine Bestellung?", „Was ist eure Rückgaberichtlinie?" Das sind die Fragen, die den größten Teil der Zeit eines Support-Teams fressen und kein Urteilsvermögen brauchen. Lass den Bot sie beantworten.

**Moderne Bots verstehen Sprache.** Anders als die alten Menü-Bots versteht ein Chatbot, der auf einem großen Sprachmodell gebaut ist, was ein Kunde tippt, und antwortet in klaren Worten. Er kann „Ich kann mich nicht einloggen, es sagt falsches Passwort" bewältigen, ohne dass der Kunde aus einer Liste wählt.

**Die Übergabe ist alles.** Ein Chatbot, der nicht antworten kann, muss das Gespräch an einen Menschen weitergeben, mit intaktem Kontext — der Mensch sollte sehen, was der Kunde schon sagte, nicht bei null anfangen. Entscheide die Übergaberegeln, bevor du baust: wann der Bot unsicher ist, wann der Kunde nach einer Person fragt, wann das Thema sensibel ist. Ein Bot, der seine Grenzen kennt, wird vertraut; einer, der blufft, nicht.

**Halte die FAQ lebendig.** Eine FAQ-Seite, die veraltet ist, ist schlimmer als keine — sie gibt falsche Antworten zuversichtlich. Prüfe sie regelmäßig und aktualisiere sie, wenn sich deine Produkte und Richtlinien ändern. Der Chatbot und die FAQ sollten aus derselben Quelle der Wahrheit schöpfen (siehe die Wissensdatenbank unten).

**Messe Lösung und Scheitern.** Verfolge, wie viele Fragen der Bot allein löst und wie viele er übergibt. Die Misserfolge sagen dir, was du ihm als Nächstes beibringen sollst. (Dieselbe Chatbot-Technologie, auf Vertrieb statt Support angewendet, ist in [Kapitel 26 — Vertrieb und Marketing](ch26-sales-and-marketing.md) behandelt.)

### 27.2 Ticket-Management

Ein *Ticket* ist eine nummerierte Akte einer Kundenanfrage. Ticket-Management bedeutet, jede Anfrage zu sortieren, sie der richtigen Person zuzuweisen, ihren Fortschritt zu verfolgen und sie zu schließen, wenn gelöst. Wenn die Menge hoch ist, ist gutes Ticket-Management der Unterschied zwischen einem organisierten Support-Team und einem chaotischen.

**KI sortiert und leitet weiter.** Statt dass eine Person jedes Ticket liest und entscheidet, wer es handhaben soll, liest KI das Ticket und leitet es automatisch an das richtige Team oder den richtigen Agenten weiter, basierend auf dem Thema, der Geschichte des Kunden und der Dringlichkeit. Das spart den Triage-Schritt, der reiner Overhead ist.

**Nach Dringlichkeit und Gefühl priorisieren.** KI kann Tickets so rangieren, dass die dringendsten und verstimmtesten Kunden zuerst gesehen werden. Ein Kunde, dessen Service völlig ausgefallen ist, oder der klar wütend ist, sollte nicht hinter einer Routinefrage warten. Dringlichkeit mit Stimmung (siehe unten) zu kombinieren, macht die Warteschlange klüger.

**Die Antwort vorschlagen.** KI kann ein Ticket lesen und eine Antwort vorschlagen, oder den Agenten auf den Wissensdatenbank-Artikel verweisen, der es löst. Der Agent prüft und sendet, statt von Grund auf zu schreiben. Das senkt die Bearbeitungszeit bei jedem Ticket.

**Die Routineaktionen automatisieren.** Manche Tickets brauchen eine einfache Aktion — ein Passwort zurücksetzen, ein Dokument erneut senden, eine Adresse aktualisieren. KI kann diese automatisch tun und das Ticket schließen, oder die Aktion für einen Menschen zum Genehmigen entwerfen. Die Routinearbeit verschwindet aus der Warteschlange.

**Halte die Audit-Spur.** Jedes Ticket sollte aufzeichnen, was geschah, wer was tat, und wann. Das zählt für Qualitätsprüfung, für Schulung und für Verantwortlichkeit. Gute Ticketing-Werkzeuge produzieren das automatisch; bestätige, dass deins es tut.

### 27.3 Stimmungsanalyse

Stimmungsanalyse bedeutet, KI zu nutzen, um das *Gefühl* hinter einer Nachricht zu lesen — ist der Kunde glücklich, neutral, frustriert oder wütend? Sie verwandelt rohen Text in ein emotionales Signal, das du handeln kannst.

**Warum es zählt.** Ein wütender Kunde, der in einer normalen Warteschlange wartet, mag abwandern, bevor ihn jemand sieht. Wenn KI die Wut früh markiert, kann ein Senior-Agent schnell antworten und einen schlechten Moment in einen guten verwandeln. Stimmung ist ein Routing-Signal, das reine Themen-Abgleichung verfehlt.

**Wie es funktioniert.** Die KI liest die Worte und den Ton einer Nachricht und weist eine Stimmung zu — positiv, neutral, negativ — oder einen Score. Sie lernt aus vielen Beispielen von Nachrichten, die von Menschen markiert wurden. Sie ist nicht perfekt, aber gut genug, um die klar verstimmten Kunden zu markieren.

**Nutze sie zum Priorisieren, nicht zum Beurteilen.** Speise Stimmung in die Ticket-Warteschlange ein, damit die negativsten Nachrichten nach oben steigen. Benutze sie nicht, um Agenten zu bewerten oder zu bestrafen, und behandle eine einzelne Stimmungsablesung nicht als das letzte Wort über die Gefühle eines Kunden. Sie ist ein Hinweis, Acht zu geben, kein Urteil.

**Beobachte Trends über die Zeit.** Stimmung ist am nützlichsten als Trend. Wenn negative Stimmung über alle Tickets hinweg Monat für Monat steigt, ist etwas falsch mit deinem Produkt oder Service, noch bevor Kunden eine formale Beschwerde schreiben. Verfolge die durchschnittliche Stimmung und beobachte die Richtung.

**Bedenke die Grenzen.** Sarkasmus, Ironie und kulturelle Unterschiede können die Stimmungsanalyse täuschen. Ein „großartig, noch ein Problem" liest sich für ein naives Modell positiv. Nutze Stimmung als ein Signal unter vielen, und lass das Urteilsvermögen eines Menschen es überstimmen.

### 27.4 Intelligente Wissensdatenbank

Eine Wissensdatenbank ist eine durchsuchbare Bibliothek von Antworten auf übliche Fragen. Eine *intelligente* Wissensdatenbank nutzt KI, um es weit leichter zu machen, die richtige Antwort zu finden — und die Antworten aktuell zu halten.

**Suche, die die Frage versteht.** Statt exakter Schlüsselwörter abzugleichen, versteht eine KI-Wissensdatenbank, was der Kunde meint, und gibt den relevanten Artikel zurück, auch wenn die Worte sich unterscheiden. „Meine Karte wurde doppelt belastet" findet den Doppelzahlungs-Artikel, nicht nur Artikel, die genau diese Worte enthalten.

**KI schreibt und aktualisiert Artikel.** Wenn ein Support-Agent ein neues Problem löst, kann KI aus dem gelösten Ticket einen Wissensdatenbank-Artikel entwerfen, damit die Antwort fürs nächste Mal festgehalten ist. Das verwandelt jedes gelöste Problem in eine wiederverwendbare Antwort, statt es im Kopf eines Agenten eingeschlossen zu lassen.

**Eine Quelle der Wahrheit.** Dein Chatbot, deine FAQ-Seite und deine Agenten sollten alle aus derselben Wissensdatenbank schöpfen. Wenn du eine Stelle aktualisierst, bekommt jeder Kanal die richtige Antwort. Wenn du sie getrennt pflegst, driften sie auseinander und geben widersprüchliche Antworten, was Vertrauen zerstört.

**Die Lücken aufspüren.** KI kann sehen, welche Fragen Kunden stellen, die keinen Artikel haben. Diese Lücken sind eine To-do-Liste: Schreibe die fehlenden Antworten, und der Bot und die Suche werden besser. Die Wissensdatenbank verbessert sich selbst, indem sie dir zeigt, was fehlt.

**Halte sie frisch.** Eine abgestandene Wissensdatenbank gibt falsche Antworten zuversichtlich. Prüfe Artikel regelmäßig, pensioniere die veralteten, und lass die KI Artikel markieren, die vielleicht ein Update brauchen, weil sich das Produkt geändert hat. Frische ist der ganze Wert einer Wissensdatenbank.

## Ethik und Verantwortung

Support ist, wo Vertrauen gewonnen oder verloren wird, also sind die ethischen Einsätze hoch.

**Lass nie einen Bot einen Menschen verstecken.** Kunden haben das Recht, eine Person zu erreichen. Ein Chatbot, der den Weg zu einem Menschen blockiert, ist ein feindliches Design. Mach die Übergabe leicht, klar und immer verfügbar.

**Lege offen, dass es ein Bot ist.** Ein Kunde sollte wissen, dass er mit KI spricht und nicht mit einer Person. Das ist überall gute Praxis und an manchen Orten eine gesetzliche Anforderung.

**Ignoriere keinen wütenden Kunden wegen eines Modellfehlers.** Wenn die Stimmungsanalyse einen wütenden Kunden verfehlt, muss die menschliche Warteschlange ihn trotzdem fangen. Stimmung ist ein Helfer, kein Torwächter. Lass nie einen Modellfehler eine echte Beschwerde begraben.

**Schütze Kundendaten.** Support-Tickets enthalten persönliche, manchmal sensible Informationen. Behandle sie sorgfältig und befolge die Datenschutzregeln — die Grundlagen sind in [Kapitel 10 — Privatsphäre und DSGVO](ch10-privacy-and-gdpr.md). Füge keine sensiblen Kundendaten in öffentliche KI-Werkzeuge ein, ohne die Sicherheitsimplikationen zu prüfen (siehe [Kapitel 6 — Cybersicherheit im Zeitalter der KI](ch06-cybersecurity-in-the-ai-era.md)).

**Halte einen Menschen verantwortlich.** KI kann eine Antwort entwerfen oder ein Ticket weiterleiten, aber ein Mensch besitzt das Ergebnis. Wenn etwas schiefgeht, muss eine Person verantwortlich sein, keine Blackbox.

**Nutze Stimmung zum Helfen, nicht zum Manipulieren.** Die Gefühle eines Kunden zu lesen, sollte dir helfen, ihn besser zu bedienen, nicht seine Frustration auszunutzen, um hochzuverkaufen oder ihn unter Druck zu setzen. Bleib auf der Seite der Fürsorge.

**Benutze Support-Daten nicht, um Agenten zu überwachen.** Ticket-Metriken zu verfolgen, um den Prozess zu verbessern, ist in Ordnung. Dieselben Daten zu nutzen, um einzelne Agenten zu bespitzeln und zu bestrafen, vergiftet Vertrauen. Miss die Arbeit, nicht die Person.

## Zu vermeidende Fehler

**Ein Bot, der den Menschen blockiert.** Der schlimmste Support-Fehler. Mach immer die Übergabe leicht.

**Kein Übergabe-Kontext.** Einen Kunden an einen Menschen übergeben, der ihn dann bittet, alles zu wiederholen. Trage den Kontext hinüber.

**Bluffender Chatbot.** Ein Bot, der rät, statt zuzugeben, dass er es nicht weiß. Bring ihm bei, zu übergeben, wenn unsicher.

**Abgestandene Wissensdatenbank.** Veraltete Artikel, die falsche Antworten zuversichtlich geben. Regelmäßig prüfen und aktualisieren.

**Getrennte Quellen der Wahrheit.** Chatbot, FAQ und Agenten mit je eigenen Antworten, die auseinander driften. Nutze eine Wissensdatenbank.

**Stimmung als Urteil.** Die Stimmungsablesung eines Modells als das letzte Wort über einen Kunden behandeln. Sie ist ein Hinweis, kein Urteil.

**Den wütenden Kunden verfehlen.** Einen Modellfehler ein verstimmten Kunden begraben lassen. Die menschliche Warteschlange muss ihn trotzdem fangen.

**Einen schlechten Prozess automatisieren.** Wenn dein Support-Flow kaputt ist, macht Automatisierung einen schnelleren kaputten Flow. Repariere erst den Prozess.

**Sensible Daten lecken.** Kundendaten in unsichere KI-Werkzeuge stecken. Erst Sicherheit und Privatsphäre prüfen.

**Keine Audit-Spur.** Tickets, die nicht zeigen können, was geschah. Halte das Protokoll.

**Abwehr mit Erfolg verwechseln.** Zählen, wie viele Tickets der Bot „bewältigte", statt ob der Kunde tatsächlich zufrieden war. Miss Lösung und Zufriedenheit, nicht Abwehr.

**Die Baseline überspringen.** Antwortzeit oder Zufriedenheit vorher nicht messen, sodass du die Verbesserung nicht beweisen kannst. Erst messen (siehe Kapitel 22).

## Praktische Übung

### 27.7 Übung: Gestalte deine Support-Automatisierung

Wähle einen Support-Kanal und plane seine KI-Unterstützung Ende-zu-Ende.

**Schritt 1 — Wähle den Kanal.** Wähle einen: einen Website-Chatbot, deine Ticket-Warteschlange oder deine Wissensdatenbank. Mache einen, nicht alle.

**Schritt 2 — Definiere das Ziel und die Metrik.** Schnellere Antwort? Höhere Self-Service-Lösung? Weniger wütende Kunden? Wähle eine Zahl zum Messen.

**Schritt 3 — Messe die Baseline.** Was ist diese Zahl jetzt? Durchschnittliche Antwortzeit, Lösungsrate, Zufriedenheits-Score. Schreib sie auf.

**Schritt 4 — Liste die üblichen Fragen.** Zieh den letzten Monat Tickets und finde die Top 10 wiederholten Fragen. Das sind die, die der Bot und die Wissensdatenbank bewältigen sollten.

**Schritt 5 — Schreibe die Antworten.** Für jede übliche Frage schreibe die Antwort, die du willst. Das wird deine Wissensdatenbank und das Training deines Bots.

**Schritt 6 — Setze die Übergaberegeln.** Entscheide genau, wann der Bot an einen Menschen übergibt: unsicher, erbeten, sensibel. Schreib die Regeln auf.

**Schritt 7 — Füge Stimmungs-Routing hinzu.** Wenn dein Werkzeug es unterstützt, stelle negativ-stimmungs-Tickets so ein, dass sie nach oben in der Warteschlange steigen.

**Schritt 8 — Starte klein und messen.** Lauf es zuerst auf einem Teil des Traffics. Vergleiche die Metrik mit der Baseline. Skaliere nur, was beweist, dass es tatsächlich löst, nicht nur abwehrt.

Mache einen Kanal gut. Die Liste üblicher Fragen, die du in Schritt 4 aufbaust, ist wertvoll für sich — sie zeigt dir genau, was deine Kunden verwirrt, was selbst über Support hinaus nützlich ist.

## Checkliste

### 27.8 Kundenservice-und-Support-Checkliste

Bevor du KI im Support startest, prüfe diese.

- [ ] **Du hast die Baseline gemessen** — Antwortzeit, Lösungsrate, Zufriedenheit.
- [ ] **Der Chatbot übergibt leicht an einen Menschen**, mit vollem Kontext.
- [ ] **Du legst offen, dass es ein Bot ist**, wo erforderlich und als gute Praxis.
- [ ] **Der Bot ist auf deinen echten üblichen Fragen trainiert**, nicht generischen.
- [ ] **Der Bot gibt zu, wenn er es nicht weiß**, statt zu bluffen.
- [ ] **Tickets werden automatisch weitergeleitet** an das richtige Team oder den richtigen Agenten.
- [ ] **Dringende und verstimmte Kunden werden priorisiert** in der Warteschlange.
- [ ] **Stimmung ist ein Hinweis, Acht zu geben**, kein Urteil über den Kunden.
- [ ] **Du hast eine Wissensdatenbank**, die den Bot, die FAQ und die Agenten speist.
- [ ] **Die Wissensdatenbank wird frisch gehalten** und regelmäßig geprüft.
- [ ] **KI entwirft Antworten und Artikel** aus gelösten Tickets, um Wissen festzuhalten.
- [ ] **Du hältst eine Audit-Spur** bei jedem Ticket.
- [ ] **Kundendaten werden sicher behandelt** und folgen den Datenschutzregeln (siehe Kapitel 10).
- [ ] **Ein Mensch besitzt das Ergebnis** — keine Blackbox-Verantwortlichkeit.
- [ ] **Du misst Lösung und Zufriedenheit**, nicht nur Abwehr.
- [ ] **Du reparierst den Support-Prozess, bevor du ihn automatisierst.**

Wenn eine Box leer ist, mag ein Kunde es spüren. Fülle sie, bevor du KI für dich antworten lässt.

## Das Wichtigste

- KI im Support verkürzt die Warteschlange, indem sie übliche Fragen sofort beantwortet und die schwierigen schnell an die richtige Person weiterleitet.
- Der TridentCare-Fall (eine ServiceNow-Ankündigung) erreichte 96 % Planungsautomatisierung über 127 Märkte, senkte manuelle Planung von 50 % auf 4,3 % und Patientenwartezeiten jenseits SLA um 57 %, mit Menschen, die beaufsichtigten statt die Arbeit zu machen.
- Die wichtigste Funktion des Chatbots ist eine saubere Übergabe an einen Menschen mit vollem Kontext — lass nie einen Bot eine Person blockieren.
- Eine frische, geteilte Wissensdatenbank sollte den Bot, die FAQ und deine Agenten speisen; Stimmungsanalyse sollte die Warteschlange priorisieren, nicht den Kunden beurteilen.
- Miss Lösung und Zufriedenheit, nicht Abwehr, und halte einen Menschen für jedes Ergebnis verantwortlich.

<!-- BEGIN agentbridge-examples -->

## Probier es mit AgentBridge

So sieht dieselbe Arbeit mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die du tippst, um es zu bekommen.

### Eine E-Mail in deinem Ton beantworten

![Eine entworfene E-Mail-Antwort, bereit zum Senden](../../assets/examples/quick-reply.png)
*Eine entworfene E-Mail-Antwort, bereit zum Senden*

**Was du eingibst:** `Antworte auf diesen Kunden, danke ihm und bestätige, dass wir morgen versenden: [E-Mail einfügen]`

Der Agent schreibt eine freundliche, professionelle Antwort, die wie du klingt. Du liest sie einmal, drückst Senden, und machst weiter.

*Tipp: Richte deine Mail einmal mit /email ein. Danach funktionieren Lesen und Senden aus dem Chat.*

---

### Deinen Posteingang aufholen

![Eine kurze Zusammenfassung des Posteingangs mit den dringenden Punkten](../../assets/examples/inbox-summary.png)
*Eine kurze Zusammenfassung des Posteingangs mit den dringenden Punkten*

**Was du eingibst:** `Fasse meine ungelesenen E-Mails zusammen und sag mir, welche heute eine Antwort brauchen.`

Der Agent liest deine ungelesene Mail und gibt dir eine kurze Liste: was dringend ist, was warten kann, und was du ignorieren kannst. Du packst die echten Prioritäten zuerst an.

*Tipp: Eine Morgen-Zusammenfassung kann geplant werden, damit das mit deinem Kaffee auf dich wartet.*

---

### Einen Kunden schnell finden

![Ein auf Anfrage abgerufener Kundendatensatz](../../assets/examples/customer-lookup.png)
*Ein auf Anfrage abgerufener Kundendatensatz*

**Was du eingibst:** `Finde die Kundin Maria Rossi und zeig ihren Kontakt und ihre letzte Bestellung.`

Der Agent findet den Kunden und zeigt die Kontaktdaten und die letzte Bestellung, sodass du helfen kannst, ohne ihn in die Warteschleife zu legen.

*Tipp: Frag nach den letzten drei Bestellungen, wenn du das ganze Bild willst.*

<!-- END agentbridge-examples -->
