# Kapitel 35 — Gesundheitswesen, Bildung und öffentliche Stellen

*Dieses Kapitel ist ein repräsentatives Composite. Es ist keine einzige reale Organisation. Es kombiniert die üblichen Muster, die wir in kleinen Kliniken, Schulen und öffentlichen Ämtern sehen, die KI für die Verwaltung einführen. Alle Zahlen sind illustrativ — sie zeigen die Form der Entscheidung, kein Versprechen. Ersetze sie durch deine eigenen. Die Regeln für regulierte Daten stehen in [Kapitel 10 — Datenschutz und DSGVO](ch10-privacy-and-gdpr.md) und [Kapitel 5 — Regeln und rechtliche Verantwortung](ch05-rules-and-legal-responsibility.md); dieses Kapitel zeigt, wie sich diese Regeln in der Praxis auswirken.*

## Kontext

Stell dir eine kleine kommunale Arztpraxis vor. Wir nennen sie **Riverside Family Clinic**. Sie hat vier Hausärzte, zwei Krankenschwestern und eine Empfangstheke mit drei Verwaltungsmitarbeitern. Sie betreut ein paar tausend Patienten in einer Stadt.

Der Tag der Praxis läuft über die Empfangstheke. Das Telefon klingelt ständig. Leute rufen an, um einen Termin zu buchen, einen zu verschieben, zu fragen, was sie mitbringen sollen, nach einer Überweisung zu fragen, zu fragen, wann ein Ergebnis fertig ist. Die drei Verwaltungsmitarbeiter verbringen den größten Teil ihres Tages am Telefon und mit Papier. Überweisungsbriefe kommen per Post an und müssen gelesen, abgelegt und an den richtigen Arzt weitergeleitet werden. Formulare müssen geprüft werden, bevor ein Patient gesehen wird. Währenddessen beenden die Ärzte jeden Besuch und verbringen dann Zeit damit, die Notizen zu schreiben — eine Aufgabe, die sich auftürmt, bis ein Teil davon spät in der Nacht erledigt wird.

Stell dir jetzt zwei weitere Orte mit derselben Form vor. Eine **Grundschule**, in der das Büro jeden Tag dieselben Fragen von Eltern beantwortet, die Aufnahmedokumente bearbeitet und Stundenpläne jongliert. Ein **Rathaus-Amt**, in dem Mitarbeiter Anträge von Bürgern bearbeiten — eine Genehmigung, einen Leistungsantrag, eine Registrierung —, jeder ein Stapel Formulare und Dokumente, die gelesen, geprüft und weiterbewegt werden müssen.

Drei verschiedene Orte. Dasselbe Muster: ein kleines Team, begraben unter Terminplanung, Dokumenten und wiederholten Fragen, während die ausgebildeten Menschen — Ärzte, Lehrer, Fallbearbeiter — Zeit mit Papierkram verbringen statt mit der Arbeit, für die sie ausgebildet wurden.

Was diese drei besonders macht, sind die Daten. Eine Klinik hält **Gesundheitsdaten**. Eine Schule hält Daten über Kinder. Ein öffentliches Amt hält Daten über Bürger und ihre Ansprüche. Das sind keine gewöhnlichen Aufzeichnungen. Sie gehören zu den am besten geschützten Arten personenbezogener Daten. Diese eine Tatsache setzt eine höhere Latte für alles in diesem Kapitel.

## Das Problem

Die Lecks sind die bekannten, aber die Kosten, wenn es schiefgeht, sind höher.

**Überlastung an der Theke.** Die Telefonwarteschlange ist der Flaschenhals der Klinik. Mitarbeiter verbringen Stunden mit wiederholten Fragen — Öffnungszeiten, was mitzubringen ist, wie man umbucht —, während echte dringende Anrufe warten. Lange Wartezeiten frustrieren Patienten und brennen das Personal aus.

**Nichterscheinen.** Wenn Patienten einen Termin vergessen, ist der Slot verschwendet, und jemand anderes hätte ihn haben können. In einer belebten Klinik bedeutet eine hohe Nichterscheinens-Quote, dass echte Patienten länger auf Versorgung warten.

