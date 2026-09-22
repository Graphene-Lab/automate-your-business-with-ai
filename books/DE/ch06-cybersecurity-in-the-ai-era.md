# Kapitel 6 — Cybersicherheit im KI-Zeitalter

## Einfach gesagt

Fast die gesamte Geschichte der geschäftlichen Datenverarbeitung bedeutete Sicherheit eines: Fremde aus deinem Gebäude halten. Du hattest eine abgeschlossene Tür, ein Passwort, eine Firewall. Der Böse war draußen. Deine Daten waren drinnen.

Künstliche Intelligenz hat diese Grenze verwischt. Wenn heute ein Mitarbeiter eine Kundenliste, einen Vertrag oder eine Gehaltstabelle in ein Online-KI-Werkzeug tippt, verlässt dieser Text das Gebäude. Er wandert zu Computern, die jemand anderem gehören. Vielleicht werden sie dort gespeichert. Vielleicht liest ihn das Support-Personal. Vielleicht bleibt er Monate liegen. In manchen Fällen wird er benutzt, um das Produkt dieser Firma zu verbessern. Die meisten Leute denken nie darüber nach, weil das Werkzeug wie ein Suchfeld aussieht. Es ist kein Suchfeld. Es ist ein Dienst, betrieben von einer Firma, auf Maschinen, die du nicht kontrollierst.

KI verändert das Sicherheitsbild in zwei Richtungen zugleich.

**Die Angreifer sind besser geworden.** Ein Sprachmodell gibt einem Verbrecher drei Dinge, die früher teuer waren: Tempo, Maßstab und Schliff. Eine Phishing-Mail, die früher wie eine schlechte Übersetzung aussah, lässt sich jetzt in Sekunden in flüssigem Deutsch oder Japanisch schreiben, personalisiert mit Details aus einem öffentlichen Profil. Eine Stimme lässt sich aus ein paar Sekunden einer Aufnahme kopieren; so haben in gemeldeten Betrugsfällen Finanzangestellte Überweisungen freigegeben, weil der Anrufer klang wie der eigene Chef. Nichts davon braucht ein Genie. Es braucht ein Abo.

**Deine Angriffsfläche ist größer geworden.** „Angriffsfläche" ist nur ein Begriff für die Zahl der Stellen, an denen jemand eindringen kann. Jede KI-Funktion, die du hinzufügst, ist eine neue Tür: Chat-Werkzeuge, Plugins, die an deine E-Mail reichen, Agenten, die Ordner lesen und Nachrichten senden, Modelle, die mit deinen Unterlagen trainiert werden, Anbieter, die eine Kopie jedes Prompts und jeder Antwort behalten. Vor zwei Jahren hattest du eine Haustür. Jetzt hast du vielleicht vierzig, und die meisten davon hat dein eigenes Personal geöffnet, ohne jemandem Bescheid zu sagen.

Noch eine Idee ordnet alles andere. Sicherheit schützt drei Dinge, bekannt unter drei kurzen Worten.

- **Vertraulichkeit.** Nur die richtigen Leute sehen die Daten.
- **Integrität.** Die Daten wurden nicht heimlich verändert.
- **Verfügbarkeit.** Das System funktioniert, wenn du es brauchst.

Die meisten Inhaber behandeln KI-Sicherheit nur als Vertraulichkeitsproblem. Ist es nicht. Ein Wettbewerber, der dein Modell vergiftet, ist ein Integritätsproblem. Ein Anbieter, dessen Systeme ausfallen und deine Zahlungen wochenlang blockieren, ist ein Verfügbarkeitsproblem — und genau das hat in der Geschichte später in diesem Kapitel den größten Schaden angerichtet. Wenn du dir ein KI-Werkzeug ansiehst, stell alle drei Fragen.

