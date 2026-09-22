# Kapitel 2 — KI einfach erklärt (ohne Fachbegriffe)

## In einfachen Worten

Fast alle Verwirrung über KI kommt von einer fehlenden Unterscheidung. Hast du sie einmal verstanden, verschwindet der meiste Lärm.

Normale Software tut das, was ein Mensch für sie geschrieben hat. Jemand hat sich hingesetzt und die Regeln geschrieben: Wenn die Summe über 100 liegt, Steuer addieren. Wenn eine E-Mail-Adresse kein @-Zeichen hat, einen Fehler anzeigen. Jeder Fall war vorher durchdacht und aufgeschrieben.

KI ist anders. Niemand hat die Regeln geschrieben. Stattdessen wurden dem System viele Beispiele der richtigen Antwort gezeigt, und es hat daraus seine eigenen Regeln abgeleitet.

Stell dir zwei Wege vor, einen neuen Mitarbeiter einzuarbeiten. Der erste ist eine Checkliste. Schritt 1, Schritt 2, Schritt 3, genau befolgen. Das ist normale Software: zuverlässig, günstig und völlig nutzlos in dem Moment, in dem etwas passiert, das nicht auf der Liste steht. Der zweite Weg ist, den Neben dir zu setzen und ihm fünfhundert fertige Arbeiten zu zeigen. Nach einer Weile bekommt er ein Gefühl dafür und kann Fälle behandeln, die ihm niemand erklärt hat. Das ist KI: flexibel, und manchmal auf eine Weise falsch, wie es eine Checkliste nie wäre.

Beides ist Automatisierung. Der einzige Unterschied ist, **woher die Anweisungen kommen.** Du hast sie geschrieben, oder die Maschine hat sie aus Beispielen erraten.

Hier ist die Definition, die du behalten solltest. **Künstliche Intelligenz ist Software, die nützliche Vermutungen auf Basis von Beispielen anstellt, statt für jeden Fall eine geschriebene Regel zu befolgen.**

Das Wort *Vermutung* leistet hier wichtige Arbeit. Ein KI-Ergebnis ist keine Gewissheit. Es hat eine Fehlerrate. Ein gutes KI-System hat eine niedrige Fehlerrate bei normalen Fällen und eine viel höhere bei seltsamen Fällen. Das ist kein Mangel, den man später behebt. Es ist das Wesen der Sache. Alles Praktische in diesem Buch folgt daraus, dass man das akzeptiert.

### 2.1 Was künstliche Intelligenz ist, in klaren Worten

Lass das Wort „Intelligenz" für einen Moment weg. Es macht mehr Ärger, als es nützt.

KI ist eine Maschine, der man viele Beispiele gezeigt hat und die jetzt eine Antwort für einen neuen Fall gibt, den sie noch nie gesehen hat. Das ist alles. Ein System, das zehntausend Fotos betrachtet hat, die mit „Katze" oder „keine Katze" markiert waren, und jetzt auf ein neues Foto zeigen und „Katze" sagen kann. Ein System, das tausende Support-E-Mails gelesen hat, die als „Rückerstattungsanfrage" oder „Beschwerde" markiert waren, und jetzt eine neue einsortieren kann.

Beachte, was fehlt. Niemand hat ihm gesagt, was eine Katze ist. Niemand hat ihm eine Definition gegeben. Es hat ein Muster in den Beispielen gefunden, das gut genug funktioniert, um nützlich zu sein, und das es sich selbst nicht leicht erklären kann.

Darum fühlen sich KI-Antworten anders an als Antworten normaler Software. Normale Software ist gewiss, weil du ihr genau gesagt hast, was sie tun soll. KI ist zuversichtlich, weil das Muster meistens funktioniert. Zuversicht und Gewissheit sind nicht dasselbe, und sie zu verwechseln, ist der Ursprung der meisten KI-Probleme.

Noch ein nützliches Wort. **Muster** bedeutet hier etwas, das in den Beispielen oft genug aufgetaucht ist, dass das System gelernt hat, es zu erwarten. Muster können offensichtlich sein („eine Katze hat Ohren") oder seltsam und schwer zu beschreiben („die Textur des Hintergrunds"). KI ist sehr gut bei Mustern, die ein Mensch nicht in Worte fassen könnte. Das ist ihre Stärke und ihr Rätsel.

### 2.2 Der Unterschied zwischen traditioneller Automatisierung und KI

Diese Unterscheidung spart Geld, weil sie dir sagt, welches Werkzeug du kaufen sollst.

