# Kapitel 34 — Dienstleistungen und Beratung

*Dieses Kapitel ist ein repräsentatives Composite. Es ist keine einzelne echte Firma. Es kombiniert die üblichen Muster, die wir in Beratungs- und Professional-Services-Firmen sehen, die KI einführen. Alle Zahlen sind illustrativ — sie zeigen die Form der Entscheidung, kein Versprechen. Ersetzen Sie sie durch Ihre eigenen.*

## Kontext

Stellen Sie sich eine mittelgroße Beratungsfirma vor. Wir nennen sie **Northbeam Advisory**. Sie hat etwa fünfundzwanzig Berater und ein kleines Support-Team. Sie verkauft kein Produkt. Sie verkauft Fachwissen und Zeit. Ein Kunde — meist ein anderes Unternehmen — hat ein Problem, und Northbeam schickt Leute, um es zu lösen: hier ein Strategieprojekt, dort ein Betriebs-Review, irgendwo anders eine Datenstudie.

Jedes Projekt folgt demselben groben Weg. Zuerst kommt der **Pitch**: ein Angebot, das sagt, was die Firma versteht, was sie tun wird und was es kosten wird. Wenn der Kunde zustimmt, macht das Team die Arbeit. Während der Arbeit bekommt der Kunde regelmäßige **Statusberichte**. Am Ende gibt es eine finale Lieferung und eine Rechnung. Zwischen all dem liegt ein Berg an Koordination: die richtigen Leute für den Job finden, Meetings buchen, aufschreiben, was gesagt wurde, und den Überblick behalten, wer wann frei ist.

Jahrelang lief all das über Menschen. Ein Partner schreibt ein Angebot, indem er ein altes öffnet und umschreibt. Ein Berater löst ein Problem, das die Firma vor drei Jahren gelöst hat, aber niemand erinnert sich wo, also löst er es von Grund auf. Ein Projektmanager baut jeden Statusbericht von Hand und kopiert Zahlen aus einer Datei in eine Folie. Jemand verbringt einen halben Tag damit, Beraterkalender an Projektbedarfe anzupassen. Die Firma ist erfolgreich. Aber sie verbringt eine große Menge teurer, ausgebildeter Zeit mit Arbeit, die repetitiv ist, und sie verliert ständig Wissen, für das sie schon einmal bezahlt hat.

Eine Beratungsfirma ist wie eine professionelle Praxis in einem wichtigen Punkt. Alles, was sie berührt, ist **vertraulich**. Die Strategie eines Kunden, ein Kostenmodell, ein Fusionsplan — diese werden im Vertrauen geteilt. Diese eine Tatsache prägt, wie KI hier genutzt werden kann, genau wie bei einer Anwaltskanzlei. Sie ist der Faden, der sich durch dieses Kapitel zieht.

## Das Problem

Die Lecks der Firma sind leicht zu benennen.

**Angebote sind langsam.** Jeder neue Pitch beginnt nahe am leeren Blatt. Die Firma hat Hunderte von Angeboten geschrieben und gutes Material darin, aber das richtige frühere Beispiel, die richtige Fallstudie, die richtige Preisstruktur zu finden, kostet Zeit. Ein Partner verbringt möglicherweise zwei volle Tage mit einem Angebot, das zum großen Teil Wiederverwendung ist. Langsame Angebote bedeuten auch verpasste Chancen — manche Geschäfte gehen verloren, nur weil die Antwort zu spät kam.

**Wissen geht zur Tür hinaus.** Wenn ein Berater geht, geht das Know-how in seinem Kopf mit ihm. Eine Methode, die er verfeinert hat, eine Eigenheit eines Kunden, die er gelernt hat, eine Lösung, die er erarbeitet hat — sofern niemand es aufgeschrieben hat, ist es weg. Also zahlt die Firma dafür, dieselben Probleme immer wieder zu lösen. Das ist das teuerste Leck, weil es unsichtbar ist.

**Berichterstattung ist manuell.** Ein Statusbericht ist meist jede Woche derselbe: was sich bewegt hat, was spät ist, was als Nächstes kommt. Aber eine Person stellt ihn jedes Mal von Hand zusammen, zieht Zahlen aus Projektdateien und schreibt dieselbe Art von Text. Es ist zuverlässig und es ist langweilig, und es frisst Stunden, die abrechenbar sein könnten.