Eine Warnung. Der Gedanke „wir sind zu klein, um angegriffen zu werden" stimmt nicht. Moderne Angriffe sind automatisiert: Software scannt das ganze Internet nach unverschlossenen Türen, so wie ein Dieb jedes Auto auf einem Parkplatz ausprobiert. Du wirst nicht ausgesucht, weil du interessant bist. Du wirst getroffen, weil du ein leichtes Ziel warst, und weil du Kundendaten, Bankdaten und Steuerunterlagen mit sehr wenig Schutz darum herum aufbewahrst.

Die gute Nachricht: Der meiste Schutz, den du brauchst, ist keine Hochtechnologie. Es ist eine kurze Liste langweiliger Gewohnheiten, eine Karte, wohin deine Daten gehen, und ein paar Kontrollen an der richtigen Stelle.

Die rechtliche Seite personenbezogener Daten steht in [Kapitel 10](ch10-privacy-and-gdpr.md). Personal, das KI-Werkzeuge ohne Genehmigung nutzt — „Shadow-KI" —, in [Kapitel 9](ch09-third-party-services-and-shadow-ai.md). Der Schritt-für-Schritt-Aufbau in [Kapitel 20](ch20-implementing-ai-securely.md).

## Ein wenig Geschichte

Die Sicherheitsgeschichte wiederholt eine Lektion: Der Perimeter wandert, und die Verteidiger bemerken es langsam.

Im Jahr **1988** legte der Morris-Wurm rund zehn Prozent der verbundenen Computer des frühen Internets lahm. Geschrieben von einem Doktoranden, nicht von einem Verbrecher, und er bewies, dass sich ein selbst verbreitendes Programm binnen Stunden über den ganzen Planeten bewegen kann. Durch die **1990er und 2000er** war die Standardantwort das Perimeter-Modell: eine Firewall am Rand, Antivirus auf jedem PC, Daten auf einem Server in einem Schrank. Es funktionierte, solange die Daten blieben, wo du sie hingelegt hattest.

Im Jahr **2013** wurde der US-Einzelhändler Target gehackt. Die Angreifer brachen nicht bei Target ein. Sie brachen bei einer kleinen Firma ein, die Heizungs- und Klimaanlagen für seine Filialen lieferte, nahmen die Zugangsdaten dieser Firma und gelangten so an Targets Zahlungssysteme. Rund 40 Millionen Kartennummern wurden gestohlen. Die Lektion handelte von Verbindung, nicht von Code: Dein Risiko umfasst jetzt jeden, den du anstöpselst.

Im Jahr **2016** stellte Microsoft einen Chatbot namens Tay in die sozialen Medien. Innerhalb eines Tages brachten Nutzer ihn dazu, beleidigendes Material zu posten, indem sie ihm ständig Nachrichten fütterten, und er wurde offline genommen. Niemand hat das Programm geknackt. Sie haben das geknackt, was das Modell las. Das ist der Keim der Prompt-Injektion, obwohl sie damals noch keinen Namen hatte.

Im Jahr **2017** verbreitete sich die NotPetya-Malware über ukrainische Buchhaltungssoftware und richtete weltweit Schaden in zweistelliger Milliardenhöhe an Dollar an — beim Schifffahrtsriesen Maersk, dem Pharmahersteller Merck und vielen anderen. Ein vergiftetes Glied in einer Software-Lieferkette wurde über Nacht jedermanns Problem.

Im Jahr **2020** entfernte das Remote-Arbeiten den physischen Perimeter beinahe über Nacht. Im Jahr **2022** machte ChatGPT generative KI binnen Wochen zu einem normalen Büro-Werkzeug, und das Personal begann, echte Arbeit in Werkzeuge ohne Firmenvertrag dahinter einzufügen. Im **September 2022** veröffentlichte der Sicherheitsforscher Simon Willison einen Beitrag mit dem Titel „Prompt-Injektionsangriffe gegen GPT-3" und gab einem Problem einen Namen, das die Leute längst sahen, aber nicht beschreiben konnten: Anweisungen, versteckt in Text, den ein Modell liest, und die die Anweisungen, die du ihm gegeben hast, überstimmen.