**Dokumentationslast.** Nach jedem Besuch schreibt der Arzt Notizen. Das ist notwendig und es ist schwer. Kliniker überall berichten, dass sie einen großen Teil ihres Tages mit Aufzeichnungen statt mit Patienten verbringen. Es ist ein bekannter Treiber von Stress und Ausbrennen. Die Arbeit ist sorgfältig, aber repetitiv.

**Dokumentenbehandlung.** Überweisungsbriefe, Formulare und Ergebnisse kommen in vielen Formaten. Jemand muss jeden lesen, die wichtigsten Fakten herausziehen, ablegen und an die richtige Person weiterleiten. Verpasst man ein Dokument, wartet ein Patient.

**Wiederholte Fragen von Bürgern und Eltern.** In der Schule und im Amtsbüro kommen dieselben Fragen immer und immer wieder, in vielen Sprachen, und die Antwort ist immer dieselbe. Sie zu beantworten ist einfach, aber es verbraucht das Büro.

Über all dem liegt die Regel, dass diese Daten **besondere Kategorie**-Daten sind. Nach der DSGVO erhalten Gesundheitsdaten und Daten über Kinder zusätzlichen Schutz. Der EU AI Act fügt mehr hinzu: Systeme, die in Medizinprodukten oder auf Weise eingesetzt werden, die die Rechte von Menschen betreffen, werden als höheres Risiko behandelt und tragen schwerere Pflichten. Die Details stehen in [Kapitel 10](ch10-privacy-and-gdpr.md) und [Kapitel 5](ch05-rules-and-legal-responsibility.md). Der Punkt hier ist einfach: In diesen Umgebungen sind Datenschutz und Compliance keine Box, die man am Ende ankreuzt. Sie formen jede Wahl von Anfang an.

## Die Lösung

Riverside geht die Verwaltungslast nach Sicherheitsreihenfolge an. Die Regel ist dieselbe wie in einer Anwaltskanzlei: Beginne dort, wo ein Fehler billig ist und die Daten am wenigsten sensibel sind, und bewege dich zur sensiblen Arbeit erst, wenn die Werkzeuge vertrauenswürdig sind. Und in einer Klinik wird die sensibelste Arbeit — die klinische Beurteilung — überhaupt nie automatisiert.

**KI-Terminplanung und Erinnerungen.** Ein Chatbot auf der Website und ein Telefonsystem erledigen routinehafte Buchungen: buchen, verschieben, stornieren. Sie beantworten die wiederholten Fragen sofort. Automatische Erinnerungen gehen vor jedem Termin raus, was das Nichterscheinen senkt. Die Mitarbeiter an der Theke werden frei für die Anrufe, die einen Menschen brauchen — ein besorgter Patient, ein komplexer Fall. Die Chatbot-Technologie ist dieselbe wie in [Kapitel 27 — Kundenbetreuung und Support](ch27-customer-care-and-support.md).

**Umgebende Dokumentation, die entwirft, der Arzt unterschreibt.** Für einen Besuch hört ein Werkzeug dem Gespräch zu (mit der klaren Zustimmung des Patienten) und entwirft danach die klinische Notiz. Der Arzt prüft sie, korrigiert, was falsch ist, und unterschreibt sie. Der Arzt ist voll verantwortlich für die Notiz; das Werkzeug entfernt nur das Tippen. Das ist dasselbe „Maschine entwirft, Mensch prüft"-Muster, das der Elanco-Fall in [Kapitel 25 — Verwaltung und Finanzen](ch25-administration-and-finance.md) zeigt. Das Werkzeug diagnostiziert nicht. Es schreibt auf, was gesagt wurde, damit der Arzt es prüfen kann.

**Dokumenten-Routing.** Ein Werkzeug liest eingehende Überweisungsbriefe und Formulare, extrahiert die wichtigsten Fakten — den Patienten, die Anfrage, die Dringlichkeit — und legt sie ab und leitet sie weiter. Eine Person prüft weiterhin den Stapel, aber das Sortieren ist erledigt, sodass nichts ungelesen liegt.

