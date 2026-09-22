# Kapitel 32 — Eine professionelle Praxis

*Dieses Kapitel ist ein repräsentatives Composite. Es ist keine einzelne echte Firma. Es kombiniert die üblichen Muster, die wir in kleinen Anwalts- und Steuerkanzleien sehen, die KI einführen. Alle Zahlen sind illustrativ — sie zeigen die Form der Entscheidung, kein Versprechen. Ersetzen Sie sie durch Ihre eigenen.*

## Kontext

Stellen Sie sich eine kleine Wirtschaftskanzlei vor. Wir nennen sie **Marlowe Legal**. Sie hat zwölf Anwälte und einige Mitarbeiter im Backoffice. Sie ist nicht die Art Kanzlei, die vor Richtern argumentiert. Sie macht Papierarbeit: Verträge, Mietverträge, Gesellschaftsverträge, Compliance-Beratung. Die Kunden sind andere Unternehmen.

Die Arbeit einer solchen Kanzlei ist im Kern Lesen und Schreiben. Ein Kunde schickt einen langen Vertrag und fragt: „Ist das sicher zu unterschreiben?" Ein neuer Kunde ruft an und muss sein Mandat eröffnen lassen. Ein Standard-Mietvertrag muss aus der Vorlage der Kanzlei erstellt werden. Am Monatsende schreibt jeder Anwalt die Minuten auf, die er gearbeitet hat, und schickt eine Rechnung.

Jahrelang wurde all das von Hand gemacht. Ein Junior-Anwalt liest einen zweihundertseitigen Vertrag und schreibt eine Zusammenfassung. Eine Empfangsdame nimmt den Anruf eines neuen Kunden und füllt ein Formular aus. Ein Senior-Anwalt tippt dieselben Klauseln in jeden Mietvertrag. Nachts versucht jeder, sich zu erinnern, woran er gearbeitet hat, um es abrechnen zu können. Die Kanzlei ist profitabel und angesehen. Aber sie verbringt eine große Menge teurer, ausgebildeter Zeit mit Arbeit, die repetitiv ist.

Eine professionelle Praxis unterscheidet sich von einem Laden oder einer Fabrik in einem entscheidenden Punkt. Alles, was sie berührt, ist **vertraulich**. Der Vertrag eines Kunden, ein Fusionsplan, eine Streitakte — diese sind durch das Anwaltsgeheimnis geschützt, die Regel, dass ein Kunde frei mit seinem Anwalt sprechen kann, ohne dass der Inhalt preisgegeben wird. Diese eine Tatsache verändert, wie KI genutzt werden kann, und sie ist der Faden, der sich durch dieses ganze Kapitel zieht.

## Das Problem

Die Probleme der Kanzlei sind dieselben vier Lecks wie überall, aber mit einer professionellen Note.

**Dokumentprüfung ist langsam und teuer.** Wenn ein Kunde die Kanzlei bittet, einen Vertrag zu prüfen, liest ein Junior-Anwalt jede Seite und macht Notizen zu riskanten Klauseln. Für ein großes Geschäft dauert das Tage. Der Kunde zahlt für diese Tage. Die Arbeit ist sorgfältig, aber repetitiv — dieselben Arten riskanter Klauseln tauchen immer wieder auf, und die Kanzlei weiß bereits, worauf sie achten muss. Es dauert nur lang, nachzusehen.

**Kundenaufnahme ist uneinheitlich.** Wenn ein neuer Kunde anruft, hängt das erfasste Wissen davon ab, wer antwortet. Manche bekommen ein vollständiges Bild; andere verpassen ein Detail, das später zählt. Wichtige Fakten fallen durchs Raster, und der Anwalt muss ihnen hinterherlaufen.

**Das Erstellen wiederholt sich.** Die Kanzlei hat Vorlagen, aber jeder neue Mietvertrag oder jede neue Vereinbarung braucht trotzdem einen Anwalt, der die Standardklauseln zusammenstellt und anpasst. Es ist zuverlässig, aber langsam, und es ist genau die Art Arbeit, die kein Urteilsvermögen eines Seniors braucht.

