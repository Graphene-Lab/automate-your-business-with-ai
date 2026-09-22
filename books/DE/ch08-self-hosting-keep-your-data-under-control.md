# Kapitel 8 — Self-Hosting: Behalte deine Daten unter Kontrolle

## In einfachen Worten

Self-Hosting bedeutet, Software auf Computern laufen zu lassen, die dir gehören oder die du kontrollierst, statt sie von den Computern jemand anderes zu mieten.

Du kennst beide Seiten davon. Ein Hotelzimmer zu mieten ist Cloud: Jemand anderes putzt, repariert und hat einen Ersatzschlüssel. Ein eigenes Haus zu besitzen ist Self-Hosting: Du reparierst den Kessel selbst, aber niemand sonst hat einen Schlüssel.

Auf KI angewendet bedeutet Self-Hosting, dass das Modell — die Software, die das Denken macht — auf einem Rechner in deinem Büro oder auf einem Server läuft, den du kontrollierst. Deine Fragen gehen dort hinein. Die Antworten kommen dort heraus. Nichts wandert über das Internet zu einer Firma, die du nicht gewählt hast.

Für ein kleines Unternehmen war das bis vor Kurzem nicht möglich. Bis 2022 lebten die besten Sprachmodelle nur in riesigen Rechenzentren, und man erreichte sie nur durch eine gemietete Tür namens API — eine Standard-Schnittstelle, die eine Firma öffnet, damit andere Software ihre Systeme befragen kann. Jede Frage, die du tipptest, ging durch diese Tür und landete auf ihren Maschinen.

Dann änderten sich zwei Dinge. Erstens tauchten offene Modelle auf: Modelle, deren trainierte Dateien jeder herunterladen und ausführen kann. Zweitens wurden Kompressionstechniken gut genug, dass ein komprimiertes Modell auf einem gewöhnlichen leistungsstarken Desktop-Computer läuft, mit nur einem kleinen Qualitätsverlust.

Der Kompromiss ist ein Dreieck, und du kannst nicht alle drei Ecken zugleich haben.

- **Kontrolle.** Du entscheidest, was mit deinen Daten geschieht, welches Modell du nutzt, wann es sich ändert, und wer es sehen kann.
- **Leistung.** Wie gut die KI bei schwierigen Aufgaben tatsächlich ist.
- **Kosten.** Was du zahlst, an Geld, Zeit und Aufmerksamkeit.

Cloud-KI gibt hohe Leistung bei geringem Aufwand und geringer Kontrolle. Self-Hosting gibt hohe Kontrolle, mittlere Leistung und Kosten, die du upfront in Hardware zahlst und dann erneut in laufender Zeit. Die richtige Antwort hängt davon ab, was du tust.

Zwei ehrliche Sätze, bevor wir weitergehen. Self-Hosting ist nicht automatisch sicherer — ein schlecht konfigurierter lokaler Server ist schlechter als ein gut betriebener Cloud-Dienst. Und Self-Hosting ist nicht automatisch günstiger — im kleinen Maßstab gewinnt meist das Mieten. Was Self-Hosting kauft, ist eine bestimmte und wertvolle Sache: Deine Daten gehen nicht hinaus, und niemand kann dein System ändern, ohne dass du es weißt.

Verwandte Themen anderswo: [Kapitel 11](ch11-digital-sovereignty.md) behandelt die weitere Idee, deine eigenen digitalen Werkzeuge zu kontrollieren, [Kapitel 9](ch09-third-party-services-and-shadow-ai.md) behandelt das gegenteilige Muster unkontrollierter Drittanbieter-Dienste, und [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md) behandelt die Sicherheitsgrundlagen, die auch für einen Rechner in deinem eigenen Büro gelten.

## Ein bisschen Geschichte

**1990er bis 2000er: alles zu Hause.** Ein kleines Unternehmen hatte einen Server im Schrank. E-Mail, Dateien und Konten lagen alle im Haus. Du besitzt die Maschine und alle ihre Probleme.