**Koordinationsaufwand.** Die Fähigkeiten des richtigen Beraters an ein Projekt anzupassen, zu prüfen, wer frei ist, Meetings zu buchen und danach die Notizen aufzuschreiben, ist eine ständige Steuer. Meetings finden statt, aber niemand will das Protokoll schreiben, also werden Entscheidungen unscharf und jemand muss das Gespräch später wiederholen.

Wenn Sie sehen wollen, wie diese gegen den Rest Ihrer Firma abschneiden, ist die Wirkung-Aufwand-Methode in [Kapitel 12 — Wo KI Ihrem Unternehmen helfen kann](ch12-where-ai-can-help-your-business.md) der Ort, um sie zu bewerten.

Über allen vier liegt die Vertraulichkeit. Jedes Tool, das das Angebot oder die Projektdatei eines Kunden liest, muss ein Tool sein, dem die Firma vertrauen kann, dass es sie nicht durchsickern lässt. Diese Frage kommt zuerst.

## Die Lösung

Northbeam greift die vier Lecks in Reihenfolge der Sicherheit an, nicht nur der Größe nach. Die Regel ist dieselbe, die eine Anwaltskanzlei nutzt: Beginnen Sie dort, wo ein Fehler billig ist und die Daten nicht am sensibelsten sind, und bewegen Sie sich erst zur sensiblen Arbeit, wenn die Werkzeuge vertrauenswürdig sind.

**Ein Angebots-Assistent, der aus der eigenen Geschichte der Firma entwirft.** Wenn ein neuer Pitch eingeht, schreibt ein Berater ein kurzes Briefing — der Kunde, das Problem, der grobe Umfang. Ein KI-Assistent durchsucht die früheren Angebote der Firma und zieht die relevantesten Abschnitte, dann entwirft er eine erste Version: ein Verständnis des Problems, ein vorgeschlagener Ansatz, eine passende Fallstudie. Der Partner beginnt nicht mehr kalt. Er bearbeitet einen Entwurf, statt aus dem Nichts aufzubauen. Zwei Tage werden ein paar Stunden. Das ist dasselbe „Maschine entwirft, Mensch prüft"-Muster, das der Elanco-Fall in [Kapitel 25 — Verwaltung und Finanzen](ch25-administration-and-finance.md) zeigt.

**Ein durchsuchbares Gedächtnis für die Firma.** Die Firma stellt ihre früheren Lieferungen, Methoden und Notizen in eine interne Suche, die Berater in klarer Sprache befragen können. Das wird oft eine **Wissensdatenbank mit KI-Suche** genannt. Im Kern nutzt sie eine Technik namens **retrieval-augmented generation**, oder RAG. In einfachen Worten: Statt eine allgemeine KI eine Frage zu stellen, schaut das System zuerst in den eigenen Dokumenten der Firma nach und antwortet dann nur mit dem, was es dort gefunden hat. Wenn also ein Berater fragt: „Wie haben wir eine Lieferantenrisiko-Prüfung für einen Einzelhandelskunden gehandhabt?", findet das System das echte frühere Projekt und antwortet aus ihm. Das Wissen hört auf, zur Tür hinauszugehen. Die Chatbot- und Suchtechnologie dahinter behandelt [Kapitel 27 — Kundenservice und Support](ch27-customer-care-and-support.md).

**Berichterstattung, die sich selbst entwirft.** Das Statusbericht-Tool verbindet sich mit den Projektdaten — Aufgaben, Termine, Meilensteine — und entwirft den Wochenbericht: was sich bewegt hat, was zurückfiel, was als Nächstes kommt. Der Projektmanager prüft ihn, fügt das menschliche Urteilsvermögen über Ton und was zu betonen ist hinzu, und sendet ihn. Das leere Blatt ist weg.

**Terminplanung und Meeting-Zusammenfassungen.** Ein Terminplanungs-Assistent gleicht Beraterfähigkeiten und Verfügbarkeit an Projektbedarfe an und schlägt vor, wer woran arbeiten sollte. Für Meetings zeichnet ein Tool den Anruf auf, entwirft das Protokoll und listet die Entscheidungen und Aufgabenpunkte. Ein Mensch prüft es, bevor es zirkuliert. Entscheidungen hören auf, unscharf zu sein, weil das Aufschreiben automatisch passiert.