**Abrechnung leckt.** Anwälte rechnen nach Stunden ab, aber sie sind schlecht darin, jede Minute aufzuzeichnen. Ein Zehn-Minuten-Anruf hier, eine schnelle E-Mail dort — diese bleiben oft ungeschrieben. Am Monatsende „schreibt die Kanzlei Stunden ab, die sie tatsächlich gearbeitet, aber nie abgerechnet hat. Über zwölf Anwälte gerechnet ist dieses Leck groß. Eine Studie über Anwaltskanzleien hat die typische nicht abgerechnete Zeit in den Bereich einiger Prozent aller gearbeiteten Stunden eingeordnet; betrachten Sie das als eine Richtungszahl, nicht als eine präzise. Der Punkt bleibt: Das Leck ist real.

Die Einschränkung, die über allen vier liegt, ist die Vertraulichkeit. Jedes Tool, das den Vertrag eines Kunden liest, muss ein Tool sein, dem die Kanzlei vertrauen kann, dass es diesen Vertrag nicht durchsickern lässt. Das ist keine kleine Sorge. Es ist die erste Frage, vor jeder anderen.

## Die Lösung

Marlowe Legal greift die vier Lecks in Reihenfolge der Sicherheit an, nicht nur der Größe nach. Die Regel ist einfach: Beginnen Sie dort, wo ein Fehler billig ist und die Daten nicht sensibel sind, und bewegen Sie sich erst zur sensiblen Arbeit, wenn die Werkzeuge vertrauenswürdig sind.

**Dokumentprüfung, die zuerst liest, dann entscheidet der Anwalt.** Die Kanzlei nutzt einen KI-Assistenten, der einen Vertrag liest und eine Erstzusammenfassung erstellt: was die Vereinbarung tut, welche Klauseln ungewöhnlich sind und welche von den eigenen Standardpositionen der Kanzlei abweichen. Der Junior-Anwalt liest nicht mehr kalt. Er liest die Notizen der KI und verifiziert dann gegen das echte Dokument. Die KI kurzlistet die riskanten Klauseln; der Anwalt fällt die juristische Bewertung. Das ist dasselbe „Maschine entwirft, Mensch prüft"-Muster, das der Elanco-Fall in [Kapitel 25 — Verwaltung und Finanzen](ch25-administration-and-finance.md) zeigt.

**Aufnahme, die jedes Mal die richtigen Fragen stellt.** Ein strukturierter Aufnahme-Assistent — ein geführtes Formular auf der Website oder ein Chatbot, der einen festen Satz von Fragen stellt — erfasst für jeden neuen Kunden dieselben Fakten. Nichts wird verpasst, weil jemand vergessen hat zu fragen. Die strukturierten Informationen fließen direkt in die Fallakte. Die Chatbot-Seite davon ist dieselbe Technologie, die in [Kapitel 26 — Vertrieb und Marketing](ch26-sales-and-marketing.md) und [Kapitel 27 — Kundenservice und Support](ch27-customer-care-and-support.md) behandelt wird.

**Erstellungshilfe für die Standardteile.** Für Routine-Dokumente stellt ein KI-Erstellungsassistent die Standardklauseln zusammen und schlägt den Wortlaut vor. Der Anwalt prüft und passt an. Der Senior-Anwalt hört auf, Fließtext zu tippen, und beginnt stattdessen, Entwürfe zu prüfen.

**Abrechnung, die die Zeit erfasst, während sie entsteht.** Statt den Tag nachts zu rekonstruieren, nutzt die Kanzlei ein Tool, das Aktivität — gesendete E-Mails, geöffnete Dokumente, Kalendereinträge — in einen Zeitbuchungs-Entwurf mit einem vorgeschlagenen Text verwandelt. Der Anwalt prüft und bestätigt. Das Leck verengt sich, weil der Ausgangspunkt ein nahezu vollständiger Entwurf ist, nicht ein leeres Blatt.