**2000er bis 2018: der Auszug.** Breitband wurde schnell, und Mieten wurde einfacher als Besitzen. E-Mail ging zuerst, dann Dateien, dann Buchhaltung und Kundenakten. „Die Cloud" wurde die Standardantwort. Der Witz unter Ingenieuren war zutreffend: Es gibt keine Cloud, es ist nur jemand anderes Computer.

**2013: Container.** Docker kam und verpackte Software so, dass sie überall gleich lief. Das machte Self-Hosting leise wieder einfach, weil man keinen Spezialisten mehr brauchte, um eine Anwendung auf jeder neuen Maschine neu aufzubauen.

**2022: KI war nur eine Miete.** Die besten Sprachmodelle existierten nur in einer Handvoll großer Firmen. Wenn du KI wolltest, schicktest du ihnen deinen Text. Es gab keine nutzbare Alternative.

**2023: das Jahr der offenen Modelle.** Meta veröffentlichte Llama im Februar als Forschungsmodell, dann Llama 2 mit offenen Gewichten im Juli. Mistral AI veröffentlichte im August ein starkes Sieben-Milliarden-Parameter-Modell. „Offene Gewichte" bedeutet, die trainierten Dateien sind veröffentlicht, sodass jeder sie herunterladen und ausführen kann. Im selben Jahr wurde Quantisierung — ein Modell so komprimieren, dass es viel weniger Speicher braucht — gut genug für den täglichen Gebrauch. Plötzlich war eine fähige KI nicht nur in einem Rechenzentrum.

**8. Juli 2023: Ollama.** Ein Werkzeug namens Ollama wurde veröffentlicht, quelloffen unter der MIT-Lizenz, hauptsächlich in Go mit etwas C und TypeScript geschrieben, von Jeffrey Morgan und Michael Chiang. Seine Aufgabe war es, alle Reibung zu entfernen. Ein Befehl lädt ein Modell herunter und führt es lokal aus, mit einer einfachen Oberfläche und einem lokalen Dienst, mit dem andere Programme sprechen können. Es nutzte die llama.cpp-Engine für die eigentliche Arbeit auf deiner Hardware.

**2024: „souverän" wird ein Kaufkriterium.** Firmen in regulierten Branchen und mehrere europäische Regierungen begannen, KI zu verlangen, die im Land und innerhalb der eigenen Mauern bleibt. Cloud-Anbieter antworteten mit Sovereign-Cloud-Optionen, und ein Markt für On-Premise-KI wuchs schnell.

**2026: ein Open-Source-Enterprise-Client.** Im April 2026 kündigte MZLA Technologies, eine Mozilla-Tochter, Thunderbolt an, einen quelloffenen KI-Client, der für Self-Hosting gebaut ist. Der Neugier-Abschnitt behandelt ihn.

Die Form dieser Geschichte ist eine Schleife. Wir begannen mit Self-Hosting, zogen aus aus Bequemlichkeit, und ziehen jetzt zurück für Kontrolle — mit viel besseren Werkzeugen als beim ersten Mal.

## Neugier

### 8.7 Mozillas quelloffener KI-Client für „KI, die du kontrollierst"

Im April 2026 kündigte die MZLA Technologies Corporation — eine hundertprozentige Tochter von Mozilla, der gemeinnützigen Organisation hinter Firefox — **Thunderbolt** an. Es ist ein quelloffener, plattformübergreifender KI-Client, gebaut für Organisationen, die KI nach ihren eigenen Bedingungen betreiben wollen.

Die Details, die für dieses Kapitel zählen:

- **Self-Host-fähig.** Er läuft auf der eigenen Infrastruktur des Kunden. Das Projekt beschreibt Unterstützung für On-Premise-, Sovereign-Cloud- und Air-Gapped-Setups — also ein Netzwerk, das physisch vom Internet getrennt ist.
- **Modell-agnostisch.** Er funktioniert mit jedem Agenten, der das Agent Client Protocol spricht, und mit jedem Modell, das eine OpenAI-kompatible API bietet. In der Praxis bedeutet das, dass du ihn auf ein lokales Modell, deinen eigenen Server oder einen kommerziellen Anbieter richten und wechseln kannst, ohne deine Werkzeuge zu ändern.
- **Überall.** Web, Windows, macOS, Linux, iOS und Android.
- **Mit deinen Systemen verbunden.** Er integriert sich über das Model Context Protocol in Unternehmenssysteme — eine Standardmethode, damit ein KI-Werkzeug deine internen Daten und Aktionen erreicht — und unterstützt wiederverwendbare Automatisierungen und eine erweiterbare API.
- **Auditierbar.** Weil der Code offen ist, kannst du ihn oder ein Dritter lesen und prüfen, was er tatsächlich tut. Das Projekt hat gesagt, es durchlaufe ein Sicherheits-Audit.
- **Ein Partner für europäische Souveränität.** Er kombiniert sich mit deepsets Haystack, einer quelloffenen Orchestrierungsplattform, für souveräne Bereitstellungen in Europa.
- **Support inklusive.** Enterprise-Support und vorausbegleitendes Engineering werden angeboten, was der Teil ist, den die meisten Open-Source-Projekte dir allein zu lösen überlassen.

Das Positionieren ist bemerkenswert. Der Rahmen ist „KI, die du kontrollierst", und das Argument ist, dass KI zu wichtig ist, um sie ganz auszulagern. Das ist dasselbe Argument, das ein kleiner Unternehmer macht, wenn er beschließt, Gehaltsakten auf dem eigenen Rechner zu behalten statt in einem Dienst, den er nie geprüft hat.

Ein kleineres, älteres Beispiel derselben Idee steckt in einer E-Mail-App, die viele Menschen schon nutzen. Das ThunderAI-Add-on für Thunderbird fügte in Version 2.1.1, veröffentlicht im August 2024, Unterstützung für lokale Modelle über Ollama hinzu. Mit diesem Setup läuft das Modell auf deinem eigenen Computer, der E-Mail-Text verlässt also nie die Maschine, und es wird kein Cloud-Konto oder API-Schlüssel benötigt. Es ist eine kleine Funktion, und sie macht den Punkt klar: Lokale KI ist kein Forschungsprojekt mehr. Sie ist eine Option in einem kostenlosen E-Mail-Client.

## Ein echtes Geschäftsbeispiel

### Sogar Apple baute seine eigene Cloud

Apple ist eine Firma, die fast alles mieten könnte. Im Juni 2024 kündigte sie ein System namens Private Cloud Compute an, gebaut für die KI-Funktionen ihrer Geräte, wenn eine Aufgabe zu groß für das Telefon selbst ist. Was sie sich entschied, mit diesem System zu tun, ist die Lektion.

Apple baute seine eigenen Server um seine eigenen Chips mit einem gehärteten Betriebssystem. Es entwarf das System für zustandslose Inferenz — die Anfrage verarbeiten, die Antwort zurückgeben, nichts behalten. Und es gab ein ungewöhnliches Versprechen ab: Es würde das Software-Image jedes Produktions-Builds veröffentlichen, damit externe Sicherheitsforscher genau prüfen können, was läuft, und kontrollieren, dass die Maschine, mit der sie sprechen, wirklich das ist, was sie zu sein vorgibt. Im Oktober 2024 veröffentlichte Apple einen Sicherheitsleitfaden und lud Forscher ein, das System anzugreifen.

Daraus folgen drei Dinge für ein kleines Unternehmen.

Erstens, beachte die Begründung. Apple baute keine Cloud, weil es keine mieten konnte. Es baute eine, weil Mieten bedeutet hätte, Nutzerdaten nach den Bedingungen jemand anderes zu halten, und seine ganze Marke darin besteht, dass es das nicht tut. Kontrolle über die Maschine war ihnen echtes Geld wert.

Zweitens, beachte die Verifikationsidee. Die Software zu veröffentlichen, damit Außenstehende sie prüfen können, ist derselbe Instinkt wie Open-Source-Auditing. Vertrauen wird verringert, indem man das System überprüfbar macht, nicht indem man verspricht, gut zu sein.