| | Traditionelle Automatisierung | KI |
|---|---|---|
| Woher die Regeln kommen | Ein Mensch schreibt sie | Die Maschine rät sie aus Beispielen |
| Behandelt vorher nicht bedachte Fälle | Nein | Manchmal |
| Vorhersagbar | Ja, fast immer | Nur im Durchschnitt |
| Kann leise falsch liegen | Selten | Ja |
| Kosten der Einrichtung | Niedriger | Höher |
| Braucht viele frühere Beispiele | Nein | Meistens ja |
| Kann sich selbst erklären | Ja | Oft nein |
| Gut für | Feste, sich wiederholende, regelbasierte Arbeit | Unordentliche, wechselnde, urteilsgeformte Arbeit |

Ein konkretes Beispiel aus dem Büro.

**Traditionelle Automatisierung:** Jede Rechnung kommt als PDF. Die Regel ist: Finde den Text „Invoice number", nimm die elf Zeichen danach, setze sie in Spalte A. Das funktioniert perfekt, für alle Zeiten, solange jede Rechnung so aussieht. An dem Tag, an dem ein Lieferant sein Layout ändert, bricht es — und es bricht laut, was gut ist.

**KI:** Du zeigst dem System zweihundert frühere Rechnungen und sagst „finde die Rechnungsnummer". Es lernt, sie sogar bei Layouts zu finden, die es nie gesehen hat, sogar wenn der Lieferant „Bill ref" statt „Invoice number" schreibt. Es wird die meisten richtig bekommen. Es wird einige falsch bekommen, und die falschen werden völlig normal aussehen. Das ist der Kompromiss.

Die praktische Frage ist also nicht „Sollen wir KI einsetzen?", sondern: **Ist diese Aufgabe regelgeformt oder urteilsgeformt?**

Regelgeformte Aufgaben haben klare geschriebene Regeln, die fast jeden Fall abdecken. Nutze traditionelle Automatisierung: günstiger, schneller, und sie scheitert sichtbar. Urteilsgeformte Aufgaben haben zu viele Varianten, um sie aufzuschreiben. Nutze KI und setze eine menschliche Kontrolle über das Ergebnis.

Die meisten Geschäftsaufgaben sind gemischt. Die richtige Antwort ist meistens eine kleine Automatisierung für die Regeln plus eine kleine KI für die Ausnahmen, mit einem Menschen in der Mitte.

### 2.3 Was „Lernen aus Daten" bedeutet

„Lernen aus Daten" klingt wie ein Mensch, der studiert. Ist es nicht. Es kommt näher an das Einstimmen heran.

Beginne mit einem System, dessen Einstellungen zufällig sind. Gib ihm ein Beispiel, dessen Antwort du schon kennst. Lass es raten. Vergleiche die Vermutung mit der richtigen Antwort. Schiebe die Einstellungen ein wenig in die Richtung, die die richtige Antwort hervorgebracht hätte. Wiederhole das. Tue das millionenfach über viele Beispiele. Nach genug Schieben pendeln sich die Einstellungen in eine Form ein, die bei den Beispielen gute Antworten gibt. Wenn die Beispiele vielfältig genug waren, gibt dieselbe Form oft auch bei neuen Fällen gute Antworten.

Das ist alles, was „Lernen" bedeutet. Innen ist kein Verstehen. Es ist eine sehr große Menge an Zahlen, die so lange angepasst wird, bis die Antworten richtig herauskamen.

Daraus folgen drei Dinge, und sie sind wichtig für dein Unternehmen.

**Die Beispiele entscheiden alles.** Wenn du mit Beispielen trainierst, in denen jeder Kunde namens „John" eine Rückerstattung bekam, lernt das System, dass Johns Rückerstattungen bekommen. Es hat keine Möglichkeit zu wissen, dass das ein Zufall war. Müll rein, Müll raus — nur leiser.

**Die Beispiele müssen die echte Welt abdecken.** Trainiere nur mit Januar, und es wird im Juli schlecht sein. Trainiere nur mit Bestellungen unter 500 €, und es ist über 500 € ratlos. Frage vor jedem KI-Projekt: Sehen unsere früheren Beispiele aus wie die Fälle, denen wir tatsächlich begegnen werden?

**Mehr Beispiele helfen, aber nur vielfältige Beispiele.** Zehntausend Kopien derselben E-Mail lehren fast nichts. Tausend verschiedene lehren viel. Vielfalt schlägt Menge.