**Ein Fragen-Assistent für Bürger und Eltern.** In der Schule und im Amtsbüro beantwortet ein Chatbot die wiederholten Fragen in klarer Sprache und in mehreren Sprachen, zu jeder Uhrzeit. Ein Elternteil, der fragt „welche Unterlagen brauche ich für die Aufnahme?", oder ein Bürger, der fragt „wie beantrage ich diese Genehmigung?", bekommt sofort eine Antwort. Die Bürokräfte bearbeiten nur die Fragen, die der Bot nicht kann.

Beachte die Linie, die sich nie bewegt. Die KI bucht, erinnert, entwirft, extrahiert und antwortet. Ein Arzt unterschreibt die klinische Notiz. Ein Fallbearbeiter entscheidet über einen Antrag. Ein Lehrer trifft die pädagogische Entscheidung. In diesen Umgebungen berührt die KI die Verwaltung um die Entscheidung herum, nie die Entscheidung selbst.

## Die Werkzeuge

Die Werkzeuge sind gewöhnlich, aber sie werden unter einem viel strengeren Regelwerk eingesetzt.

- **Ein Terminplanungs- und Erinnerungssystem** mit Chatbot und Telefonbehandlung für routinehafte Buchungen.
- **Ein Werkzeug zur umgebenden Dokumentation**, das Besuchsnotizen aus einem aufgezeichneten Gespräch entwirft, damit der Kliniker es prüft und unterschreibt.
- **Ein Dokument-Extraktionswerkzeug**, das Briefe und Formulare liest und weiterleitet.
- **Ein Fragen-Chatbot** für Eltern und Bürger, der in mehreren Sprachen arbeitet.

Wie man diese Werkzeuge auswählt, ohne sich von einer Demo blenden zu lassen, steht in [Kapitel 17 — Werkzeuge wählen, ohne sich täuschen zu lassen](ch17-choosing-tools-without-being-fooled.md). Wie man sie mit dem Patientensystem der Klinik oder dem Fallssystem des Büros verbindet, steht in [Kapitel 19 — KI mit Systemen verbinden, die du bereits nutzt](ch19-connecting-ai-to-systems-you-already-use.md).

**Die Compliance-Latte ist hier die ganze Geschichte.** Gesundheitsdaten und Kinderdaten können nicht in einen öffentlichen Chatbot eingefügt werden. Diese Organisationen müssen Werkzeuge nutzen, die die Daten geschützt halten: ein Geschäftsdienst mit einem klaren Vertrag ohne Training, ohne Teilen und einer Auftragsverarbeitungsvereinbarung, oder ein Modell, das auf ihren eigenen Maschinen oder in einer kontrollierten Cloud innerhalb der Region läuft. Selbst-Hosting wird erklärt in [Kapitel 8 — Selbst-Hosting: Halte deine Daten unter Kontrolle](ch08-self-hosting-keep-your-data-under-control.md). Die Gefahr, dass Mitarbeiter still sensible Daten in öffentliche Werkzeuge einfügen — Schatten-KI — ist das Thema von [Kapitel 9 — Drittdienste und Schatten-KI](ch09-third-party-services-and-shadow-ai.md). Die Daten im Land oder in der Region zu halten, statt im Ausland, ist die Souveränitätsfrage in [Kapitel 11 — Digitale Souveränität](ch11-digital-sovereignty.md). Und die rechtlichen Pflichten für diese Datenkategorie stehen in [Kapitel 10](ch10-privacy-and-gdpr.md) und [Kapitel 5](ch05-rules-and-legal-responsibility.md).

Daraus folgen zwei praktische Regeln. Erstens **Datenminimierung**: Erhebe und verarbeite nur, was nötig ist. Ein Terminplanungs-Bot braucht nicht die vollständige Krankengeschichte eines Patienten. Zweitens **Protokollpfad**: Jede Aktion, die die KI unternimmt, und jede menschliche Prüfung müssen protokolliert werden, damit die Organisation später zeigen kann, wer was getan hat.

## Die Kosten