Drittens, beachte die Größe der Lücke. Apple gab ein Vermögen aus, um „wir behalten nichts" zu erreichen. Die meisten kleinen Unternehmen können das nicht kopieren. Aber du kannst die Frage kopieren: *Wer betreibt die Maschine, wohin meine Daten gehen, was behalten sie, und kann jemand das prüfen?* Wenn du diese drei Fragen über ein Werkzeug nicht beantworten kannst, solltest du keine sensiblen Daten hineingeben. Und wenn die ehrliche Antwort „wir können nicht prüfen" ist, wird ein Modell auf deinem eigenen Rechner eine ernsthafte Option.

## Wie man es macht

### 8.5 Wie man anfängt: von Open-Source-Werkzeugen wie Ollama zu lokalen Modellen

**Schritt 1: Wähle eine Aufgabe und eine Person.**
Kaufe nicht zuerst Hardware. Wähle eine wiederholte Aufgabe mit sensiblen Daten — Verträge zusammenfassen, Antworten auf Standardanfragen entwerfen, Meeting-Notizen in Aufgabenlisten verwandeln. Gib sie einer neugierigen Person mit einem guten Computer.

**Schritt 2: Installiere Ollama.**
Ollama läuft auf Windows, macOS und Linux. Nach der Installation zieht ein Befehl ein Modell und startet einen Chat in deinem Terminal. Unter der Haube startet er einen kleinen Dienst auf deinem eigenen Rechner, auf Port 11434, mit dem andere Programme sprechen können. Dieser lokale Dienst ist das, was dir später erlaubt, das Modell mit deinen eigenen Werkzeugen zu verbinden.

**Schritt 3: Wähle das Modell nach Größe, nicht nach Name.**
Modellgrößen werden in Parametern gezählt, einem groben Maß dafür, wie groß und leistungsfähig das Modell ist. Als Faustregel:

- **1 bis 3 Milliarden** — schnell und leicht, läuft auf einem gewöhnlichen Laptop. Gut für kurze Zusammenfassungen und einfache Entwürfe.
- **7 bis 9 Milliarden** — die praktische Mitte. Gute allgemeine Qualität, braucht einen anständigen Rechner mit genug Speicher.
- **70 Milliarden und darüber** — viel stärker, aber braucht ernsthafte Hardware und viel Speicher. Normalerweise kein Startpunkt für ein kleines Unternehmen.

Suche nach **quantisierten** Versionen. Quantisierung komprimiert die Zahlen im Modell, sodass es viel weniger Speicher braucht und schneller läuft, um den Preis eines kleinen Qualitätsabfalls. Für die meisten Büroaufgaben ist dieser Abfall akzeptabel.

**Schritt 4: Füge eine freundliche Oberfläche hinzu.**
Das Terminal ist zum Testen in Ordnung. Für den täglichen Gebrauch füge eine lokal laufende Chat-Oberfläche hinzu, oder stöpsle das Modell in eine App, die Leute schon nutzen — das oben erwähnte Thunderbird-Add-on ist ein Beispiel. Das Ziel ist, dass ein nicht-technischer Kollege es ohne Hilfe nutzen kann. Wenn nur eine Person es steuern kann, wird es nie angenommen.

**Schritt 5: Halte es tatsächlich lokal.**
Hier scheitern die Leute. Der lokale Dienst darf nur auf deinem eigenen Rechner lauschen, nicht im ganzen Netzwerk. Sicherheitsforscher haben viele Ollama-Server gefunden, die dem öffentlichen Internet ausgesetzt waren, weil sie so eingestellt waren, Verbindungen von jeder Adresse anzunehmen. Also: Behalte die lokale Standard-Bindung, setze eine Firewall davor, öffne niemals Port 11434 für das Internet, und führe ihn nicht mit Administratorrechten aus. Ein lokales Werkzeug ist nicht automatisch ein sicheres Werkzeug.