In jedem Fall bleibt der Mensch verantwortlich. In der Beratung zahlt der Kunde für Urteilsvermögen und Verantwortung. Die KI entwirft, sucht und fasst zusammen. Der Berater entscheidet, passt an und steht hinter der Arbeit.

## Die Werkzeuge

Die Werkzeuge sind gewöhnlich, aber die Art, wie sie eingesetzt werden, ist durch die Vertraulichkeit geformt.

- **Ein Angebots-Assistent**, der die früheren Angebote der Firma durchsucht und aus einem Briefing ein neues entwirft.
- **Eine interne Wissenssuche** (RAG) über die Lieferungen und Notizen der Firma, damit Berater Fragen in klarer Sprache stellen und Antworten erhalten, die auf der eigenen Arbeit der Firma fußen.
- **Ein Berichterstattungs-Assistent**, der sich an Projektdaten verbindet und Statusberichte entwirft.
- **Ein Terminplanungs-Assistent** zum Anpassen von Leuten an Projekte, plus ein **Meeting-Zusammenfassungs-Tool**, das einen aufgezeichneten Anruf in einen Protokoll-Entwurf verwandelt.

Wie man diese Werkzeuge auswählt, ohne sich von einer Demo blenden zu lassen, behandelt [Kapitel 17 — Werkzeuge wählen, ohne sich täuschen zu lassen](ch17-choosing-tools-without-being-fooled.md). Wie man sie an die vorhandene Projektmanagement- und Dokumentensysteme der Firma anschließt, steht in [Kapitel 19 — KI an Systeme anschließen, die Sie bereits nutzen](ch19-connecting-ai-to-systems-you-already-use.md).

**Vertraulichkeit kommt zuerst.** Ein allgemeiner Chatbot, in den Sie ein Kundenangebot einfügen, möglicherweise speichert es, trainiert darauf oder legt es offen. Für eine Beratungsfirma kann das das Vertrauen eines Kunden und eine vertragliche Schweigepflicht brechen. Die Firma muss Werkzeuge nutzen, die Kundendaten privat halten — entweder ein Geschäftsklasse-Dienst mit einem klaren Nicht-Trainieren-, Nicht-Teilen-Vertrag, oder ein Modell, das auf den eigenen Rechnern der Firma läuft. Selbst hosten wird erklärt in [Kapitel 8 — Selbst hosten: Behalten Sie Ihre Daten unter Kontrolle](ch08-self-hosting-keep-your-data-under-control.md). Die Gefahr, dass Mitarbeiter still Kundendaten in öffentliche Tools einfügen — Schatten-KI — ist das Thema von [Kapitel 9 — Drittanbieterdienste und Schatten-KI](ch09-third-party-services-and-shadow-ai.md). Und weil Kundendateien und Kontaktlisten personenbezogene Daten enthalten, gelten die Datenschutzregeln von [Kapitel 10 — Datenschutz und DSGVO](ch10-privacy-and-gdpr.md) in vollem Umfang.

## Die Kosten

Hier ist ein illustratives Erstjahresbudget für eine Firma wie Northbeam. Das sind erfundene Zahlen, um die Form zu zeigen. Nutzen Sie Ihre eigenen.

**Direkte Kosten.**
- Angebots-Assistent (Geschäftsklasse, mit Vertraulichkeitsvertrag): etwa 12.000 € pro Jahr.
- Interne Wissenssuche (RAG-Plattform): etwa 9.000 € pro Jahr.
- Berichterstattungs-Assistent: etwa 4.800 € pro Jahr.
- Terminplanungs- und Meeting-Zusammenfassungs-Tools: etwa 6.000 € pro Jahr.
- Einrichtung und Integration mit den Projektmanagement- und Dokumentensystemen: etwa 12.000 € einmalig.
- Schulung der Berater und Support-Mitarbeiter: etwa 5.000 € einmalig.

Erstjahr gesamt: rund **48.800 €**. In stabilen Jahren danach kommen die wiederkehrenden Abos auf etwa **31.800 €**.