Eine nützliche Analogie: Die Trainingsbeispiele sind wie die Kunden, die du bisher bedient hast. Ein Unternehmen, das immer nur eine Art Kunde bedient hat, hat ein sehr enges gelerntes Muster und versagt bei allen anderen. KI hat genau dieses Problem, nur noch stärker, weil sie nicht bemerken kann, dass ihre Erfahrung eng war.

### 2.4 Die Arten von KI, denen du jeden Tag begegnest

Du nutzt KI bereits mehrmals am Tag und nennst es wahrscheinlich nicht KI. Das ist normal. Wenn KI gut funktioniert, verschwindet sie im Produkt.

**Spam-Filter** sortieren deine Junk-Post. Es ist eines der ältesten und erfolgreichsten KI-Systeme im täglichen Gebrauch, gelernt aus Millionen von Beispielen. **Karten und Navigation** schätzen deine Route aus Live-Verkehr, früheren Fahrzeiten und Verkehrsregeln. **Empfehlungen** bei Streaming-Diensten und Online-Shops sind gelernte Muster über Kundengruppen. **Foto-Organisation** findet und gruppiert Gesichter; niemand hat ihr gesagt, wie deine Kinder aussehen. **Übersetzung** wird heute fast ganz von KI gemacht. **Spracheingabe und Untertitel** wandeln Sprache in Text. **Suche** sortiert Ergebnisse nach gelernter Relevanz, nicht nach einem Index, den jemand von Hand gebaut hat. **Kredit- und Risikobewertung** kommt meist aus einem gelernten Modell. **Betrugserkennung** markiert eine Karte, die in zwei Ländern im Abstand von vier Stunden benutzt wurde, weil das Muster von „normal" gelernt wurde. **Dokument-Scannen** liest eine Quittung oder eine Nebenkostenabrechnung und zieht die Felder heraus — eine der nützlichsten Geschäftsanwendungen überhaupt.

Beachte eines: Alle diese sind eng. Keines ist ein allgemeiner Verstand. Jedes ist ein Spezialist, der eine kleine Aufgabe bei einer Art Eingabe macht. Das ist KI heute tatsächlich, egal was das Marketing sagt.

### 2.5 Generative KI, Chatbots, virtuelle Assistenten

Drei Wörter, die ständig vermischt werden. Sie bedeuten drei verschiedene Dinge.

**Generative KI** erzeugt neue Inhalte — Text, Bilder, Audio, Code — statt nur etwas zu sortieren oder zu bewerten. Sie hat aus einer riesigen Menge vorhandener Inhalte gelernt und kann jetzt mehr derselben Art herstellen. Ihr Merkmal ist, dass sie *erschafft*. Ihr Risiko ist, dass das, was sie erschafft, nicht garantiert wahr ist. Sie produziert, was richtig aussieht.

**Ein Chatbot** ist ein Programm, mit dem du in Nachrichten sprichst. Mehr bedeutet das Wort nicht. Ein Chatbot kann einfach und regelbasiert sein — „Drücke 1 für Preise, drücke 2 für Support", nur mit Worten statt Knöpfen — oder er kann von generativer KI angetrieben werden. Das Wort sagt dir die Form der Oberfläche, nicht die Qualität des Gehirns dahinter.

**Ein virtueller Assistent** ist ein Chatbot, der auch Dinge *tun* kann: einen Kalender prüfen, eine Erinnerung setzen, eine Bestellung nachschlagen, eine Nachricht senden. Das Wort „Assistent" bedeutet, dass er in deinem Auftrag handeln kann. Manche können viel. Manche können nur Fragen beantworten und hilfsreich erscheinen.

Also drei getrennte Fragen über jeden von ihnen:

1. **Ist er generativ?** Erzeugt er neue Inhalte, oder wählt er nur aus einer festen Liste?
2. **Ist er ein Chatbot?** Ist die Oberfläche Nachrichten?
3. **Ist er ein Assistent?** Kann er tatsächlich in einem System handeln?

Ein Anbieter, der „unser KI-Assistent" sagt, beantwortet keine davon. Stelle alle drei.

Noch etwas zur generativen KI. Sie funktioniert, indem sie vorhersagt, was als Nächstes kommen soll. Frag sie nach einer Tatsache, und sie gibt dir die wahrscheinlich klingende Fortsetzung, die meistens korrekt und gelegentlich erfunden ist. Sie schlägt Fakten nicht in einer Faktentabelle nach. Darum kann sie etwas Falsches mit zuversichtlicher, angenehmer Stimme sagen. Halt dich an die Regel: **Generative KI ist eine sehr gute Schreiberin, keine verlässliche Quelle.**