**Schritt 6: Lass ihn deine eigenen Dateien lesen.**
Der nützlichste nächste Schritt ist Abruf, oft RAG genannt. In klaren Worten: Statt das Modell neu zu trainieren, steckst du deine Dokumente in einen durchsuchbaren Index. Wenn jemand eine Frage stellt, findet das System die relevanten Stellen und gibt sie dem Modell zusammen mit der Frage. Das Modell antwortet aus deinen Dokumenten. Es wird nichts auf deinen Daten trainiert, und das Ganze kann auf deinem eigenen Rechner laufen. So bekommst du „frag unser Handbuch", ohne das Handbuch irgendwohin zu schicken.

**Schritt 7: Skaliere erst, wenn der Test funktionierte.**
Wenn der Pilot nützlich ist, dann kauf Hardware. Eine Workstation mit einer starken Grafikkarte ist die übliche Antwort, weil Grafikspeicher das begrenzt, wie groß ein Modell sein kann, das du ausführen kannst. Apple-Maschinen mit vereinheitlichtem Speicher sind aus demselben Grund eine häufige Wahl. Ein kleiner Server ergibt Sinn, wenn mehrere ihn gleichzeitig brauchen.

**Schritt 8: Entscheide die Aufteilung.**
Die meisten Firmen landen hybrid. Sensible Daten und routinemäßige Massen Aufgaben laufen lokal. Schwieriges Schlussfolgern, sehr lange Dokumente und Spezialfunktionen nutzen einen Cloud-Dienst unter einem richtigen Vertrag. Schreibe die Regel auf: Welche Daten wohin gehen, und wer entscheidet.

### 8.6 Ideale Anwendungsfälle

**Sensible personenbezogene Daten.** Gesundheitsakten, Personalakten, Gehaltsabrechnungen, Bewerber-Lebensläufe, finanzielle Kundendetails. Wenn die Daten nicht hinaus dürfen, entfernt lokale Verarbeitung die Frage ganz.

**Proprietäre Informationen.** Designs, Zeichnungen, Quellcode, Ausschreibungs- und Angebotsdokumente, Preismodelle, Strategiepläne. Das sind die Dateien, die am meisten wehtun, wenn ein Anbieter sie behält oder leckt.

**Regulierte Branchen.** Gesundheitswesen, Kanzleien, Banken und Versicherungen, Regierung und Verteidigung, und jedes Unternehmen unter Datenresidenz-Regeln, die verlangen, dass Daten im Land oder in der Region bleiben. Self-Hosting macht eine schwierige Compliance-Unterhaltung zu einer einfachen.

**Schlechte oder keine Konnektivität.** Baustellen, Fabriken, Schiffe, Bergwerke, Außenstellen, Notfallhilfe. Ein lokales Modell funktioniert, wenn das Internet es nicht tut.

**Massenhafte sich wiederholende Arbeit.** Tausende Tickets, Rechnungen oder Dokumente. Ein Preis pro Anfrage tut bei Menge weh; eine feste Maschine wächst nicht.

**Günstiges Experimentieren.** Ideen ausprobieren, ohne dass ein Zähler läuft. Nützlich, bevor du Budget bindest.

**Wo es schlecht passt:** Schlussfolgern auf Spitzen-Niveau, sehr lange Dokumente, fortgeschrittene Bildgenerierung, und jedes Team ohne jeglichen technischen Support. Wenn niemand es warten kann, fang nicht an.

## Ethik und Verantwortung

Self-Hosting löst ein ethisches Problem und schafft andere. Sei klar, welches was ist.

**Was es löst.** Deine Kundendaten reisen nicht mehr zu Firmen, die du nicht gewählt hast, und können nicht ohne dich genutzt werden, um das Produkt jemand anderes zu trainieren. Das ist ein echter Gewinn an Respekt gegenüber den Menschen, deren Daten du hältst.

