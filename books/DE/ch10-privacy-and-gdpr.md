# Kapitel 10 — Privatsphäre und DSGVO: Was Sie wirklich wissen müssen

## In einfachen Worten

DSGVO steht für Datenschutz-Grundverordnung. Es ist das Regelwerk der Europäischen Union für den Umgang mit personenbezogenen Daten — jede Information über eine lebende, identifizierbare Person. Es ist eines der strengsten Datenschutzgesetze der Welt, und es betrifft weit mehr Firmen, als die meisten Inhaber erwarten.

Das ganze Gesetz lässt sich auf eine Idee reduzieren: **Wenn Sie Informationen über eine Person haben, müssen Sie fair damit umgehen, aus einem klaren Grund, nur behalten, was Sie brauchen, es sicher aufbewahren und respektieren, was diese Person von Ihnen über die Nutzung verlangt.**

Sie sind betroffen, wenn Sie in der EU sind, und auch, wenn Sie außerhalb der EU sind, aber Menschen in der EU Waren oder Dienstleistungen anbieten oder ihr Verhalten beobachten. Ein kleiner Online-Shop in einem anderen Land, der Kunden in Frankreich beliefert, liegt in der Reichweite der DSGVO. Das heißt extraterritoriale Reichweite, und es überrascht viele Firmen.

Warum ist das für KI wichtig? Weil KI mit Daten arbeitet, und ein großer Teil dieser Daten personenbezogen ist. Kundennamen, Support-E-Mails, Lebensläufe, Personalakten, Webseiten-Besucher — alles personenbezogene Daten. Wenn Sie irgendetwas davon in ein KI-Werkzeug stecken, verarbeiten Sie personenbezogene Daten, und die Regeln gelten. Wenn Sie diese Daten an einen Drittdienst schicken, folgen die Regeln ihm zur Tür hinaus. Das ist die Verbindung zu [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).

Dieses Kapitel ist die ausführliche Heimat der DSGVO in diesem Buch. Es erklärt die Grundsätze, die Datenarten, die Rechtsgrundlagen, Ihre Pflichten und die Rechte, die Menschen Ihnen gegenüber haben. Der EU AI Act — ein eigenes Gesetz über KI-Systeme selbst — wird vollständig in [Kapitel 5](ch05-rules-and-legal-responsibility.md) behandelt; hier schauen wir nur darauf, wo er die Privatsphäre berührt. Die Sicherheitsseite des Datenschutzes ist in [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md).

Ein ehrlicher Hinweis: Das ist ein schlichter Leitfaden, keine Rechtsberatung. Für echte Entscheidungen, besonders über Grenzen hinweg, sprechen Sie mit einem Datenschutz-Fachmann.

## Ein wenig Geschichte

**1995: die erste EU-Regel.** Die Datenschutzrichtlinie setzte frühe Standards in Europa, aber jedes Land setzte sie anders um, was ein Flickwerk ergab.

**27. April 2016: DSGVO verabschiedet.** Die EU ersetzte das Flickwerk durch eine einzige Verordnung, die überall in den Mitgliedstaaten gleich gelten und die Regeln für das Internet-Zeitalter modernisieren sollte.

**25. Mai 2018: DSGVO gilt.** Das ist das wichtige Datum. Von diesem Tag an waren die Regeln vollständig in Kraft, mit hohen Bußgeldern bei schweren Verstößen. Firmen auf der ganzen Welt mussten sich daran halten oder das Risiko eingehen.

**2018 bis 2023: das Durchsetzungszeitalter.** Nationale Datenschutzbehörden verhängten Bußgelder, manche sehr hoch, für Verstöße und schlechte Praxis. Privatsphäre wurde ein Thema auf Vorstandsebene, nicht nur ein Anwaltsproblem.

**2018: der EDSA.** Der Europäische Datenschutzausschuss wurde geschaffen, um die nationalen Behörden zu koordinieren und Leitlinien herauszugeben, damit das Gesetz in der EU einheitlich angewandt wird. Seine Leitlinien sind die Stelle, an die Sie sich wenden, wenn das Gesetz unklar ist.

**1. August 2024: Der EU AI Act tritt in Kraft.** Ein eigenes Gesetz, die Verordnung (EU) 2024/1689, begann seinen gestaffelten Rollout. Es reguliert KI-Systeme nach Risiko. Es ersetzt die DSGVO nicht. Wo ein KI-System personenbezogene Daten nutzt, gelten beide Gesetze zugleich.

## Kuriosität

### 10.9 Was Europas Datenschützer über KI-Modelle sagten