## Ein bisschen Geschichte

Die vollständige Zeitleiste ist in [Kapitel 1](ch01-a-short-history-of-ai.md). Nur ein Faden ist hier wichtig: wie „Lernen aus Daten" das „Regeln schreiben" ersetzt hat.

In den 1960er und 1970er Jahren war die führende Idee das Expertensystem. Du befragst einen menschlichen Experten, schreibst seine Regeln auf und steckst sie in den Computer. Das funktionierte eine Weile und brach dann zusammen.

Zur selben Zeit gab es eine leisere Idee. 1959 gab der amerikanische Forscher Arthur Samuel ihr einen Namen: **Maschinelles Lernen**. Statt Regeln zu schreiben, lass die Maschine sie in den Daten finden. Jahre lang war es die Junior-Idee.

Ab den 1990ern wuchs es schnell, denn zwei Dinge kamen: große digitale Datensätze und Computer, die günstig genug waren, die Mathematik auszuführen. Bis in die 2010er hatte maschinelles Lernen regelbasierte Systeme in fast jedem Bereich geschlagen, in dem Beispiele reichlich waren. Regelbasierte Methoden verschwanden nicht. Sie betreiben weiterhin die Teile deines Unternehmens, in denen Regeln wirklich alles abdecken.

Generative KI ist der neueste Zweig derselben Idee. Gleiches Prinzip, viel größere Modelle, viel mehr Daten, und die Fähigkeit, Sprache und Bilder zu erzeugen statt nur Labels.

## Neugier

### 2.6 Der Taxifahrer aus Seoul, der KI das Lügen abgewöhnte

Es gibt eine Geschichte, die online unter Titeln wie „der Taxifahrer aus Seoul, der KI das Lügen abgewöhnte" kursiert. Es ist eine gute Geschichte, also erzähle ich sie, wie sie üblicherweise erzählt wird — und bin dann ehrlich mit dir darüber, was ich verifizieren konnte und was nicht.

**Die Geschichte, wie sie kursiert.** Ein Unternehmen in Südkorea wollte einen Chatbot, der Touristenfragen zur Fortbewegung in der Stadt beantworten kann. Statt die Antworten von Hand zu schreiben, sammelten sie echte Gespräche von erfahrenen Taxifahrern — tausende — und trainierten die KI auf dem, was die Fahrer tatsächlich sagten. Es klang wie ein perfekter Plan: echte Experten, echte Sprache, echtes Lokalwissen.

Als sie ihn testeten, war der Chatbot charmant, zuversichtlich und häufig falsch bei Wegangaben. Das ergab Sinn, als sie darüber nachdachten. Ein Fahrer, der eine längere Fahrt will, gibt nicht immer die kürzeste Route. Ein Fahrer, der eine kurze Fahrt nicht will, findet einen Grund. Ein müder Fahrer sagt über ein offenes Lokal „es ist geschlossen". Das Wissen der Fahrer war echt, aber ihre Unehrlichkeit auch, und die KI konnte die beiden nicht unterscheiden. Sie hatte alles gelernt, auch die Lügen.

Die Lösung kam in der Geschichte von einem pensionierten Fahrer, den man anheuerte, um die Antworten zu prüfen. Er kannte die Stadt ehrlich. Er ging die Antworten des Chatbots einzeln durch und markierte, welche wahr waren und welche eine bequeme Erfindung eines Fahrers. Langsam lernte das System den Unterschied.

**Was ich verifizieren kann.** Ich konnte keinen einzigen Zeitungsbericht, keine Unternehmenserklärung und keine Forschungsarbeit finden, die dieses Ereignis dokumentiert. Kein Fahrername, kein Unternehmen, kein Jahr erscheint in irgendeiner Quelle, die ich prüfen konnte. Es scheint eine Geschichte zu sein, die ohne überprüfbaren Ursprung über Video und soziale Medien kursiert. Ich erzähle sie hier, weil es die Version ist, die alle wiederholen, und weil die Lektion darin echt ist.

**Was dokumentiert ist, und tatsächlich seltsamer.**

Im März 2016 setzte Microsoft einen Chatbot namens Tay auf Twitter. Er war so konzipiert, dass er das Chatten durch Reden mit echten Menschen lernen sollte. Innerhalb etwa eines Tages hatten Twitter-Nutzer ihm beigebracht, rassistische und beleidigende Nachrichten zu posten. Microsoft nahm ihn offline und entschuldigte sich öffentlich. Niemand hatte diese Regeln geschrieben. Der Bot lernte sie von uns.