Im Jahr **2023** bedeuteten Open-Weight-Modelle, dass eine Firma KI auf eigener Hardware betreiben konnte, wie [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) erklärt. Im selben Jahr begannen Anbieter, „Agenten" auszuliefern, die handeln können statt nur zu antworten, was den Preis jedes Fehlers erhöhte. Im Jahr **2024** wurde das Anbieter-Risiko unmöglich zu ignorieren, wie im Neugier-Abschnitt unten erzählt. Ab **2025** kamen Agenten mit Werkzeugen und Zugangsdaten im Schlepptau, sodass die Explosionsradius einer falschen Berechtigung heute alles ist, was dieser Agent erreichen kann.

Lies die Zeitleiste als eine lange Argumentation. Jeder Schritt verlagerte das Vertrauen weg von einer verschlossenen Tür und hinein in eine Beziehung: ein Auftragnehmer, ein Anbieter, ein Plugin, ein Modell, ein Agent. Sicherheit hörte auf, eine Mauer zu sein, und wurde eine Frage danach, wen und was du angebunden hast.

## Neugier

### 6.8 Der Anbieter, der beinahe ein Gesundheitswesen lahmlegte

Am 12. Februar 2024 drangen Angreifer in Change Healthcare ein, eine Firma, die in den Vereinigten Staaten Arztrechnungen und Zahlungen verarbeitet. Nach einer Aussage, die der Vorstandsvorsitzende von UnitedHealth Group im Mai 2024 vor dem US-Kongress machte, betraten sie über ein Fernzugangs-Portal, das keine Multi-Faktor-Authentifizierung verlangte — die zweite Prüfung bei einem Login, die die meisten gestohlenen Passwörter am Funktionieren hindert. An der Haustür war keine clevere Malware. Da war ein gestohlenes Passwort und ein fehlendes zweites Schloss. Die Angreifer verbrachten neun Tage drinnen, bewegten sich leise und kopierten rund sechs Terabyte Daten heraus. Am 21. Februar schalteten sie Ransomware ein und blockierten die Systeme.

Change Healthcare ist eine Tochter von UnitedHealth Group und sitzt mitten in der amerikanischen Kette für Gesundheitszahlungen. Als sie stoppte, stoppte ein sehr großer Anteil der Arztabrechnungen, Apothekenzahlungen und Versicherungsgenehmigungen mit. Kleine Praxen kamen nicht an ihr Geld und waren binnen Wochen pleite; Branchenverbände meldeten Verluste der Leistungserbringer von mehreren zehn Millionen Dollar pro Tag im betroffenen Netzwerk. Große Namen, die mit dem Hack nichts zu tun hatten — Ketten-Apotheken, regionale Versicherer, ein Marinekrankenhaus — fanden ihren eigenen Betrieb blockiert, weil sie alle Daten durch denselben Mittelschleuser schickten.

UnitedHealth reichte bis Mitte März mehr als 2 Milliarden Dollar an Notfallkrediten für betroffene Leistungserbringer nach, und mehr als 6 Milliarden bis Mitte April. Berichten von Reuters und Wired zufolge wurde ein Lösegeld von rund 22 Millionen Dollar in Bitcoin an eine Wallet der kriminellen Gruppe ALPHV, auch BlackCat genannt, gezahlt, die UnitedHealth am 29. Februar als Angreifer bestätigte. Im Oktober 2024 schätzte UnitedHealth, dass bei etwa 190 Millionen Menschen die Daten betroffen waren, eine der größten jemals verzeichneten Datenpannen.