Im Dezember 2024 verabschiedete der Europäische Datenschutzausschuss (EDSA) — das Gremium, das alle nationalen Datenschützer der EU koordiniert — die **Stellungnahme 28/2024** zum Schutz personenbezogener Daten im Kontext von KI-Modellen. Sie ist die wichtigste Datenschutz-Erklärung bisher dazu, wie KI zur DSGVO passt.

Einige Punkte daraus sind für einen Firmeninhaber wichtig:

**Ein Modell kann in drei Stufen betrachtet werden.** Der EDSA trennt das Leben eines KI-Modells in Entwicklung (es trainieren), Einsatz (es in Betrieb nehmen) und Nutzung (Menschen interagieren damit). Jede Stufe kann personenbezogene Daten betreffen, und jede hat ihre eigenen Datenschutzfragen. Das ist nützlich, weil es Ihnen sagt, die Frage in jeder Stufe zu stellen, nicht nur am Anfang.

**Berechtigtes Interesse kann eine Rechtsgrundlage sein, aber kein Freifahrtschein.** Die Stellungnahme sagt, ein Unternehmen darf sich bei der Entwicklung oder Nutzung eines KI-Modells auf „berechtigtes Interesse" stützen, aber nur wenn die Verarbeitung wirklich notwendig ist und ein Interessenausweis zeigt, dass sie die Rechte der Menschen nicht überwiegt. Sie können nicht einfach ein Interesse erklären und die beteiligten Menschen ignorieren.

**Ein Modell ist nur dann „anonym", wenn Sie keine personenbezogenen Daten herausbekommen.** Das ist der scharfe Teil. Der EDSA sagt, damit ein Modell als anonym — und damit außerhalb der DSGVO — behandelt wird, muss es sehr unwahrscheinlich sein, dass jemand durch Befragen personenbezogene Daten daraus herausziehen kann. Wenn ein Modell dazu gebracht werden kann, personenbezogene Details zu wiederholen, die es beim Training auswendig gelernt hat, ist es nicht wirklich anonym, und die Datenschutzregeln greifen weiterhin.

**Schlechte Trainingsdaten können dem Modell folgen.** Die Stellungnahme warnt, dass ein Modell, das mit rechtswidrig verarbeiteten personenbezogenen Daten trainiert wurde, die Rechtmäßigkeit des späteren Einsatzes beeinträchtigen kann, es sei denn, das Modell wurde ordentlich anonymisiert. In einfachen Worten: Ein Modell, das auf schmutzigen Daten gebaut wurde, kann schmutzig bleiben, und es zu nutzen kann dieses Problem in Ihr Geschäft tragen.

Die praktische Botschaft für eine kleine Firma ist klar. Wenn Sie einen KI-Anbieter wählen, ist die Datenschutzfrage nicht nur „was macht ihr jetzt mit meinen Daten", sondern „mit welchen Daten wurde dieses Modell trainiert, und kann man personenbezogene Daten wieder daraus herausziehen?" Diese Frage gehört in Ihre Anbieter-Checkliste.

## Ein echtes Geschäftsbeispiel

### Das HR-Werkzeug und die Zugriffsanfrage

Eine mittelgroße Firma mit 120 Mitarbeitern führt ein KI-Werkzeug ein, um Bewerbungen zu sichten. Es lädt Lebensläufe und Anschreiben hoch — alles personenbezogene Daten, manches davon sensibel, denn Lebensläufe können Gesundheitslücken, Alter, Nationalität und Gewerkschaftsaktivität preisgeben. Das Werkzeug rankt die Kandidaten.

Drei Monate später schreibt eine abgelehnte Bewerberin die Firma an. Sie stellt eine **Auskunftsanfrage**: Nach der DSGVO hat sie das Recht zu erfahren, welche personenbezogenen Daten die Firma über sie hat und wie sie genutzt wurden. Die Firma muss antworten, in der Regel innerhalb eines Monats und kostenfrei.

Jetzt muss die Firma harte Fragen beantworten, die sie nie gestellt hat. Wo sind ihr Lebenslauf und das KI-Ranking gespeichert? Kann sie die Daten hervorbringen und die Logik erklären? Gab es eine rechtmäßige Grundlage, ihren Lebenslauf mit diesem Werkzeug zu verarbeiten? Hat es vorher eine Risikobewertung gemacht? Wenn das Werkzeug ein Drittdienst war, hat der Vertrag das alles abgedeckt? Wenn das KI-Ranking als automatisierte Entscheidung mit schwerwiegender Wirkung auf sie gilt, greifen zusätzliche Regeln, einschließlich ihres Rechts, keiner rein automatisierten Entscheidung mit rechtlicher oder ähnlich erheblicher Wirkung unterworfen zu werden.