**Indirekte Kosten.**
- Berater verbringen Zeit damit, jeden KI-Entwurf zu prüfen. Das ist die Kosten des Sicherheitsnetzes, und es muss bleiben.
- Das Lernloch, während sich alle anpassen.
- Die Kosten der Pflege der Wissensdatenbank. Eine Suche ist nur so gut wie das, was Sie hineingeben, und jemand muss sie sauber und aktuell halten.
- Zeit, die für die Prüfung jedes Werkzeugs auf Vertraulichkeit und Compliance vor der Nutzung aufgewendet wird.
- Die Kosten eines Fehlers, wenn ein Entwurf ohne Prüfung vertraut wird — in der Beratung kann eine falsche Zahl in einem Kundenbericht weit mehr kosten als ein Abo.

Die volle Methode, um diese Kosten zu zählen und die Einsparungen in eine Renditezahl zu verwandeln, steht in [Kapitel 16 — Ziele, Kosten und Kapitalrendite](ch16-goals-costs-and-return-on-investment.md). Rechnen Sie die Mathematik nicht im Kopf. Schreiben Sie sie auf.

## Die Ergebnisse

Nach einem Jahr, gemessen an einer Ausgangsbasis, die die Firma vor dem Start aufgezeichnet hat, sieht das illustrative Ergebnis so aus. Ihre Zahlen werden abweichen. Diese zeigen, wie eine gute Passung aussehen kann.

- **Angebote wurden schneller.** Ein Pitch, der zwei Tage dauerte, dauert jetzt ein paar Stunden, weil der Partner einen Entwurf bearbeitet, statt vom leeren Blatt aus aufzubauen. Die Firma antwortet auch früher, was einige Geschäfte gewinnt, die sie verpasst hätte.
- **Wissen blieb.** Als Berater gingen, blieb ihr Know-how in der durchsuchbaren Datenbank. Die Firma löste weniger Probleme zweimal.
- **Berichterstattungszeit sank.** Der wöchentliche Statusbericht wurde eine Prüfung eines Entwurfs, kein manueller Aufbau, was Stunden über die Projektmanager hinweg freigab.
- **Meetings brachten Aufzeichnungen.** Entscheidungen und Aufgabenpunkte wurden automatisch aufgeschrieben, sodass weniger Gespräche wiederholt werden mussten.
- **Mehr abrechenbare Zeit.** Mit weniger Zeit für Wiederverwendung und Suche verbrachten Berater mehr ihres Tages mit Arbeit, für die der Kunde zahlt.

Der ehrliche Vorbehalt: Nichts davon war sofort. Der Angebots-Assistent erzeugte anfangs raue Entwürfe, bis er genug gute frühere Angebote hatte, um den Stil der Firma zu lernen. Die Wissenssuche gab schwache Antworten, bis die Dokumente organisiert und markiert waren. Das Meeting-Zusammenfassungs-Tool beschriftete anfangs die Sprecher falsch. Die Gewinne stiegen über Wochen an, wie die Lernkurven-Warnung in [Kapitel 16](ch16-goals-costs-and-return-on-investment.md) vorhersagt. Die Firma maß die echten Zahlen nach dem Anstieg, nicht während ihm.

## Gelernte Lektionen

**Vertraulichkeit ist die erste Einschränkung, nicht ein nachträglicher Gedanke.** In der Beratung lautet die Frage nie nur: „Funktioniert dieses Werkzeug?" Sie lautet: „Kann diesem Werkzeug die private Akte eines Kunden anvertraut werden?" Beantworten Sie das vor allem anderen. Nutzen Sie Werkzeuge der Geschäftsklasse mit einem klaren Nicht-Trainieren-Vertrag, oder hosten Sie selbst. Siehe [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) und [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).

**Die KI entwirft; der Berater berät.** Der Wert eines Beraters ist Urteilsvermögen und Verantwortung. Die KI kurzlistet, entwirft und fasst zusammen; der Berater entscheidet und unterschreibt. Lassen Sie einen Entwurf niemals zur kundengerichteten Arbeit werden, ohne dass ein menschlicher Geist darauf liegt.