Warum kümmert das ein kleines Unternehmen, das nie eine Arztrechnung anfassen wird? Wegen der Frage, wer das eigentliche Opfer war. Die Krankenhäuser und Apotheken, die litten, wurden nicht gehackt. Viele von ihnen hatten gute Sicherheit. Sie wurden getroffen, weil eine Firma mitten in ihrem Arbeitsablauf gehackt wurde, und sie konnten ohne diese Firma nicht überleben. Ihre Sicherheit war nur so gut wie der am schlechtesten geschützte Anbieter in ihrer Kette.

Jetzt füge die Analyse-Perspektive hinzu, denn sie liegt näher, als es aussieht. 2024 legte OpenAI einen Vorfall offen, der überhaupt kein Einbruch in die eigenen Systeme war. Das Problem lag bei Mixpanel, einem Drittanbieter-Analysedienst auf der Entwickler-Website für dessen Anwendungsprogrammierschnittstelle. Analysedienste sind kleine Softwarestücke, die eine Firma auf ihre Website setzt, um Besuche zu zählen und zu sehen, wie Leute klicken. Dieser Anbieter wurde gehackt, und die Namen, E-Mail-Adressen und Geräteangaben einiger Kontoinhaber wurden preisgegeben. Chat-Inhalte, Passwörter und geheime Schlüssel nicht.

Der Schaden dort war begrenzt. Die Lektion nicht. Wenn du einen KI-Dienst kaufst, kaufst du auch jede Firma, auf die dieser Dienst sich stützt: seine Analysen, sein Hosting, seine Support-Werkzeuge, seine Plugins. Du erbst eine Lieferkette, die du nie gewählt hast und nie gehört haben magst.

## Ein echtes Geschäftsbeispiel

### Der Ingenieur, der den Chatbot um Hilfe bat

Im April 2023 berichtete Bloomberg, dass Samsung generative KI-Werkzeuge wie ChatGPT auf Firmenrechnern verboten habe. Der Grund war keine Risikotheorie. Ingenieure hatten vertraulichen Quellcode in einen öffentlichen Chatbot eingefügt, während sie nach einem Bug-Fix suchten, mehr als einmal, in einer Abteilung, die an Halbleitern arbeitete — einer der am strengsten gehüteten Code-Arten der Welt. Ein von Bloomberg geprüftes Memo merkte dem Vernehmen nach an, eine interne Umfrage habe ergeben, dass 65 Prozent der Befragten das Werkzeug bereits für ein Sicherheitsrisiko hielten.

Sieh das von der Seite des Ingenieurs. Nichts wurde gestohlen. Niemand brach ein. Ein Mensch hing an einem Problem fest, fand ein Werkzeug, das es in zehn Sekunden löste, und benutzte es. Das Werkzeug war ausgezeichnet. Das Urteilsvermögen war schlecht. Der Code gehörte ihm nicht zum Verschenken.

Das ist der häufigste KI-Sicherheitsfehler überhaupt, und er ist nicht exotisch. Er passiert in Anwaltskanzleien, wenn jemand den Vertrag eines Kunden einfügt, um ihn zusammenzufassen. In Steuerkanzleien mit einer Steuererklärung. In Agenturen mit einer unveröffentlichten Kampagne eines Kunden. In der Personalabteilung mit einem Stapel Lebensläufe. Das Muster ist immer gleich: ein hilfreiches Werkzeug, ein gehetzter Mensch und ein Copy-Paste, das eine Grenze überschreitet, die niemand gezogen hat.

Zwei Dinge folgen daraus. Erstens: Die Behebung ist nicht nur ein Verbot, denn ein Verbot ohne Alternative stoppt das Verhalten nicht; es versteckt es, was schlimmer ist, denn jetzt kannst du den Datenfluss nicht mehr sehen. Zweitens: Die Behebung ist nicht nur Schulung, denn ein Mensch in Eile um fünf Uhr abends erinnert sich nicht an eine vierzigseitige Richtlinie. Die Behebung besteht darin, den sicheren Weg zum einfachen Weg zu machen: ein zugelassenes Werkzeug, das schneller ist als das unsichere, plus eine Kontrolle, die die schlimmsten Daten aufhält, bevor sie gehen. Beides steht im nächsten Abschnitt.