Die Firma hetzt herum, weil sie das Werkzeug einführte, bevor sie über die Daten nachdachte. Die Lehre ist die Reihenfolge der Schritte: Sie müssen die Daten und die Rechtsgrundlage verstehen, **bevor** Sie das Werkzeug einschalten, nicht wenn eine Anfrage eintrifft. Der Rest dieses Kapitels gibt Ihnen die Bausteine dafür.

## So machen Sie es

### 10.1 DSGVO auf einer Seite: die Grundprinzipien

Die DSGVO ruht auf einigen Grundsätzen. Wenn Sie diese einhalten, halten Sie den Großteil des Gesetzes ein.

**Rechtmäßigkeit, Fairness, Transparenz.** Sie brauchen einen gültigen rechtlichen Grund, personenbezogene Daten zu verarbeiten, Sie dürfen sie nicht auf Weisen nutzen, die Menschen als unfair empfinden, und Sie müssen den Menschen sagen, was Sie tun.

**Zweckbindung.** Erheben Sie Daten für einen klaren, genannten Zweck. Verwenden Sie sie später nicht für etwas Unverwandtes ohne eine neue rechtmäßige Grundlage.

**Datenminimierung.** Erheben Sie nur, was Sie wirklich brauchen. Wenn Sie keine Telefonnummer brauchen, fragen Sie nicht danach. Das ist für KI wichtig: kippen Sie nicht Ihre ganze Datenbank in ein Werkzeug, wenn eine kleine Scheibe genügt.

**Richtigkeit.** Halten Sie Daten korrekt und aktualisieren Sie sie. Menschen können Korrekturen verlangen.

**Speicherbegrenzung.** Bewahren Sie personenbezogene Daten nicht länger auf, als Sie sie brauchen. Haben Sie einen Löschplan.

**Integrität und Vertraulichkeit.** Halten Sie es sicher gegen Verletzungen. Die Anleitung dazu steht in [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md).

**Rechenschaftspflicht.** Sie müssen *nachweisen* können, dass Sie compliant sind — mit Protokollen, Richtlinien und Dokumenten. Deshalb ist der Papierkram im Abschnitt Checkliste nicht optional.

### 10.2 Personenbezogene Daten, sensible Daten, anonyme Daten: die Unterschiede, die zählen

**Personenbezogene Daten** sind jede Information über eine lebende Person, die direkt oder indirekt identifiziert werden kann. Ein Name, eine E-Mail, eine Telefonnummer, ein Foto, eine Ausweisnummer, ein Standort, eine Online-Kennung wie eine Cookie-ID. Selbst eine Kombination von Details, die jemanden heraushebt, zählt. Wenn Sie auf eine Person zeigen können, ist es eine personenbezogene Daten.