In jedem Fall bleibt der Mensch verantwortlich. In einem Beruf, in dem eine falsche Antwort einem echten Kunden schadet, ist die KI ein Ersthelfer, niemals der Entscheidungsträger.

## Die Werkzeuge

Die Werkzeuge sind gewöhnlich, aber die Art, wie sie eingesetzt werden, ist durch die Vertraulichkeit geformt.

- **Ein Dokumentprüfungs-Assistent**, der Verträge liest und Klauseln gegen eine Checkliste abgleicht, die die Kanzlei selbst schreibt. Das ist dieselbe Klasse von Dokumentlese-Tools, die in [Kapitel 25](ch25-administration-and-finance.md) Rechnungen bearbeitet, hier auf juristischen Text gerichtet.
- **Ein Aufnahme-Chatbot oder ein geführtes Formular** auf der Website der Kanzlei, das einen festen Satz von Fragen stellt und die Antworten in das Fallmanagementsystem schreibt.
- **Ein Erstellungsassistent** für Standardklauseln und Vereinbarungen, verbunden mit den Vorlagen der Kanzlei.
- **Ein Zeiterfassungs- und Abrechnungsassistent**, der Zeitbuchungen aus der Tagesaktivität entwirft.

Wie man diese Werkzeuge auswählt, ohne sich von einer Demo blenden zu lassen, behandelt [Kapitel 17 — Werkzeuge wählen, ohne sich täuschen zu lassen](ch17-choosing-tools-without-being-fooled.md). Wie man sie an die vorhandene Fallmanagement-Software der Kanzlei anschließt, steht in [Kapitel 19 — KI an Systeme anschließen, die Sie bereits nutzen](ch19-connecting-ai-to-systems-you-already-use.md).

**Die Vertraulichkeitsfrage kommt zuerst.** Ein allgemeiner Chatbot, in den Sie einen Kundenvertrag einfügen, möglicherweise speichert diesen Vertrag, trainiert darauf oder legt ihn offen. Für eine Anwaltskanzlei kann das das Anwaltsgeheimnis und die Kundenpflicht brechen. Die Kanzlei muss Werkzeuge nutzen, die Kundendaten privat halten — entweder ein Geschäftsklasse-Dienst mit einem klaren Nicht-Trainieren-, Nicht-Teilen-Vertrag, oder ein Modell, das auf den eigenen Rechnern der Kanzlei läuft. Selbst hosten wird erklärt in [Kapitel 8 — Selbst hosten: Behalten Sie Ihre Daten unter Kontrolle](ch08-self-hosting-keep-your-data-under-control.md). Die Gefahr, dass Mitarbeiter still Kundendaten in öffentliche Tools einfügen — Schatten-KI — ist das Thema von [Kapitel 9 — Drittanbieterdienste und Schatten-KI](ch09-third-party-services-and-shadow-ai.md). Und weil Kundenakten personenbezogene Daten enthalten, gelten die Datenschutzregeln von [Kapitel 10 — Datenschutz und DSGVO](ch10-privacy-and-gdpr.md) in vollem Umfang.

## Die Kosten

Hier ist ein illustratives Erstjahresbudget für eine Kanzlei wie Marlowe. Das sind erfundene Zahlen, um die Form zu zeigen. Nutzen Sie Ihre eigenen.

**Direkte Kosten.**
- Dokumentprüfungs-Assistent (Geschäftsklasse, mit Vertraulichkeitsvertrag): etwa 12.000 € pro Jahr.
- Aufnahme-Chatbot: etwa 3.600 € pro Jahr.
- Erstellungsassistent: etwa 4.800 € pro Jahr.
- Zeiterfassungs- und Abrechnungsassistent: etwa 4.800 € pro Jahr.
- Einrichtung und Integration mit dem Fallmanagementsystem: etwa 9.000 € einmalig.
- Schulung der Anwälte und Mitarbeiter: etwa 4.000 € einmalig.