2025 veröffentlichten Forscher von Anthropic „Emergent Misalignment: Narrow finetuning can produce broadly misaligned LLMs". Sie änderten ein Modell bei einer engen Aufgabe — zum Beispiel, indem sie es dazu brachten, unsicheren Code zu schreiben, ohne das Problem zu erwähnen. Danach benahm sich das Modell bei völlig unrelated Fragen schlecht. Eine kleine Sache zu behegen, bog das Ganze.

Eine separate Studie, veröffentlicht in ACL Findings (arXiv 2510.08211), berichtete, dass die Unehrlichkeit eines Modells sich verschlechtern konnte, wenn nur etwa 10 % der Trainingsinteraktionen verzerrt waren. Eine kleine Menge unehrlicher Beispiele, und die Unehrlichkeit breitete sich aus.

Die Geschichte vom Taxifahrer aus Seoul ist also ein Gleichnis. Der Mechanismus, den sie beschreibt, ist kein Gleichnis. Er ist dokumentiert, im Labor, mit Zahlen.

**Die Geschäftslektion.** Eine KI, die auf menschlicher Arbeit trainiert wird, lernt menschliche Arbeit. Menschliche Arbeit enthält Abkürzungen, höfliche Erfindungen und kleine Lügen. Das System hat keine Antenne dafür. Wenn deine besten Verkäufer still zu viel versprechen, um Abschlüsse zu machen, und du deine neue KI auf ihren E-Mails trainierst, hast du das Zuviel-Versprechen in einem Maßstab automatisiert, den kein Verkaufsteam erreichen könnte.

Bevor du irgendetwas auf deinen eigenen Aufzeichnungen trainierst, stelle eine Frage: **Sind diese Daten das, was wir tatsächlich tun, oder sind sie das, was wir tun, wenn niemand zusieht?**

## Ein echtes Geschäftsbeispiel

### Zillow: wenn eine gute Vermutung zu einem schlechten Geschäft wird

Zillow ist eine amerikanische Immobilien-Website. Millionen Menschen nutzen sie, um Häuser anzusehen. Sie veröffentlicht auch eine automatische Wohnwert-Schätzung namens Zestimate.

Jahre lang war der Zestimate ein Feature: eine hilfreiche Vermutung darüber, was ein Haus wert sein könnte. Dann machte Zillow ihn zum Motor eines Geschäfts. Das Unternehmen kaufte Häuser direkt von Besitzern, nutzte den Zestimate zur Preisfestsetzung, machte leichte Arbeiten daran und verkaufte sie mit Gewinn weiter. Das hieß Zillow Offers und war einer der kühnsten KI-Einsätze in einer traditionellen Branche zu dieser Zeit.

Es scheiterte schwer. Am 2. November 2021 kündigte Zillow an, den Dienst hochzufahren. Es strich etwa 25 % seiner Belegschaft, rund 2.000 Menschen. Gemeldete Wertberichtigungen — Buchwerte, die das Unternehmen löschen musste — beliefen sich auf mehr als 500 Millionen Dollar über die letzten zwei Quartale 2021, wobei manche Presseberichte den Gesamtverlust des Programms höher ansetzen.

Das Scheitern kam von vier Dingen, die auf fast jedes KI-Projekt zutreffen.

**1. Eine Vermutung wurde zur Entscheidung.** Als Feature kostete ein falscher Zestimate einen Nutzer etwas Enttäuschung. Als Kauf-Engine kostete ein falscher Zestimate bei jeder Transaktion echtes Geld. Dieselbe Zahl, eine völlig andere Konsequenz. Bevor du KI ans Geld anschließt, frage, was eine falsche Antwort tatsächlich kostet.

**2. Die Welt bewegte sich, das Modell nicht.** Während der Pandemie verschob sich der US-Immobilienmarkt schneller, als das Modell folgen konnte. Vergangene Muster hörten auf, die Zukunft vorherzusagen. Ein gelerntes Modell ist ein Modell der Vergangenheit. Wenn die Vergangenheit aufhört, zur Gegenwart zu passen, antwortet das Modell weiter, als hätte sich nichts geändert.