## Wie man es macht

### 6.7 Wie du dich schützt: KI-Firewalls, Filter, Überwachung

Tu das der Reihe nach. Jeder Schritt hängt vom vorherigen ab.

**Schritt 1: Zeichne die Karte, bevor du irgendetwas kaufst.**
Nimm ein Blatt Papier. Listet jedes KI-Werkzeug auf, das dein Unternehmen berührt, auch die kostenlosen auf den Handys deiner Leute. Für jedes: welche Daten reingehen, was rauskommt, wo es gespeichert wird, wer der Anbieter ist, und ob du einen unterschriebenen Vertrag hast. Du wirst Werkzeuge finden, von denen du nichts wusstest. Das ist das wertvollste Sicherheitsdokument, das du dieses Jahr erstellst.

**Schritt 2: Lege eine Tür zwischen deine Leute und die KI-Dienste.**
Ein „KI-Gateway" oder „KI-Firewall" ist ein einzelner Punkt, durch den der gesamte KI-Verkehr läuft, damit du ihn siehst und kontrollieren kannst. Mainstream-Produkte tun das: Content-Safety- und Prompt-Shielding-Dienste der großen Cloud-Plattformen, Guardrails in Cloud-Modelldiensten, KI-fähige Gateways und Data-Loss-Prevention-Werkzeuge, die prüfen, was Mitarbeiter senden. Du musst wissen, dass es die Kategorie gibt und was sie dir kauft: ein Ort, um Werkzeuge zu erlauben oder zu blockieren, Inhalte zu prüfen und Protokolle zu führen.

**Schritt 3: Filtere, was rausgeht.**
Die wertvollste Kontrolle auf dieser Liste. Konfiguriere dein Gateway oder dein Data-Loss-Werkzeug so, dass es die Kategorien blockiert oder davor warnt, die niemals rausdürfen: Personalausweis- und Steuernummern, Bank- und Kartennummern, Gesundheitsinformationen, Gehaltsdateien, unterschriebene Verträge, Quellcode und vertrauliche Kundendokumente. Ein Pop-up „das sieht nach personenbezogenen Daten aus, bist du sicher?" stoppt für sich allein einen großen Teil der Unfälle, weil die meisten von ihnen Unfälle sind.

**Schritt 4: Filtere, was reinkommt.**
Das ist die Prompt-Injektions-Verteidigung, und sie hat eine goldene Regel: **lass ein KI-Werkzeug niemals auf Anweisungen handeln, die es in einem Dokument, einer E-Mail, einer Webseite oder einer Tabelle findet.** Ein Modell, das deinen Posteingang liest, soll zusammenfassen, nicht gehorchen. Wo ein Werkzeug handeln muss, verlange, dass ein Mensch bestätigt, bevor es läuft. Behandle jedes externe Dokument als nicht vertrauenswürdige Eingabe, so wie du einen Anhang eines Fremden behandelst.

**Schritt 5: Gib Agenten so wenig Macht wie möglich.**
Entscheide die Berechtigungen eines Agenten auf Papier, bevor du ihn verbindest. Nur-Lesen, wo möglich. Sein eigener Dienstkonto, nie ein geteiltes Administrator-Login. Ein Ordner, nicht das ganze Laufwerk. Eine Ausgabengrenze bei allem, was Geld kostet. Ein Zeitlimit. Ein namentlich festgelegter menschlicher Verantwortlicher. Wenn er nicht löschen muss, lass ihn nicht löschen. Gib dem Werkzeug die kleinste Menge an Schlüsseln, die es die Arbeit noch tun lässt.