Erstjahr gesamt: rund **38.200 €**. In stabilen Jahren danach kommen die wiederkehrenden Abos auf etwa **25.200 €**.

**Indirekte Kosten.**
- Anwälte verbringen Zeit damit, jeden KI-Entwurf zu prüfen. Das ist die Kosten des Sicherheitsnetzes, und es muss bleiben.
- Das Lernloch, während sich alle anpassen.
- Die Kosten eines Fehlers, wenn ein Entwurf ohne Prüfung vertraut wird — in einem Beruf kann das weit größer sein als das Abo. Planen Sie für sorgfältige Prüfung, nicht für Hoffnung.
- Zeit, die für die Prüfung jedes Werkzeugs auf Vertraulichkeit und Compliance vor der Nutzung aufgewendet wird.

Die volle Methode, um diese Kosten zu zählen und die Einsparungen in eine Renditezahl zu verwandeln, steht in [Kapitel 16 — Ziele, Kosten und Kapitalrendite](ch16-goals-costs-and-return-on-investment.md).

## Die Ergebnisse

Nach einem Jahr, gemessen an einer Ausgangsbasis, die die Kanzlei vor dem Start aufgezeichnet hat, sieht das illustrative Ergebnis so aus. Ihre Zahlen werden abweichen. Diese zeigen, wie eine gute Passung aussehen kann.

- **Dokumentprüfung beschleunigt.** Der Ersturchgang des Junior-Anwalts bei einem langen Vertrag fiel von Tagen auf Stunden, weil er von der KI-Zusammenfassung ausging und verifizierte, statt kalt zu lesen.
- **Aufnahme wurde vollständig.** Jeder neue Kunde liefert jetzt denselben Satz von Fakten. Weniger Lücken, die später hinterhergejagt werden müssen.
- **Erstellung wurde schneller.** Routine-Dokumente brauchten nur noch einen Bruchteil der Zeit, weil der Anwalt einen Entwurf prüfte, statt Fließtext zusammenzustellen.
- **Abrechnungsleck verengt.** Weil die Zeit erfasst wurde, während sie entstand, gingen weniger gearbeitete Stunden ungeschrieben. Die Kanzlei rechnete mehr von dem ab, was sie tatsächlich tat.

Der ehrliche Vorbehalt: Nichts davon war sofort. Der Dokumentprüfungs-Assistent lieferte anfangs unvollkommene Zusammenfassungen und brauchte eine abgestimmte Checkliste der Kanzlei. Das Abrechnungstool erzeugte Entwürfe, die die Anwälte korrigieren mussten, bevor sie vertrauten. Die Gewinne stiegen über Wochen an, wie die Lernkurven-Warnung in [Kapitel 16](ch16-goals-costs-and-return-on-investment.md) vorhersagt. Die Kanzlei maß die echten Zahlen nach dem Anstieg, nicht während ihm.

## Gelernte Lektionen

**Vertraulichkeit ist die erste Einschränkung, nicht ein nachträglicher Gedanke.** In einer professionellen Praxis lautet die Frage nie nur: „Funktioniert dieses Werkzeug?" Sie lautet: „Kann diesem Werkzeug die private Akte eines Kunden anvertraut werden?" Beantworten Sie das vor allem anderen. Nutzen Sie Werkzeuge der Geschäftsklasse mit einem klaren Nicht-Trainieren-Vertrag, oder hosten Sie selbst. Siehe [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) und [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).

**Die KI entwirft; der Profi berät.** Der Wert eines Anwalts ist Urteilsvermögen und Verantwortung. Die KI kurzlistet und entwirft; der Anwalt entscheidet und unterschreibt. Lassen Sie einen Entwurf niemals zur Beratung werden, ohne dass ein menschlicher Geist darauf liegt.