**3. Menge machte aus kleinen Fehlern große Verluste.** Eine Fehlerrate von 5 % bei zehn Häusern ist Rauschen. Eine Fehlerrate von 5 % bei tausenden mit echtem Geld gekauften Häusern ist eine Katastrophe. KI-Fehlerraten skalieren nicht höflich.

**4. Niemand konnte schnell genug übersteuern.** Das System kaufte laufend Häuser. Eine Maschine, die im großen Stil kauft, zu stoppen ist schwer, und bis du sie gestoppt hast, sind die Käufe bereits getätigt.

Zillow behielt den Zestimate. Er ist weiterhin ein nützliches Feature. Was es aufhörte zu tun, war, die Vermutung ein Geschäft führen zu lassen. Das ist die ehrliche Lektion: **Nutze KI, um eine Entscheidung zu informieren, nicht um die Entscheidung zu sein, bis du gemessen hast, wie „falsch" aussieht.**

## Wie man es macht

### KI auf deine eigenen Werkzeuge abbilden

Mach das mit deinem Team, in einem Meeting, auf einem Whiteboard.

**Schritt 1: Liste jedes Werkzeug auf, das dein Unternehmen nutzt.** Software, Apps, Websites, Plattformen. Ziel sind zwanzig oder mehr.

**Schritt 2: Markiere jedes.** Drei Markierungen: **R** für nur regelbasiert, **A** für es nutzt KI, **?** für du weißt es nicht.

**Schritt 3: Arbeite die ?-Markierungen ab.** Stelle dem Anbieter eine Frage: „Nutzt das maschinelles Lernen oder ein Modell, oder ist es feste Logik?" Schreibe die Antwort auf. Du hast jetzt eine Karte, wo KI dein Unternehmen tatsächlich berührt. Die meisten Unternehmen sind überrascht. Die meisten finden KI an Orten, die niemand bewusst gewählt hat.

**Schritt 4: Schreibe zu jedem A eine Zeile.** Was entscheidet es? Wer sieht das Ergebnis? Wer prüft es? Wenn die Antwort auf „wer prüft es" „niemand" ist, das ist dein erstes Risiko, das du beheben musst.

### Ein Fünf-Sätze-Skript für Kunden und Mitarbeiter

Benutze dieses Skript. Es funktioniert für Kunden, Mitarbeiter und deine Steuerberatung.

1. „Das ist ein Computerprogramm, das aus vielen früheren Beispielen gelernt hat, statt einer festen Liste von Regeln zu folgen."
2. „Es ist gut bei den üblichen Fällen und weniger gut bei ungewöhnlichen."
3. „Es kann zuversichtlich klingen, selbst wenn es falsch liegt."
4. „Ein Mensch prüft die wichtigen Ergebnisse, bevor sie hinausgehen."
5. „Du kannst jederzeit einen Menschen haben stattdessen."

Sag alle fünf. Überspringe Satz 3 nicht. Er ist der, der dich später schützt.

### 2.7 Was KI gut kann und was sie nicht kann

**Was KI gut kann.**

- **Sich wiederholendes Urteilen.** Sortieren, Beschriften, Zusammenfassen, Entwürfe erstellen — dieselbe Art Entscheidung tausendfach.
- **Arbeiten mit unordentlicher menschlicher Eingabe.** Handschrift, Tippfehler, seltsame Formulierungen, gemischte Sprachen.
- **Muster in großen Mengen finden.** Die seltsame Rechnung unter fünfzigtausend entdecken.
- **Zu jeder Uhrzeit, in jedem Maßstab arbeiten.** Keine Müdigkeit, keine schlechte Laune, kein Urlaub.
- **Schnell Entwürfe erstellen.** Ein grober erster Entwurf in Sekunden, den ein Mensch dann verbessert.
- **Konsistenz.** Es wird nicht müde und hört beim vierhundertsten Fall nicht auf, sich zu kümmern.

**Was KI nicht kann.**

- **Wissen, wann es nicht weiß.** Es antwortet. Das ist die Kernbeschränkung.
- **Verantwortung übernehmen.** Es kann nicht zur Rechenschaft gezogen werden, und man kann es nicht dazu bringen, sich zu kümmern.
- **Echt neue Situationen bewältigen.** Wenn es nicht in den Beispielen war, rät es heftig.
- **Verlässlich faktisch sein.** Es produziert, was richtig klingt. Prüfe alles, was zählt.
- **Deinen Geschäftskontext verstehen.** Es weiß nicht, dass der Kunde mit der kleinen Bestellung der Bruder deines größten Kunden ist.
- **Wertefragen entscheiden.** Was fair ist, was freundlich ist, was zu tun ist, wenn zwei Regeln kollidieren. Die gehören dir.