**Schritt 6: Protokolliere alles und lies die Protokolle.**
Erfasse, wer welches KI-Werkzeug wann und wofür ungefähr benutzt hat — dann sieh es dir an. Ein wöchentlicher Fünfzehn-Minuten-Blick zeigt dir nicht zugelassene Werkzeuge, ungewöhnliches Volumen und Muster, die du in Richtlinien ummünzen kannst. Keine Protokolle heißt keine Untersuchung: Nach einem Vorfall rätst du nur.

**Schritt 7: Halte einen menschlichen Kontrollpunkt bei allem Unumkehrbaren.**
Jede Aktion, die nicht rückgängig gemacht werden kann — Geld senden, Daten löschen, eine Kundenliste mailen, etwas unterschreiben — braucht einen menschlichen Genehmigungsschritt. Keine Benachrichtigung. Eine Genehmigung.

**Schritt 8: Vernachlässige die langweiligen Grundlagen nicht.**
KI ersetzt keine gewöhnliche Sicherheit; sie sitzt obendrauf. Multi-Faktor-Authentifizierung auf jedem Konto, das an Firmendaten reicht, auch Anbieter-Portale. Ein Passwort-Manager, damit niemand Passwörter wiederverwendet. Zeitnahe Updates. Getestete Backups, offline gehalten. Endpoint-Schutz auf jedem Rechner. Wenn diese schwach sind, rettet dich keine KI-spezifische Kontrolle.

**Schritt 9: Schulen mit einer Regel, nicht einem Handbuch.**
Gib dem Personal einen Satz, den es tragen kann: *Was du nicht in eine E-Mail an einen Fremden stecken würdest, steckst du nicht in ein KI-Werkzeug.* Dann sag ihm, was es stattdessen tun soll, und mach diese Alternative einfach. Regeln ohne Alternativen werden ignoriert.

**Schritt 10: Plane den Ausfall des Anbieters ein.**
Frag jeden KI-Anbieter: Was passiert, wenn du eine Woche nicht erreichbar bist? Habe ein manuelles Fallback für jeden Prozess, den du von ihm abhängig gemacht hast. Verfügbarkeit ist eine Sicherheitseigenschaft, und die Gesundheitsgeschichte oben ist der Beweis.

## Ethik und Verantwortung

Sicherheit ist eine ethische Angelegenheit, bevor sie eine technische ist. Wenn Kunden dir ihre Adresse, ihre Gesundheitsdaten oder ihre Zahlungsinformationen geben, vertrauen sie dir, sie sicher aufzubewahren. Sie zu verlieren ist kein Unfall, der dir passiert; es ist ein Schaden, der ihnen zugefügt wird. Das ist dieselbe Fürsorgepflicht, die in [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md) besprochen wird, angewandt auf Systeme statt auf Entscheidungen.

Drei Pflichten folgen. **Pflicht zur Kompetenz:** Ein Werkzeug einzusetzen, das du nicht verstehst, ist nicht neutral. Wenn du nicht sagen kannst, wohin deine Daten gehen, kannst du sie nicht schützen, und „wir wussten es nicht" ist eine schwache Verteidigung vor einem Regulierer, einem Kunden oder einem Gericht. Die Literacy-Pflicht im EU AI Act, behandelt in [Kapitel 5](ch05-rules-and-legal-responsibility.md), macht das explizit. **Pflicht zur Offenlegung:** Wenn du gehackt wirst, sag den betroffenen Menschen es rasch und klar. Es zu verstecken, um deinen Ruf zu schützen, wälzt die Kosten deines Problems auf die Leute ab, die dir vertraut haben; die gesetzlichen Fristen stehen in [Kapitel 10](ch10-privacy-and-gdpr.md). **Verhältnismäßigkeit bei der Überwachung:** Das Protokollieren der KI-Nutzung schützt die Firma, und es bedeutet auch, das zu lesen, was deine Leute tippen. Lege eine schriftliche Richtlinie fest, was protokolliert wird, warum, wer es sehen darf und wie lange. Überwache den Datenfluss, nicht den Menschen. Geheimhaltung zerstört Vertrauen und verstößt oft gegen lokales Recht.