Hier ist ein illustratives Budget für das erste Jahr für eine Klinik wie Riverside. Das sind erfundene Zahlen, um die Form zu zeigen. Nutze deine eigenen. Die Compliance-Arbeit macht diese Umgebungen teurer in der Einrichtung als ein Geschäft.

**Direkte Kosten.**
- Terminplanungs- und Erinnerungssystem: etwa 6.000 € pro Jahr.
- Werkzeug zur umgebenden Dokumentation (konform, mit Auftragsverarbeitungsvereinbarung): etwa 14.400 € pro Jahr.
- Dokument-Extraktion und Routing: etwa 7.200 € pro Jahr.
- Fragen-Chatbot für Patienten: etwa 3.600 € pro Jahr.
- Einrichtung, Integration und die Compliance-Arbeit (Folgenabschätzung für den Datenschutz, Anbieterprüfung, Sicherheitsüberprüfung): etwa 18.000 € einmalig.
- Schulung der Mitarbeiter: etwa 5.000 € einmalig.

Gesamt im ersten Jahr: rund **54.200 €**. In den stabilen Jahren danach kommen die wiederkehrenden Abos auf etwa **31.200 €**.

**Indirekte Kosten.**
- Kliniker verbringen Zeit damit, jede entworfene Notiz zu prüfen. Das ist das Sicherheitsnetz, und es muss bleiben.
- Der Compliance-Aufwand: eine Folgenabschätzung für den Datenschutz ist nicht kostenlos, und sie muss vor dem Livegang gemacht werden, nicht danach.
- Das Lern-Tief, während sich Mitarbeiter und sogar Patienten anpassen.
- Die Kosten eines Fehlers, wenn einem Entwurf ohne Prüfung vertraut wird — in einer Klinik kann das einem Patienten schaden, was weit schlimmer ist als ein verlorener Verkauf.
- Laufende Überwachung, damit die Werkzeuge bei sich ändernden Regeln konform bleiben.

Die vollständige Methode, diese Kosten zu zählen und die Einsparungen in eine Rückflusszahl zu verwandeln, steht in [Kapitel 16 — Ziele, Kosten und Kapitalrendite](ch16-goals-costs-and-return-on-investment.md). In einer regulierten Umgebung füge die Kosten der Compliance in das Buch ein, bevor du eine Einsparung zählst.

## Die Ergebnisse

Nach einem Jahr, gemessen an einer Ausgangsbasis, die die Klinik vor dem Start erfasst hat, sieht das illustrative Ergebnis so aus. Deine Zahlen werden abweichen. Diese zeigen, wie eine gute Passung aussehen kann.

- **Das Nichterscheinen sank.** Automatische Erinnerungen brachten mehr Patienten zu ihren Terminen, sodass weniger Slots verschwendet wurden und mehr Leute behandelt wurden.
- **Die Telefonwarteschlange wurde kürzer.** Der Chatbot und die Selbstbuchung erledigten die routinehaften Anrufe, sodass die Empfangstheke sich auf Patienten konzentrieren konnte, die eine Person brauchten.
- **Die Dokumentationszeit sank.** Ärzte verbrachten weniger Zeit mit dem Tippen von Notizen und mehr Zeit mit Patienten, weil sie von einem zu prüfenden Entwurf ausgingen statt von einer leeren Seite.
- **Dokumente bewegten sich schneller.** Überweisungen und Formulare wurden automatisch sortiert und weitergeleitet, sodass weniger ungelesen lag und weniger Patienten wartend zurückblieben.
- **Der Zugang verbesserte sich.** Der mehrsprachige Fragen-Assistent half Eltern und Bürgern, die die lokale Sprache nicht sprechen, Antworten zu bekommen, ohne auf einen Dolmetscher zu warten.

Die ehrliche Einschränkung: Nichts davon war sofort. Das Dokumentationswerkzeug entwarf anfangs unvollkommene Notizen und brauchte jeden Arzt, der seinen Stil korrigierte. Der Terminplanungs-Bot missverstand anfangs manche Anfragen. Die Gewinne stiegen über Wochen an, wie die Lernkurven-Warnung in [Kapitel 16](ch16-goals-costs-and-return-on-investment.md) vorhersagt. Die Klinik maß die echten Zahlen nach dem Anstieg, nicht während ihm.