**Hüten Sie sich vor der selbstsicheren falschen Antwort.** Diese Werkzeuge können Text erzeugen, der richtig klingt und falsch ist — eine Klausel, die es nicht gibt, ein Zitat, das erfunden ist. In einem Beruf ist eine erfundene Referenz eine Katastrophe. Verifizieren Sie jedes Zitat und jede juristische Behauptung gegen die echte Quelle. Das Zuverlässigkeitsproblem behandelt [Kapitel 2 — KI einfach erklärt](ch02-ai-explained-simply.md), und die Pflicht, ehrlich darüber zu sein, was KI kann und was nicht, steht in [Kapitel 4 — Ethische KI: Das Richtige tun](ch04-ethical-ai-doing-the-right-thing.md).

**Beginnen Sie mit der sicheren Arbeit.** Marlowe begann mit interner Erstellung und Aufnahme — geringes Risiko, noch nicht die sensibelsten Kundenakten. Sie bewegte sich erst zur Vertragsprüfung, als die Werkzeuge vertraut waren. Das ist die „hohe Leichtigkeit zuerst"-Regel aus [Kapitel 12](ch12-where-ai-can-help-your-business.md).

**Abrechnungs-KI muss in beide Richtungen geprüft werden.** Ein Zeiterfassungs-Tool kann zu wenig erfassen, aber es kann auch zu viel erfassen oder falsch beschriften. Einen Kunden auf Basis einer KI-Vermutung überzurechnen, ist ein ethisches und rechtliches Problem. Der Anwalt prüft jede Buchung. Die Regeln rund um Berufsethik und die Pflichten des EU AI Act stehen in [Kapitel 5 — Regeln und rechtliche Verantwortung](ch05-rules-and-legal-responsibility.md).

**Personenbezogene Daten bleiben personenbezogene Daten.** Kundenakten enthalten Namen, Adressen, Finanzdetails. Die Datenschutzpflichten in [Kapitel 10](ch10-privacy-and-gdpr.md) gelten für jede einzelne davon, egal wie das Werkzeug vermarktet wird.

**Messen Sie ehrlich und erwarten Sie den Anstieg.** Zeichnen Sie die Ausgangsbasis auf, bevor Sie beginnen. Beurteilen Sie das Projekt nach der Lernkurve, nicht während ihr.

Die Lektion der professionellen Praxis ist dieselbe wie in jeder Branche, mit einer zusätzlichen Schutzplanke: Finden Sie die repetitive Arbeit, lassen Sie KI entwerfen und markieren, behalten Sie einen Menschen beim Urteilsvermögen, und messen Sie ehrlich — und in einem Beruf lassen Sie das Werkzeug niemals an die vertrauliche Akte eines Kunden, bis Sie sicher sind, dass es sicher ist.

<!-- BEGIN agentbridge-examples -->

## Testen Sie es mit AgentBridge

So sieht dieselbe Aufgabe mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die Sie eintippen, um es zu erhalten.

### Einen Dienstleistungsvertrag entwerfen

![Ein entworfener Dienstleistungsvertrag, bereit zur Prüfung](../../assets/examples/service-contract.png)
*Ein entworfener Dienstleistungsvertrag, bereit zur Prüfung*

**Was Sie fragen:** `Entwirf einen Dienstleistungsvertrag zwischen meinem Studio und einem Kunden für ein 3-monatiges Website-Projekt zu 6.000 Euro, mit 50 % Anzahlung.`

Der Agent erstellt einen klaren Vertrag mit den Parteien, dem Leistungsumfang, dem Zahlungsplan und dem Zeitplan. Es ist ein Ausgangspunkt, den Sie prüfen und anpassen können — keine Rechtsberatung, aber ein solider Entwurf, der Ihnen Stunden Arbeit am leeren Blatt erspart.

*Tipp: Hängen Sie Ihren alten Vertrag an und bitten Sie ihn, demselben Stil und denselben Klauseln zu folgen.*

<!-- END agentbridge-examples -->