Eine letzte Regel: Benutze keine KI-Werkzeuge, um andere Systeme anzugreifen, und teste deine eigenen Abwehrkräfte nicht an Live-Daten oder Live-Kundenkonten. Nutze eine separate Testumgebung.

## Zu vermeidende Fehler

1. **Ein KI-Werkzeug wie eine Suchmaschine behandeln.** Eine Suchmaschine indexiert öffentliche Seiten. Ein KI-Dienst empfängt deinen Text, speichert ihn und verarbeitet ihn auf fremden Computern.
2. **Breite Berechtigungen erteilen „damit es funktioniert".** Bequemlichkeit heute ist morgen ein Einbruch. Vergib das Minimum und erweitere nur bei nachgewiesenem Bedarf.
3. **Ein KI alles lesen lassen.** Einen Assistenten auf ein Shared-Laufwerk zu richten, das Gehälter, Rechtsakten und Kundenunterlagen enthält, macht aus einem kompromittierten Konto totale Preisgabe.
4. **Kein Protokollieren.** Ohne Aufzeichnungen kannst du nicht herausfinden, was passiert ist, oder beweisen, dass du die Kontrolle hattest.
5. **„Enterprise-Grade" als Antwort akzeptieren.** Frag stattdessen: Trainieren Sie mit meinen Daten, wie lange behalten Sie Prompts, wer sind Ihre Unterauftragsverarbeiter, wo werden Daten gespeichert, sagen Sie mir Bescheid, wenn Sie gehackt werden?
6. **Den kostenlosen Consumer-Plan ignorieren.** Personal auf privaten Konten heißt: Deine Daten gehen irgendwohin ohne Vertrag und ohne Kontrollen.
7. **Alles blockieren.** Ein Verbot ohne zugelassene Alternative stoppt die Nutzung nicht; sie versteckt sie.
8. **Vertraulichkeit mit Integrität verwechseln.** Vergiften und Manipulieren sind keine Lecks. Schützt du nur gegen abfließende Daten, übersiehst du verfälschte Daten.
9. **Einem Anbieter vertrauen, weil er groß ist.** Der größte Zahlungshack im Gesundheitswesen der Geschichte begann mit einem fehlenden zweiten Login-Faktor.
10. **Sicherheit als einmaliges Projekt behandeln.** Bedrohungen, Werkzeuge und Personal ändern sich. Überprüfe die Karte jedes Quartal.

## Praktische Übung

### 6.9 Karte deine Schwachstellenpunkte

Reserviere neunzig Minuten mit einem Kollegen, der die tägliche Arbeit kennt. Tu das nicht allein.

**Teil A — Liste die Daten (20 Minuten).** Schreib jede Kategorie sensibler Information auf, die dein Unternehmen besitzt. Typische Zeilen: Kundennamen und Kontakte, Zahlungs- oder Bankdaten, Personalausweis- oder Steuernummern, Mitarbeiter- und Gehaltsunterlagen, Lebensläufe und Bewerberdaten, Gesundheits- oder Versicherungsinfos, Verträge und Angebote, Quellcode oder Entwürfe, Strategie- und Finanzpläne.

**Teil B — Verfolge jede einzelne (40 Minuten).** Beantworte für jede Zeile fünf Fragen schriftlich:

1. Wo lebt sie? (System, Ordner, Tabelle, Papier)
2. Wer kann sie erreichen? (Rollen, namentliche Personen, Auftragnehmer)
3. Welches KI-Werkzeug berührt sie, falls überhaupt?
4. Verlässt sie unser Gebäude? Wohin geht sie, und unter welchem Vertrag?
5. Können wir es geschehen sehen? (Protokollierung, ja oder nein)

**Teil C — Bewerten und auswählen (30 Minuten).** Markiere jede Zeile:

- **Rot** — sensible Daten, die das Unternehmen ohne Vertrag und ohne Protokollierung verlassen.
- **Gelb** — sensible Daten, die drinnen bleiben, aber weit erreichbar sind, oder unter einem Vertrag rausgehen, den du nicht gelesen hast.
- **Grün** — wenig sensible Daten, oder sensible Daten mit Vertrag, Filter und Protokollen.

Jede rote Zeile ist eine Aktion für diesen Monat. Wähle die Top fünf und schreib je einen Verantwortlichen und eine Frist daneben. Eine typische Fünferliste am Anfang: Multi-Faktor-Authentifizierung auf Anbieterkonten, ein zugelassenes KI-Werkzeug fürs Personal, eine Data-Loss-Regel für Ausweisnummern, der Zugriff auf Shared-Laufwerke reduziert auf die Ordner, die jede Rolle braucht, und eine einseitige Nutzungsregel. Halte die Karte auf einer Seite, und aktualisiere sie jedes Quartal und immer wenn du ein neues KI-Werkzeug hinzufügst.

## Checkliste

### 6.10 Die 10 Mindest-Sicherheitsmaßnahmen

- [ ] **Jedes Konto hat Multi-Faktor-Authentifizierung**, auch Anbieter-Portale, E-Mail, Banking, Cloud-Speicher und Administrator-Logins.
- [ ] **Eine schriftliche Karte existiert** von jedem genutzten KI-Werkzeug, welche Daten in jedes reingehen und wo diese Daten gespeichert werden.
- [ ] **Ein zugelassenes KI-Werkzeug existiert und ist einfacher zu benutzen** als die nicht zugelassenen Alternativen.
- [ ] **Ausgehende Filterung ist eingerichtet** für Ausweis- und Steuernummern, Zahlungsdaten, Gesundheitsdaten, Gehälter, Verträge und Quellcode.
- [ ] **Kein KI-Werkzeug handelt auf Anweisungen, die es in Dokumenten findet, die es liest**; Aktionen brauchen menschliche Bestätigung.
- [ ] **Jeder KI-Agent läuft mit minimalen Rechten**: eigenes Konto, nur-Lesen wo möglich, gedeckelte Ausgaben, keine Administrator-Rechte.
- [ ] **Protokolle für die KI-Nutzung existieren, und jemand liest sie wöchentlich.**
- [ ] **Unumkehrbare Aktionen brauchen einen menschlichen Genehmigungsschritt**, nicht nur eine Benachrichtigung.
- [ ] **Anbieter-Prüfung ist schriftlich erledigt**: Training mit deinen Daten, Aufbewahrungsdauer, Unterauftragsverarbeiter, Speicherort der Daten, Bedingungen für die Benachrichtigung bei einem Hack.
- [ ] **Backups sind getestet und offline gehalten, und ein manuelles Fallback existiert** für jeden Prozess, der von einem KI-Anbieter abhängt.

## Kernaussagen

- KI macht Angriffe billiger und schneller, und sie vervielfacht die Zahl der Türen in dein Unternehmen; beides ändert sich zugleich.
- Das häufigste Leck ist kein Hack — es ist ein hilfreicher Mitarbeiter, der vertrauliche Daten in ein Werkzeug einfügt, das er nie geprüft hat.
- Schütze alle drei Eigenschaften: Vertraulichkeit (abfließende Daten), Integrität (vergiftete Daten) und Verfügbarkeit (ein ausfallender Anbieter).
- Die Kernabwehren sind eine Datenkarte, ein kontrolliertes Gateway, ausgehende Filterung, minimale Rechte für Agenten und Protokolle, die tatsächlich jemand liest.
- Dein Risiko umfasst das Risiko deiner Anbieter, und auch das Risiko deren Anbieter; frag, auf wen sie sich stützen, bevor du dich auf sie stützt.