**Was es nicht löst.** Das Modell kann weiterhin falsch, voreingenommen oder zuversichtlich irreführend sein. Ein voreingenommenes Modell auf deiner eigenen Hardware laufen zu lassen, macht es nicht fair. Die Pflichten in [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md) gelten weiterhin, und ebenso die Offenlegungsregeln in [Kapitel 5](ch05-rules-and-legal-responsibility.md).

**Was es hinzufügt.** Du bist jetzt der Betreiber. Patchen, Zugriffskontrolle, Protokollierung und Backups sind deine Aufgabe. Wenn ein ungepatchter lokaler Server Daten leckt, liegt das auf eine neue und sehr direkte Weise bei dir.

**Mitarbeiterüberwachung.** Wenn du Anfragen an ein lokales System protokollierst, hältst du jetzt eine detaillierte Aufzeichnung davon, was deine Mitarbeiter fragten. Habe eine schriftliche Richtlinie, was behalten wird, warum, wer es liest, und wie lange. Halte es verhältnismäßig, und sag es den Leuten.

**Verkaufe Souveränität nicht zu gut.** „Souverän" ist ebenso ein Marketing-Wort wie ein technisches. Wenn du Kontrolle behauptest, aber nicht patchen, sichern oder auditieren kannst, ist die Behauptung leer. Sag, was du tatsächlich hast, und sag klar, was du nicht hast.

**Energie.** Eine Maschine, die den ganzen Tag Modelle laufen lässt, verbraucht Strom. Lokal ist nicht automatisch umweltfreundlicher als ein großes, effizientes Rechenzentrum. Wenn du einen Umweltvorteil behauptest, prüfe ihn zuerst.

## Zu vermeidende Fehler

1. **Hardware vor dem Testen einer Aufgabe kaufen.** Teste zuerst mit einem gemieteten oder geliehenen Setup. Auf Hoffnung gekaufte Hardware bleibt ungenutzt.
2. **Den lokalen KI-Dienst dem Internet aussetzen.** Das ist der häufigste und schwerwiegendste Self-Hosting-Fehler. Halte ihn lokal, Firewall ihn, öffne nicht den Port.
3. **Annehmen, lokal gleich sicher.** Du besitzt jetzt die Sicherheit dieser Maschine, einschließlich der Teile, an die du nie gedacht hast.
4. **Keine Backups.** Die Maschine, die Modelle, die Konfiguration und der Dokumenten-Index müssen alle gesichert werden.
5. **Das größte Modell wählen.** Größer ist langsamer, hungriger und oft nicht besser für deine tatsächliche Aufgabe.
6. **Modell-Lizenzen ignorieren.** Modelle mit offenen Gewichten kommen mit unterschiedlichen Bedingungen, einschließlich Regeln zur kommerziellen Nutzung und dazu, wie du deine Nutzung beschreiben darfst. Lies die Lizenz, bevor du darauf aufbaust.
7. **Ein-Personen-Abhängigkeit.** Wenn eine Person weiß, wie es funktioniert, und geht, stoppt das System. Schreibe das Setup, den Neustart und die Wiederherstellungsschritte auf.
8. **Die falsche Arbeitslast self-hosten.** Wenn die Aufgabe Spitzenqualität braucht, wird lokal enttäuschen, und du wirst fälschlich schließen, die Technologie sei nutzlos.
9. **Nie aktualisieren, oder aktualisieren ohne Testen.** Eine neue Modellversion ändert Antworten. Führe deine Beispielaufgaben nach jeder Änderung erneut aus.
10. **Es als Alles-oder-Nichts behandeln.** Ein Hybrid-Setup ist normalerweise die richtige Antwort, nicht ein totaler Umzug in eine Richtung.

## Praktische Übung

### 8.8 Auswerten, ob Self-Hosting zu deiner Firma passt

Bewerte jede Zeile mit 0, 1 oder 2. Sei ehrlich.