## Gelernte Lektionen

**Regulierte Daten bedeuten eine höhere Latte, vom ersten Schritt an.** Gesundheitsdaten und Kinderdaten sind besondere Kategorie. Du kannst sie nicht wie eine Produktbeschreibung behandeln. Nutze konforme Werkzeuge, unterzeichne eine Auftragsverarbeitungsvereinbarung, halte die Daten in der Region und mache eine Folgenabschätzung für den Datenschutz vor dem Livegang. Die Regeln stehen in [Kapitel 10](ch10-privacy-and-gdpr.md) und [Kapitel 5](ch05-rules-and-legal-responsibility.md).

**Automatisiere niemals die Entscheidung.** Ein Werkzeug darf eine klinische Notiz entwerfen, aber ein Arzt unterschreibt sie und trägt sie. Ein Werkzeug darf einen Antrag sortieren, aber ein Fallbearbeiter entscheidet ihn. In diesen Umgebungen arbeitet die KI an der Verwaltung um die Entscheidung herum und trifft nie die Entscheidung. Das ist sowohl eine Sicherheitsregel als auch, für risikoreichere Nutzungen, eine rechtliche nach dem EU AI Act.

**Zustimmung zur Aufzeichnung ist nicht optional.** Umgebende Dokumentation zeichnet ein Gespräch auf. Der Patient muss es wissen und zustimmen, klar und vorher. Nimm nicht still auf. Das ist Verarbeitung personenbezogener Daten nach [Kapitel 10](ch10-privacy-and-gdpr.md).

**Datenminimierung schützt dich.** Gib jedem Werkzeug nur die Daten, die es braucht. Der Terminplanungs-Bot braucht nicht die vollständige Krankenakte. Je weniger sensible Daten ein Werkzeug berührt, desto kleiner der Schaden, wenn es schiefgeht.

**Behalte einen Protokollpfad.** Protokolliere, was die KI tat und was der Mensch prüfte. In einer regulierten Umgebung ist es genauso wichtig, die Aufzeichnung später zeigen zu können wie das Ergebnis selbst.

**Hüte dich der selbstbewussten falschen Antwort.** Ein entworfene Notiz, die falsch wiedergibt, was gesagt wurde, oder ein Chatbot, der eine falsche Anweisung gibt, kann hier echten Schaden anrichten. Ein Mensch muss prüfen. Das Zuverlässigkeitsproblem steht in [Kapitel 2 — KI einfach erklärt](ch02-ai-explained-simply.md), und die Pflicht zur Ehrlichkeit in [Kapitel 4 — Ethische KI: Das Richtige tun](ch04-ethical-ai-doing-the-right-thing.md).

**KI kann den Zugang erweitern, nicht nur Kosten senken.** Der mehrsprachige Assistent und der immer offene Chatbot halfen Menschen, die sonst Mühe haben, das Büro zu erreichen. In öffentlichen Diensten ist diese Fairness ein Ergebnis, das genauso viel wert ist wie das gesparte Geld.

**Misse ehrlich und erwarte den Anstieg.** Erfasse die Ausgangsbasis, bevor du beginnst. Beurteile das Projekt nach der Lernkurve, nicht während ihr. Die Methode steht in [Kapitel 22 — Ergebnisse und ROI messen](ch22-measuring-results-and-roi.md).

Die Lektion für Kliniken, Schulen und öffentliche Ämter ist dieselbe wie in jedem Sektor, mit der strengsten Leitplanke von allen: Finde die Verwaltungslast — Terminplanung, Dokumente, wiederholte Fragen —, lass die KI entwerfen, sortieren und antworten, halte einen ausgebildeten Menschen bei jeder Entscheidung, schütze die sensiblen Daten, wie es das Gesetz verlangt, und misse ehrlich. Der Preis ist nicht nur ein billigeres Büro. Es ist mehr Zeit mit Patienten, Schülern und Bürgern — und das ist der ganze Sinn der Arbeit.