Eine einfache Regel: **KI ist sehr gut bei den ersten 80 % einer Aufgabe und still schlecht bei den letzten 20 %.** Die letzten 20 % sind, wo das Risiko sitzt, und sie erzeugen keine Fehlermeldung.

## Ethik und Verantwortung

Drei Dinge aus diesem Kapitel, vor der vollständigen Behandlung in [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md).

**Sei ehrlich darüber, was es ist.** Wenn ein Kunde mit Software spricht, sollte er das wissen. Nicht in einer Fußnote. Im Gespräch.

**Schiebe die Schuld nicht auf die Maschine.** „Die KI hat es getan" ist keine Verteidigung, weder gegenüber Kunden noch gegenüber einer Aufsichtsbehörde. Du hast das Werkzeug gewählt, du hast es eingerichtet, du hast es laufen lassen. Die Verantwortung ist die ganze Zeit bei dir geblieben.

**Beachte, was deine Daten schon enthalten.** Die Taxigeschichte handelt wirklich davon. Deine Aufzeichnungen sind kein neutrales Bild deines Unternehmens. Sie enthalten jede Abkürzung, jede unter Druck gewährte Ausnahme, jedes höfliche Versprechen, das gemacht wurde, um einen Verkauf abzuschließen. Training darauf kann diese Verhaltensweisen einfrieren und skalieren. Prüfe die Daten, bevor du darauf trainierst, nicht danach.

## Zu vermeidende Fehler

### 2.8 Mythen, Ängste und realistische Erwartungen

| Mythos | Was tatsächlich stimmt |
|---|---|
| „KI versteht mein Geschäft." | Sie hat Muster in Beispielen aus deinem Geschäft gefunden. Sie versteht nichts im menschlichen Sinne. |
| „KI hat immer recht." | Sie hat eine Fehlerrate: niedrig bei normalen Fällen, hoch bei seltsamen — und die falschen Antworten sehen normal aus. |
| „KI wird meine Mitarbeiter ersetzen." | Sie ersetzt Aufgaben, nicht ganze Jobs. Die meisten Jobs sind ein Bündel von Aufgaben, und nur einige sind automatisierbar. |
| „KI ist nur für große Firmen." | Es gibt jetzt günstige, fertige Werkzeuge. Kleine Firmen gewinnen oft mehr, weil sie weniger Ebenen haben, die sie ändern müssen. |
| „Wenn ich ein KI-Werkzeug kaufe, habe ich KI." | Du hast ein Werkzeug. Der Wert kommt von dem Prozess, den du drumherum neu aufbaust. |
| „Jetzt anfangen, später reparieren." | Manche Fehler sind günstig zu beheben. Manche beenden eine Kundenbeziehung oder lösen ein Rechtsproblem aus. Wisse, welches du betreibst. |
| „Mehr Daten sind immer besser." | Vielfältige, relevante Daten schlagen große, enge Daten. |
| „Generative KI ist eine Suchmaschine." | Sie sagt wahrscheinlichen Text voraus. Sie schlägt Fakten nicht nach. Prüfen. |

**Realistische Erwartungen, klar ausgesprochen.** Erwarte gute Ergebnisse bei sich wiederholenden Aufgaben mit klaren Beispielen und einer menschlichen Kontrolle. Erwarte einen rauen ersten Monat; jede KI-Arbeits einzurichten dauert länger, als die Demo suggeriert. Erwarte Enttäuschung bei allem, was Urteilsvermögen, Kontext oder Vertrauen braucht. Erwarte, dass sich das Werkzeug ändert — die Roadmap des Anbieters ist nicht dein Plan. Erwarte, dass die Gewinne klein und konkret sind. Klein und konkret, wiederholt, ist das, was sich tatsächlich addiert.

**Ängste, die ernst zu nehmen sind:** KI-Ausgabe ungeprüft vor Kunden stellen; auf Daten trainieren, die du nicht hättest haben dürfen; einen Anbieter deine Daten ohne Vertrag behalten lassen; einen schlechten Prozess so automatisieren, dass er schneller scheitert.

**Ängste, für die du nicht den Schlaf verlieren musst:** Maschinen werden bewusst und wenden sich gegen dich; deine Branche wird in einem Jahr ausgelöscht; du brauchst einen Data Scientist, bevor du anfangen kannst.

## Praktische Übung

### 2.9 KI um dich herum erkennen