| Frage | 0 | 1 | 2 |
|---|---|---|---|
| Wie sensibel sind die Daten? | Öffentlich | Intern | Kundenvertraulich oder reguliert |
| Technischer Support verfügbar | Keiner | Teilweise IT-Hilfe | Jemand, der einen Server warten kann |
| Hardware-Budget | Keins | Eine gute Workstation | Workstation plus ein kleiner Server |
| Aufgabenkomplexität | Zusammenfassungen und Entwürfe | Fragen über Dokumente | Komplexes Schlussfolgern, sehr lange Dokumente |
| Konnektivität | Unzuverlässig | In Ordnung | In Ordnung |
| Menge | Gelegentlich | Täglich | Hoch und wachsend |

Lies die Bewertung Zeile für Zeile, denn die Zeilen schieben nicht alle in dieselbe Richtung.

- **Sensibilität 2** und **Menge 2** schieben beide Richtung Self-Hosting.
- **Technischer Support 0** schiebt stark dagegen, was auch immer die anderen Bewertungen sagen.
- **Aufgabenkomplexität 2** schiebt dagegen, weil lokale Modelle beim schwierigen Schlussfolgern hinterherhinken.

Jetzt mache einen eintägigen Test, bevor du irgendetwas ausgibst. Nimm zwanzig echte Aufgaben von deiner Liste. Mache zehn mit einem mittelgroßen lokalen Modell und zehn mit einem Cloud-Dienst. Vergleiche drei Dinge: War die Antwort gut genug, um sie so zu nutzen, wie sie war, wie lange dauerte es, und was hätte es andersherum gekostet. Schreibe die Ergebnisse auf.

Wenn die lokale Antwort für die meisten Aufgaben nutzbar war, ist Self-Hosting die Investition wert. Wenn sie nur für wenige nutzbar war, halte diese lokal und lass den Rest in der Cloud unter einem Vertrag. So oder so hast du jetzt Beweise statt einer Meinung.

## Checkliste

### 8.9 Was du zum Starten brauchst

- [ ] **Eine benannte Aufgabe**, die sensible Daten betrifft und oft wiederkehrt.
- [ ] **Eine benannte Person**, die das System installieren, neu starten, sichern und aktualisieren kann — oder einen Plan, eine einzustellen.
- [ ] **Ein Rechner mit genug Speicher**, gewählt nach einem Test, nicht vorher.
- [ ] **Ein Modell gewählt nach Größe und Quantisierung**, abgestimmt auf die Aufgabe statt auf das größte verfügbare.
- [ ] **Eine lokale Oberfläche**, die ein nicht-technischer Kollege ohne Hilfe nutzen kann.
- [ ] **Der Dienst nur an die lokale Maschine gebunden**, firewalled, ohne offenen Port zum Internet.
- [ ] **Eine schriftliche Lizenzprüfung** für das gewählte Modell, einschließlich Bedingungen zur kommerziellen Nutzung.
- [ ] **Ein Backup-Plan** für die Maschine, die Modelle, die Konfiguration und den Dokumenten-Index.
- [ ] **Eine Patch-Routine** mit festem Datum, und ein erneuter Test der Beispielaufgaben nach jeder Änderung.
- [ ] **Eine schriftliche Aufteilungsregel**, die festlegt, welche Daten lokal bleiben und welche einen Cloud-Dienst nutzen dürfen, und wer entscheidet.

## Das Wichtigste

- Self-Hosting bedeutet, die KI läuft auf Maschinen, die du kontrollierst, sodass deine Daten sie nicht verlassen.
- Es wurde für kleine Unternehmen praktisch, als 2023 Modelle mit offenen Gewichten und gute Kompression kamen, und Werkzeuge wie Ollama die Einrichtungs-Reibung entfernten.
- Du tauschst Leistung und Bequemlichkeit gegen Kontrolle: Das Dreieck ist Kontrolle, Leistung und Kosten, und du kannst nicht alle drei haben.
- Lokal ist nicht automatisch sicher oder günstig; ein falsch konfigurierter lokaler Server ist ein echtes Risiko, und Wartung ist jetzt deine Aufgabe.
- Fange mit einer Aufgabe, einer Person und einem eintägigen Test an, bevor du Hardware kaufst.