**Sensible Daten** (das Gesetz nennt sie „besondere Kategorien") bekommen stärkeren Schutz. Sie umfassen: rassische oder ethnische Herkunft, politische Meinungen, religiöse oder weltanschauliche Überzeugungen, Gewerkschaftszugehörigkeit, genetische Daten, biometrische Daten zur Identifizierung einer Person, Gesundheitsdaten und Daten über das Sexualleben oder die sexuelle Orientierung einer Person. Die Regel ist, dass die Verarbeitung dieser verboten ist, es sei denn, eine bestimmte Bedingung greift, wie ausdrückliche Einwilligung oder eine klare gesetzliche Anforderung. Passen Sie bei KI auf, dass diese sich in Lebensläufen, Support-Tickets und Personalakten verstecken. Ein Chatbot, der lernt „dieser Kunde ist Chemotherapie", hat Gesundheitsdaten berührt.

**Anonyme Daten** sind Informationen, die eine Person nicht mehr identifizieren können, selbst wenn man sie mit anderen Daten kombiniert. Wirklich anonyme Daten liegen außerhalb der DSGVO, weil es keine identifizierbare Person gibt. Aber echte Anonymität ist schwer zu erreichen. Wenn Sie jemanden re-identifizieren könnten, ist es nicht anonym. Das ist der Unterschied, an dem Menschen sich verheddern, und er ist der Fokus von Abschnitt 10.8.

Die praktische Regel: Behandeln Sie fast alles über einen Kunden, Mitarbeiter oder Bewerber standardmäßig als personenbezogene Daten. Behandeln Sie alles, was Gesundheit, Überzeugungen oder Identität berührt, als sensibel und gehen Sie mit extra Sorgfalt damit um. Nennen Sie Daten nur anonym, wenn Sie die Fähigkeit, jemanden zu identifizieren, wirklich entfernt haben.

### 10.3 Einwilligung: wann sie nötig ist und wann nicht

Die Einwilligung ist eine rechtmäßige Grundlage für die Verarbeitung, nicht die einzige, und sie wird oft missverstanden.

Damit Einwilligung gültig ist, muss sie **frei erteilt, spezifisch, informiert und eindeutig** sein, und durch eine klare Handlung gegeben werden. Ein vorangekreuztes Kästchen ist keine Einwilligung. Vergrabene Klauseln sind keine Einwilligung. Einwilligung für „Marketing und alles Mögliche" ist keine gültige Einwilligung.

Sie brauchen Einwilligung, wenn keine andere Grundlage passt, und in den meisten Fällen immer für sensible Daten, sowie für bestimmte Dinge wie Marketing-E-Mails an Verbraucher in vielen EU-Ländern.

Oft brauchen Sie **keine** Einwilligung, wenn eine andere Grundlage greift. Wenn Sie Daten verarbeiten, um einen Vertrag zu erfüllen, den Sie mit dem Kunden haben, ist das die „Vertrags"-Grundlage, nicht Einwilligung. Wenn ein Gesetz verlangt, dass Sie Aufzeichnungen führen, ist das „rechtliche Verpflichtung". Um Einwilligung zu bitten, wenn Sie schon einen Vertrag haben, kann tatsächlich Probleme schaffen, weil die Einwilligung jederzeit widerrufen werden kann, und dann können Sie nicht liefern, was Sie versprochen haben.

Für KI ist die Einwilligung heikel. Wenn Sie Kundendaten zum Trainieren eines Modells nutzen wollen, ist ein vages „wir dürfen Ihre Daten zur Verbesserung unserer Dienste nutzen" meist nicht genug. Sie müssen spezifisch sein, und Sie müssen die Leute Nein sagen lassen, ohne den Dienst zu verlieren. Der sicherere Weg ist, eine breite Einwilligung gar nicht erst zu brauchen: minimieren Sie die Daten, nutzen Sie sie nur, wo eine echte Grundlage existiert, und bevorzugen Sie nicht-personenbezogene oder anonymisierte Eingaben fürs Training.

### 10.4 Berechtigtes Interesse: wann Sie Daten ohne ausdrückliche Einwilligung nutzen dürfen

Berechtigtes Interesse ist die flexibelste und am meisten missbrauchte Grundlage. Sie erlaubt Ihnen, personenbezogene Daten ohne Einwilligung zu verarbeiten, wenn Sie einen echten, rechtmäßigen Geschäftsgrund haben — aber erst nach einem sorgfältigen Test.

Der Test hat drei Teile. **Zweck:** Ist Ihr Grund berechtigt? Betrugserkennung oder Netzsicherheit zu verbessern ist es meist. **Notwendigkeit:** Ist die Verarbeitung der personenbezogenen Daten tatsächlich nötig, um es zu erreichen, oder könnten Sie es mit weniger oder mit anonymen Daten? **Abwägung:** Überwiegen Ihre Interessen die Rechte und Erwartungen der Person? Würde ein verständiger Mensch überrascht oder geschädigt?

Sie müssen diese Abwägung dokumentieren. Sie ist kein Gefühl; sie ist eine schriftliche Bewertung, die Sie vorzeigen können.

Für KI kann berechtigtes Interesse manche Nutzungen abdecken — zum Beispiel Kundendaten aus dem Support zur Verbesserung der Servicequalität zu nutzen, wenn es notwendig und ausgewogen ist. Aber es erlaubt Ihnen nicht, etwas zu tun, das ein Kunde aufdringlich findet. Ein Modell unter „berechtigtem Interesse" mit sensiblen Daten zu trainieren, ist sehr schwer zu rechtfertigen. Und wie die EDSA-Stellungnahme im Kuriositäts-Abschnitt sagt, müssen die Notwendigkeits- und Abwägungstests wirklich bestehen.

Die Faustregel: Wenn Sie sich unwohl fühlen würden, die Nutzung der Person laut zu erklären, deckt berechtigtes Interesse sie wahrscheinlich nicht.

### 10.5 Rechte der betroffenen Person: Auskunft, Berichtigung, Löschung, Datenübertragbarkeit

Menschen haben Rechte über ihre Daten, und Sie müssen in der Lage sein, sie zu wahren. Die wichtigsten:

**Recht auf Information.** Sie müssen den Menschen klar sagen, welche Daten Sie erheben und warum, meist in einer Datenschutzhinweis.

**Recht auf Auskunft.** Eine Person kann fragen, welche Daten Sie über sie haben und wie Sie sie nutzen. Das ist die Auskunftsanfrage aus dem Beispiel. Sie müssen eine Kopie bereitstellen, meist innerhalb eines Monats, kostenfrei.

**Recht auf Berichtigung.** Wenn die Daten falsch sind, können sie berichtigt werden.

**Recht auf Löschung („Recht auf Vergessenwerden").** Sie können Sie bitten, ihre Daten zu löschen, und Sie müssen, es sei denn, ein gesetzlicher Grund zur Aufbewahrung überwiegt — zum Beispiel eine Steuerunterlage, die Sie aufbewahren müssen.

**Recht auf Einschränkung der Verarbeitung.** Sie können die Art, wie Sie die Daten nutzen, in bestimmten Situationen pausieren, während ein Streit geklärt wird.

**Recht auf Datenübertragbarkeit.** Sie können ihre Daten in einem strukturierten, gängigen, maschinenlesbaren Format verlangen, damit sie sie woanders hin bewegen können. Das verbindet sich mit dem Lock-in-Problem in [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).

**Recht auf Widerspruch.** Sie können der Verarbeitung auf Basis berechtigten Interests widersprechen, sowie Direktwerbung.

**Rechte rund um automatisierte Entscheidungen.** Nach Artikel 22 hat eine Person das Recht, keiner Entscheidung unterworfen zu werden, die ausschließlich auf automatisierter Verarbeitung beruht und rechtliche oder ähnlich erhebliche Wirkung auf sie hat, mit begrenzten Ausnahmen, sowie das Recht auf menschliche Beteiligung. Das ist kritisch für KI, die Menschen für Jobs, Kredit oder Dienste sichtet.

Bauen Sie einen einfachen, schriftlichen Prozess auf, um diese Anfragen fristgerecht zu empfangen und zu beantworten. Wenn Sie eine KI von Drittanbietern nutzen, stellen Sie sicher, dass der Anbieter Ihnen helfen kann, die Daten hervorzubringen und zu löschen, sonst können Sie die Anfrage nicht erfüllen.

### 10.6 Der EU AI Act: was sich für die Privatsphäre ändert

Der EU AI Act ist ein eigenes Gesetz neben der DSGVO, und er wird vollständig in [Kapitel 5](ch05-rules-and-legal-responsibility.md) behandelt. Hier ist nur die Privatsphären-Sicht, damit die beiden nicht verwechselt werden.

Stellen Sie es sich so vor. **Die DSGVO regelt die personenbezogenen Daten, die durch ein KI-System fließen. Der AI Act regelt das KI-System selbst — sein Risikoniveau, seine Pflichten und wie es genutzt werden darf.** Wenn Ihr KI-System personenbezogene Daten nutzt, gelten beide gleichzeitig. Sie sind keine Alternativen; sie stapeln sich.

Für ein Hochrisiko-KI-System, das personenbezogene Daten verarbeitet, erledigen Sie am Ende zwei verwandte Jobs. Unter dem AI Act durchlaufen Sie ein Risiko- und Konformitätsverfahren für das System. Unter der DSGVO brauchen Sie eine rechtmäßige Grundlage für die personenbezogenen Daten und, wo das Risiko hoch ist, eine Datenschutz-Folgenabschätzung. Die gute Nachricht: Die Arbeit überlappt — Ihre Daten verstehen, Ihren Prozess dokumentieren und Risiko bewerten, dient beiden Gesetzen.

Der AI Act drängt auch auf Datenqualität für Hochrisiko-Systeme — Trainings- und Testdaten sollten relevant und repräsentativ und so fehlerfrei wie angemessen sein. Das stimmt mit dem Richtigkeitsprinzip der DSGVO überein. Und die Transparenzpflichten des AI Act — den Leuten sagen, dass sie mit KI interagieren — sitzen neben den Transparenzpflichten der DSGVO.

Der praktische Punkt: Behandeln Sie den AI Act und die DSGVO nicht als eine Checkliste. Stellen Sie zwei Fragen über jedes KI-System. *Wie hoch ist das Risiko des Systems unter dem AI Act?* Und *welche personenbezogenen Daten fließen durch es, und ist das unter der DSGVO rechtmäßig?* Das Erste ist der Job von Kapitel 5; das Zweite ist der dieses Kapitels.

### 10.7 Datenschutz-Folgenabschätzung (DSFA): wann sie Pflicht ist und wie man sie macht

Eine Datenschutz-Folgenabschätzung ist eine strukturierte Prüfung, die Sie **vor** dem Start einer Verarbeitungstätigkeit machen, die wahrscheinlich ein hohes Risiko für Menschen birgt. Für KI werden Sie oft eine brauchen.

Sie müssen eine DSFA machen, wenn die Verarbeitung ein hohes Risiko ist. Klare Auslöser sind: systematische und umfangreiche Bewertung von Menschen auf Basis automatisierter Verarbeitung, die erhebliche Wirkungen erzeugt (das deckt KI ab, die Menschen bewertet, rankt oder profiliert); großangelegte Verarbeitung sensibler Daten; und großangelegte systematische Überwachung öffentlich zugänglicher Bereiche. Neue Technologien, neuartig eingesetzt, erhöhen das Risiko ebenfalls.

Wie man eine macht, in schlichten Schritten:

1. **Beschreiben Sie die Verarbeitung.** Welche Daten, welcher Zweck, wie lange, wer sieht sie, wo sie gespeichert sind, und ob ein Dritter oder eine KI beteiligt ist.
2. **Prüfen Sie Notwendigkeit und Verhältnismäßigkeit.** Ist das der am wenigsten aufdringliche Weg, Ihr Ziel zu erreichen?
3. **Bewerten Sie die Risiken für Menschen.** Nicht Risiko für Ihre Firma — Risiko für ihre Privatsphäre, Fairness und Rechte. Denken Sie an Voreingenommenheit, Fehler, Übererhebung und Re-Identifizierung.
4. **Listen Sie die Maßnahmen zur Risikominderung auf.** Minimieren Sie Daten, anonymisieren Sie wo möglich, fügen Sie menschliche Prüfung hinzu, sichern Sie das System, setzen Sie kurze Aufbewahrung.
5. **Entscheiden Sie.** Wenn nach Ihren Maßnahmen ein hohes Risiko bleibt, müssen Sie Ihre nationale Datenschutzbehörde konsultieren, bevor Sie fortfahren.
6. **Dokumentieren und überprüfen.** Schreiben Sie es auf und prüfen Sie es, wenn sich das System ändert.

Eine DSFA ist kein Formular zum Abhaken. Sie ist eine Denkübung, die ehrlich gemacht oft Ihr Design zum Besseren verändert.

### 10.8 Anonymisierung und Pseudonymisierung: was sie sind und warum sie zählen

Diese zwei Wörter klingen ähnlich und sind sehr verschieden. Sie zu verwechseln richtet echten Schaden an.

**Pseudonymisierung** bedeutet, Sie ersetzen direkte Kennungen durch einen Stellvertreter, wie einen Code, und halten den Schlüssel, der den Code mit der Person verknüpft, getrennt und sicher. „Kunde 4471" statt „Maria Rossi", mit weggeschlossener Zuordnungstabelle. Pseudonymisierte Daten sind unter der DSGVO **immer noch personenbezogene Daten**, weil Sie mit dem Schlüssel die Person re-identifizieren können. Es ist eine wertvolle Sicherheitsmaßnahme — es senkt das Risiko, wenn die Daten gestohlen werden — aber es nimmt Sie nicht aus dem Gesetz heraus.

**Anonymisierung** bedeutet, Sie entfernen identifizierende Informationen so gründlich, dass niemand eine Person re-identifizieren kann, selbst wenn man die Daten mit anderen Quellen kombiniert. Das Gesetz fragt, ob Re-Identifizierung „vernünftigerweise wahrscheinlich" ist, unter Berücksichtigung von Kosten, Zeit und heutigem Stand der Technik. Wirklich anonyme Daten liegen **außerhalb der DSGVO**, weil es keine identifizierbare Person gibt. Aber echte Anonymität ist echt schwer. Datensätze, die anonym aussehen, wurden durch Kreuzreferenzieren anderer öffentlicher Daten re-identifiziert.

Warum das für KI zählt: Wenn Sie ein Modell mit Daten trainieren wollen, ohne dass die DSGVO gilt, brauchen Sie echte Anonymität, nicht Pseudonymisierung. Und wie die EDSA-Stellungnahme warnt, kann selbst ein trainiertes Modell nicht anonym sein, wenn personenbezogene Daten durch geschicktes Befragen daraus extrahiert werden können. „Wir haben die Trainingsdaten anonymisiert" ist also eine Behauptung, die Sie verteidigen können müssen, nicht nur aufstellen.

Die sichere Arbeitsregel: Behandeln Sie pseudonymisierte Daten als personenbezogene Daten, weil sie es sind. Behandeln Sie Daten nur als anonym, wenn Sie getestet haben, dass Re-Identifizierung vernünftigerweise nicht möglich ist. Im Zweifel lassen Sie den DSGVO-Schutz an.

## Ethik und Verantwortung

Die DSGVO ist der Boden, nicht die Obergrenze. Compliance heißt, Sie vermeiden Bußgelder; Ethik heißt, Sie tun das Richtige, auch wo das Gesetz schweigt.

**Achten Sie den Menschen hinter den Daten.** Jede Akte ist das Privatleben von jemandem. Fragen Sie, ob Ihre Nutzung fair erschiene, wenn Sie selbst von einer KI profiliert würden.

**Verstecken Sie sich nicht hinter „das Modell hat es getan."** Wenn eine KI eine unfaire Entscheidung über eine Person mit Ihren Daten trifft, sind Sie verantwortlich. Halten Sie einen Menschen, der das Ergebnis trägt, wie [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md) darlegt.

**Seien Sie transparent über KI.** Sagen Sie den Leuten, wann eine KI ihre Daten berührt und was sie tut. Überraschungen erodieren Vertrauen schneller als jeder technische Fehler.

**Minimieren Sie als moralische Gewohnheit.** Weniger zu erheben ist nicht nur eine gesetzliche Regel; es ist Respekt. Jedes Feld, das Sie nicht erheben, ist ein Feld, das nicht geleakt oder missbraucht werden kann.

**Schützen Sie die Schutzbedürftigen.** Sensible Daten über Gesundheit, Überzeugungen oder Finanzen verdienen die höchste Sorgfalt. Wenn ein Werkzeug das nicht garantieren kann, stecken Sie es nicht in das Werkzeug.

## Zu vermeidende Fehler

1. **„Wir sind zu klein für die DSGVO."** Größe befreit Sie nicht. Wenn Sie personenbezogene Daten von Menschen in der EU verarbeiten, gelten die Regeln.
2. **Zu denken, Einwilligung sei immer nötig, oder nie.** Sie ist eine von sechs Grundlagen. Nutzen Sie die richtige und dokumentieren Sie warum.
3. **Pseudonymisierung mit Anonymität verwechseln.** Pseudonymisierte Daten sind immer noch personenbezogene Daten und immer noch im Anwendungsbereich.
4. **Ihre ganze Datenbank in ein KI-Werkzeug kippen.** Das bricht die Datenminimierung und streut Risiko.
5. **Keine rechtmäßige Grundlage fürs Training mit personenbezogenen Daten.** „Unsere Dienste verbessern" ist meist nicht genug.
6. **Sensible Daten in Lebensläufen und Tickets ignorieren.** Gesundheit, Überzeugungen und Gewerkschaftsaktivität können in gewöhnlichen Dokumenten stecken.
7. **Keine DSFA vor einem Hochrisiko-KI-Rollout.** Machen Sie sie vorher, nicht nach einer Beschwerde.
8. **Kein Prozess für Auskunfts- und Löschanfragen.** Wenn Sie die Daten nicht finden und löschen können, können Sie das Recht nicht wahren.
9. **Die Kontrolle über Daten an einen Dritten verlieren.** Wenn der Anbieter Ihnen nicht beim Löschen oder Exportieren helfen kann, sind Sie exponiert. Siehe [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).
10. **Das Gesetz als einmaliges Projekt behandeln.** Die DSGVO ist laufend. Aufbewahrung, Verletzungen und Anfragen kommen weiter.

## Praktische Übung

### 10.10 Ihre DSGVO-Compliance-Checkliste für KI

Nehmen Sie einen halben Tag und arbeiten Sie das für einen KI-Anwendungsfall durch, der personenbezogene Daten berührt.

1. **Karten Sie die Daten.** Listen Sie genau, welche personenbezogenen Daten in die KI fließen. Benennen Sie jedes Feld. Markieren Sie jede sensible Kategorie. (Eine Dateninventar-Vorlage ist im Anhang.)
2. **Nennen Sie die Rechtsgrundlage.** Schreiben Sie für jede Nutzung, welche der sechs Grundlagen greift und warum. Wenn Sie keine benennen können, stoppen Sie und überdenken Sie es.
3. **Prüfen Sie auf sensible Daten.** Wenn besondere-Kategorie-Daten vorhanden sind, bestätigen Sie, dass eine bestimmte Bedingung sie erlaubt, oder entfernen Sie sie.
4. **Wenden Sie Minimierung an.** Streichen Sie jedes Feld, das Sie nicht strikt brauchen.
5. **Entscheiden Sie das Ziel.** Gehen die Daten an einen Dritten? Wenn ja, fahren Sie die Anbieter-Fragen aus [Kapitel 9](ch09-third-party-services-and-shadow-ai.md).
6. **Machen Sie eine DSFA.** Wenn die Nutzung ein hohes Risiko ist — Profiling, großangelegte sensible Daten, automatisierte Entscheidungen —, schließen Sie die DSFA-Schritte in Abschnitt 10.7 ab.
7. **Planen Sie die Rechte.** Schreiben Sie, wie Sie Auskunfts-, Berichtigungs- und Löschanfragen für diese Daten handhaben, einschließlich der beim Anbieter gespeicherten Daten.
8. **Setzen Sie Aufbewahrung.** Entscheiden Sie, wie lange Sie die Daten behalten und wann Sie sie löschen.
9. **Prüfen Sie die Regeln für automatisierte Entscheidungen.** Wenn die KI über Menschen mit erheblicher Wirkung entscheidet, stellen Sie sicher, dass ein menschlicher Prüfpfad existiert.
10. **Dokumentieren Sie alles.** Schreiben Sie die Antworten auf. Rechenschaftspflicht heißt, Sie können Ihre Arbeit vorzeigen.

Wenn irgendein Schritt eine Lücke lässt, die Sie nicht füllen können, ist diese Lücke Ihre To-do-Liste.

## Checkliste

### 10.11 Die Dokumente, die Sie haben müssen

Für ein KI-System, das personenbezogene Daten berührt, halten Sie diese Dokumente bereit und aktuell.

- [ ] **Datenschutzhinweis**, der klar erklärt, welche Daten Sie erheben, warum, und wie KI beteiligt ist.
- [ ] **Verzeichnis von Verarbeitungstätigkeiten**, das jede Nutzung personenbezogener Daten beschreibt.
- [ ] **Rechtsgrundlage-Erklärung** für jeden Verarbeitungszweck, schriftlich festgehalten.
- [ ] **Dateninventar**, das jedes personenbezogene Datenfeld und wo es lebt, auflistet.
- [ ] **DSFA** für jede Hochrisiko-KI-Verarbeitung, mit der Restrisiko-Entscheidung.
- [ ] **Interessenausweis**, wenn Sie sich auf berechtigtes Interesse stützen.
- [ ] **Auftragsverarbeitungsvertrag** mit jedem Anbieter, der Ihre Daten bearbeitet.
- [ ] **Aufbewahrungsplan**, der angibt, wie lange jede Datenart behalten und wann sie gelöscht wird.
- [ ] **Betroffenen-Anfrage-Verfahren** für Auskunft, Berichtigung, Löschung und Übertragbarkeit, mit einem-Monats-Takt.
- [ ] **Verletzungsreaktionsplan**, einschließlich Meldung an die Behörde innerhalb von 72 Stunden und an betroffene Personen, wenn erforderlich.
- [ ] **Automatisierte-Entscheidungs-Schutzmaßnahmen** mit einem menschlichen Prüfpfad für bedeutsame Entscheidungen.
- [ ] **Kontaktdaten des Datenschutzbeauftragten**, falls Ihre Verarbeitung einen erfordert.

Halten Sie diese am Leben. Ein Dokument, das Sie nie aktualisieren, ist ein Dokument, das Sie im Stich lässt, wenn ein Regulator oder ein Kunde fragt.

## Wichtige Punkte

- Die DSGVO gilt für alle personenbezogenen Daten über identifizierbare Menschen in der EU, auch wenn sie durch ein KI-Werkzeug fließen, und sie reicht an Firmen außerhalb der EU, die EU-Kunden bedienen.
- Sie brauchen für jede Nutzung eine rechtmäßige Grundlage; Einwilligung ist nur eine von sechs, und sensible Daten brauchen zusätzlich eine bestimmte Bedingung.
- Menschen haben echte Rechte — Auskunft, Berichtigung, Löschung, Übertragbarkeit —, und Sie müssen sie wahren können, auch für Daten, die ein Drittanbieter hält.
- Pseudonymisierung ist nicht Anonymität; nur Daten, die vernünftigerweise nicht re-identifizierbar sind, verlassen die DSGVO, und ein Modell, das personenbezogene Daten leckt, ist nicht anonym.
- Machen Sie für Hochrisiko-KI vor dem Start eine DSFA, und denken Sie daran, dass der AI Act und die DSGVO zusammen gelten, nicht statt des jeweils anderen.