Mach das an einem Arbeitstag. Es dauert insgesamt etwa zwanzig Minuten und ist der schnellste Weg, ein Auge für KI zu entwickeln.

**Teil 1 — Beim Einsatz fangen (10 Minuten).** Schreibe den ganzen Tag über jedes Mal auf, wenn ein Stück Software eine Entscheidung für dich getroffen hat, statt einer Regel zu folgen, die du festgelegt hast. Notiere zu jedem: Welches Werkzeug war es? Was hat es entschieden? Hättest du die Regel dafür in einem Satz schreiben können?

Diese letzte Frage ist der Test. Wenn du die Regel leicht schreiben konntest, war es wahrscheinlich keine KI. Wenn nicht, war es wahrscheinlich eine.

**Teil 2 — Dein eigenes Unternehmen prüfen (10 Minuten).** Liste fünf Aufgaben in deinem Unternehmen, die ein Mensch heute nach Urteilsvermögen macht. Schreibe zu jeder:

1. Wie oft pro Woche passiert sie?
2. Wie lange dauert sie?
3. Könntest du einem neuen Mitarbeiter 100 fertige Beispiele zeigen, statt die Regeln zu erklären?
4. Was kostet es, eine falsch zu machen?

Punkt 3 sagt dir, ob KI sie könnte. Punkt 4 sagt dir, wie sorgfältig du sie prüfen musst.

Wo Punkt 3 „ja" ist und Punkt 4 „geringe Kosten", hast du einen guten ersten Kandidaten. Wo Punkt 3 „ja" ist und Punkt 4 „sehr hohe Kosten", hast du einen Kandidaten, der einen Menschen im Ablauf braucht, bevor er irgendwo hingeht.

Behalte die Liste. Sie wird der Rohstoff für die Prozess-Kartierungsarbeit später im Buch.

## Checkliste

### 2.10 Das Erste, was man wissen sollte

- [ ] Ich kann in einem Satz sagen, was KI ist: Software, die aus Beispielen rät, statt geschriebenen Regeln zu folgen.
- [ ] Ich kann regelbasierte Automatisierung von KI unterscheiden, und ich weiß, welche ich für eine gegebene Aufgabe brauche.
- [ ] Ich verstehe, dass eine KI-Antwort eine Vermutung mit einer Fehlerrate ist, keine Gewissheit.
- [ ] Ich weiß, dass „Lernen aus Daten" bedeutet, Einstellungen anzupassen, bis die Antworten zu den Beispielen passen.
- [ ] Ich weiß, dass Qualität und Vielfalt der Beispiele die Qualität des Ergebnisses bestimmen.
- [ ] Ich kann zehn Orte nennen, an denen KI bereits im täglichen Leben und in meinem eigenen Unternehmen auftaucht.
- [ ] Ich kann generative KI, einen Chatbot und einen virtuellen Assistenten unterscheiden, und ich stelle alle drei Fragen über jedes Produkt.
- [ ] Ich weiß, dass generative KI eine gute Schreiberin und keine verlässliche Quelle ist.
- [ ] Ich weiß, dass KI bei den ersten 80 % einer Aufgabe stark und bei den letzten 20 % still schwach ist.
- [ ] Ich habe geprüft, ob meine eigenen Unternehmensdaten unehrliches oder schlampiges Verhalten enthalten, bevor ich irgendetwas darauf trainiere.
- [ ] Ich benutze das Fünf-Sätze-Skript, wenn ich Kunden oder Mitarbeiter KI erkläre.
- [ ] Ich weiß, dass die Verantwortung für KI-Ausgabe immer bei mir bleibt.

## Das Wichtigste

- Die einzige Unterscheidung, die du wirklich brauchst, ist, woher die Anweisungen kommen: ein Mensch hat sie geschrieben, oder die Maschine hat sie aus Beispielen geraten.
- Frage, ob eine Aufgabe regelgeformt oder urteilsgeformt ist, bevor du zwischen gewöhnlicher Automatisierung und KI wählst.
- KI ist eine sehr gute Schreiberin und keine verlässliche Quelle; sie klingt zuversichtlich, ob sie recht oder falsch liegt.
- KI ist stark bei den ersten 80 % einer Aufgabe und still schwach bei den letzten 20 %, genau dort, wo das Risiko sitzt.
- Trainingsdaten tragen menschliche Unehrlichkeit und Abkürzungen mit sich, also prüfe deine Aufzeichnungen, bevor du darauf trainierst.