**Eine Wissensdatenbank ist ein Garten, kein Mülleimer.** KI-Suche ist nur so gut wie die Dokumente dahinter. Wenn Sie chaotische, veraltete oder falsche Dateien hineinwerfen, bekommen Sie selbstsichere falsche Antworten. Jemand muss die Datenbank besitzen, aktuell halten und kontrollieren, wer was sehen kann. Zugriffskontrolle zählt: Ein Berater an einem Kundenprojekt sollte nicht die vertraulichen Materialien eines anderen Kunden heraussuchen können. Das Datenbereitschafts-Prinzip steht in [Kapitel 14 — Daten: Der Rohstoff](ch14-data-the-raw-material.md).

**Meetings aufzuzeichnen braucht Zustimmung.** Ein Meeting-Zusammenfassungs-Tool funktioniert, indem es den Anruf aufzeichnet. Ein Gespräch aufzuzeichnen ist eine Verarbeitung personenbezogener Daten, und die Leute müssen es wissen und zustimmen. Sagen Sie es den Teilnehmern, bevor Sie aufzeichnen, und befolgen Sie die Regeln in [Kapitel 10 — Datenschutz und DSGVO](ch10-privacy-and-gdpr.md). Zeichnen Sie nicht still auf.

**Hüten Sie sich vor der selbstsicheren falschen Antwort.** Diese Werkzeuge können Text erzeugen, der richtig klingt und falsch ist — eine Fallstudie, die nie stattfand, eine Zahl, die nicht aufgeht. In der Beratung ist eine erfundene Zahl in einem Kundenbericht eine Katastrophe. Verifizieren Sie jede Zahl und jede Behauptung gegen die echte Quelle. Das Zuverlässigkeitsproblem behandelt [Kapitel 2 — KI einfach erklärt](ch02-ai-explained-simply.md), und die Pflicht, ehrlich darüber zu sein, was KI kann und was nicht, steht in [Kapitel 4 — Ethische KI: Das Richtige tun](ch04-ethical-ai-doing-the-right-thing.md).

**Beginnen Sie mit der sicheren Arbeit.** Northbeam begann mit interner Suche und Berichterstattungs-Entwürfen — geringes Risiko, noch nicht die sensibelsten Kundenangebote. Sie bewegte sich erst zum Angebotsentwurf, als die Werkzeuge vertraut waren. Das ist die „hohe Leichtigkeit zuerst"-Regel aus [Kapitel 12](ch12-where-ai-can-help-your-business.md).

**Messen Sie ehrlich und erwarten Sie den Anstieg.** Zeichnen Sie die Ausgangsbasis auf, bevor Sie beginnen. Beurteilen Sie das Projekt nach der Lernkurve, nicht während ihr. Die Methode steht in [Kapitel 22 — Ergebnisse und ROI messen](ch22-measuring-results-and-roi.md).

Die Lektion der Beratungsfirma ist dieselbe wie in jeder anderen Branche, mit einer zusätzlichen Schutzplanke: Finden Sie die repetitive Arbeit — Angebote, Suche, Berichterstattung, Koordination — lassen Sie KI entwerfen und abrufen, behalten Sie einen Menschen beim Urteilsvermögen und der Kundenbeziehung, und messen Sie ehrlich. Und in einer Firma, die auf Vertrauen gebaut ist, lassen Sie das Werkzeug niemals an die vertrauliche Akte eines Kunden, bis Sie sicher sind, dass es sicher ist.

<!-- BEGIN agentbridge-examples -->

## Testen Sie es mit AgentBridge

So sieht dieselbe Aufgabe mit AgentBridge aus. Jede Box zeigt das fertige Ergebnis und die eine Zeile, die Sie eintippen, um es zu erhalten.

### Zeichnen Sie Ihr Servicegebiet

![Eine Servicegebietskarte für Kunden](../../assets/examples/service-area.png)
*Eine Servicegebietskarte für Kunden*

**Was Sie fragen:** `Zeige unser Servicegebiet auf einer Karte mit den wichtigsten Städten, die wir abdecken.`

Der Agent erstellt eine klare Karte Ihrer Abdeckung, die Sie auf Ihre Website setzen oder an Kunden senden können.

*Tipp: Halten Sie sie aktuell, wenn Sie wachsen — bitten Sie einfach um eine neue Version.*

<!-- END agentbridge-examples -->
