# Kapitel 7 — Trustless: Vertrauen ohne zu vertrauen

## In einfachen Worten

Das Wort „trustless" ist schlecht gewählt. Es klingt nach einer Welt ohne Vertrauen, in der niemand irgendetwas glaubt. Das bedeutet es nicht, und die echte Idee ist viel nützlicher.

Trustless bedeutet: **Du musst weder einer Person noch einer Institution vertrauen, weil du die Tatsache selbst überprüfen kannst.**

Beginne mit einem vertrauten Gegensatz. Du beauftragst eine Umzugsfirma. Du übergibst eine Anzahlung. Jetzt bist du davon abhängig, dass sie auftaucht. Du musst ihnen vertrauen, oder ihrer Marke, oder dem Gesetz, das sie bestraft, wenn sie es nicht tun. Denk jetzt an einen Automaten. Du wirfst Münzen ein, das Getränk fällt heraus. Da ist keine Beziehung, kein Versprechen, und kein Bedarf, irgendwem zu glauben. Der Automat erzwingt das Geschäft durch seine Bauart. Das ist das Gefühl von trustless: Die Vereinbarung wird durch ein System erzwungen statt durch die guten Absichten einer Person.

Drei Werkzeuge machen das möglich.

**Überprüfung statt Versprechen.** Statt dass dir jemand sagt, eine Sache sei wahr, prüfst du sie. Eine digitale Signatur ist das gängige Beispiel. Sie beweist, dass eine Datei von dem stammt, der einen bestimmten Schlüssel besitzt, und dass die Datei sich seit der Signierung nicht geändert hat. Du musst dem Absender nicht vertrauen. Du prüfst die Signatur.

**Transparenz statt Geheimhaltung.** Statt eine Aufzeichnung in einem privaten Notizbuch zu führen, führst du sie irgendwo, wo viele Leute sie lesen und niemand sie still umschreiben kann. Wenn jeder die Aufzeichnung sehen kann, kann keine Partei die Geschichte zu ihrem Vorteil ändern.

**Automatische Durchsetzung statt Hoffnung.** Statt Bedingungen zu vereinbaren und zu hoffen, dass sie eingehalten werden, schreibst du die Bedingungen so, dass ein Stück Software sie ausführt. Geld wird freigegeben, wenn die Bedingung erfüllt ist. Niemand muss einer Rechnung hinterherjagen.

Nun die ehrliche Warnung, früh gesagt: trustless bedeutet nicht risikofrei. Du hast dein Vertrauen von Menschen auf Systeme verlagert, und Systeme werden von Menschen gebaut. Code hat Fehler. Die Zuführungen, die einem System sagen, was in der echten Welt passiert ist, können falsch sein oder angelogen werden. Schlüssel gehen verloren, und ein verlorener Schlüssel kann verlorenes Geld bedeuten. Das Ziel ist nicht, Vertrauen zu entfernen. Es ist, Vertrauen irgendwohin zu legen, das du prüfen kannst, und zu verringern, wie viel davon du brauchst.

Warum sich das überhaupt antun? Weil Vertrauen teuer ist. Jeder Vermittler, auf den du dich verlässt — eine Bank, ein Treuhänder, ein Makler, ein Notar, eine Plattform, die Geld bis zur Erledigung behält — nimmt einen Anteil und braucht Zeit. Trustless-Systeme entfernen etwas davon und machen das Übriggebliebene billiger, schneller und sichtbar. Das ist nicht nur für Banken und Programmierer; es hat direkten Nutzen in jeder Firma, die bei Lieferanten kauft, Freiberufler einstellt und Aufzeichnungen braucht, denen ihr Buchhalter vertrauen kann.

Die weitere Frage, wer deine digitalen Werkzeuge kontrolliert, steht in [Kapitel 11](ch11-digital-sovereignty.md). Ob es sich auszahlt, ist eine Frage aus [Kapitel 16](ch16-goals-costs-and-return-on-investment.md). Die Sicherheitsseite der Überprüfung ist in [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md).

## Ein bisschen Geschichte

**2008.** Im Oktober wurde ein Papier mit dem Titel „Bitcoin: A Peer-to-Peer Electronic Cash System" unter dem Namen Satoshi Nakamoto veröffentlicht. Sein erklärtes Ziel war elektronische Zahlung ohne vertrauenswürdige Dritte. Der Trick war ein gemeinsamer, geordneter Datensatz — eine Blockchain — zusammengehalten von vielen unabhängigen Computern, sodass keiner von ihnen allein ihn umschreiben kann.

**2009.** Das Bitcoin-Netzwerk begann im Januar zu laufen. Zum ersten Mal konnten zwei Fremde Wert miteinander begleichen, ohne eine Bank in der Mitte, und keiner musste dem anderen vertrauen.

**2015.** Ethereum kam und fügte das wichtigste Upgrade hinzu: Smart Contracts. Ein Smart Contract ist ein Programm, das im Netzwerk gespeichert ist und genau wie geschrieben abläuft, wenn seine Bedingungen erfüllt sind. Geld konnte nun an eine Regel gebunden werden.

**2016.** Ein Projekt namens The DAO hielt Geld in einem Smart Contract und wurde wegen eines Fehlers in diesem Contract geleert. Die Nachwirkungen spalteten die Gemeinschaft. Die Lektion war scharf und gilt noch: Automatische Durchsetzung erzwingt Fehler mit derselben Loyalität, mit der sie Funktionen erzwingt.

**2017 bis 2021.** Dezentrale Finanzen wuchsen zu einem echten Sektor: Ausleihen, Handel und Abwicklung durch Verträge statt Banken, mit Stablecoins — Token, die einen stabilen Wert halten sollen — als ihrem Arbeitsgeld. Er zeigte auch dieselben Ausfälle in größerem Maßstab: schlechter Code, falsche Preiszuführungen, unehrliche Betreiber. Im Jahr **2019** veröffentlichte die W3C, das Gremium, das Web-Standards setzt, Verifiable Credentials: eine Möglichkeit für eine Autorität, eine digitale Behauptung — einen Abschluss, eine Lizenz, einen Altersnachweis — auszustellen, die jeder prüfen kann, ohne den Aussteller anzurufen. Das ist die Identitäts-Hälfte des Bildes.

**2021 bis 2023.** Ein Standard namens ERC-4337, bekannt als Account Abstraction, wurde 2021 vorgeschlagen und später finalisiert. Er erlaubt, dass ein Konto ein kleines Programm statt eines einzelnen privaten Schlüssels ist, sodass das Konto seine eigenen Regeln halten kann: Ausgabengrenzen, eine Liste erlaubter Zahlungsempfänger, eine zweite Unterschrift für große Beträge und Wiederherstellung, wenn ein Schlüssel verloren geht.

**Mai 2025.** Ein Ethereum-Upgrade namens Pectra ging im Hauptnetz live. Es ließ eine gewöhnliche Wallet-Adresse auf Smart-Contract-Code zeigen und brachte Transaktions-Bündelung, gesponserte Gebühren und bessere Wiederherstellung zu Adressen, die zuvor keine hatten. Es hob auch den maximalen Einsatz an, den ein einzelner Validator halten kann.

**August 2025.** Ein Standard-Entwurf namens ERC-8004 erschien, betitelt „Trustless Agents". Er wurde für das Problem geschrieben, worum es in diesem Kapitel wirklich geht: Software-Agenten, die mit den Agenten anderer Leute handeln.

Lies die Zeitleiste als eine lange Argumentation. Jeder Schritt verlagerte die Durchsetzung aus den Händen einer Person in ein überprüfbares System: zuerst Geld, dann Vereinbarungen, dann Identität, dann Berechtigungen, und zuletzt Agenten.

## Neugier

### 7.6 Ethereum baut die Rohrleitungen für eine Agenten-Wirtschaft

Im August 2025 wurde ein Standard-Entwurf namens **ERC-8004** auf Ethereums offizieller Standard-Seite veröffentlicht. Sein Titel ist „Trustless Agents", und sein erklärter Zweck ist, Software-Agenten zu erlauben, über Organisationsgrenzen hinweg andere Agenten zu entdecken, auszuwählen und mit ihnen zu arbeiten, ohne jedes vorherige Vertrauen.

Er definiert drei Register, alle on-chain.

**Identität.** Jeder Agent erhält eine On-Chain-Kennung, aufgebaut auf dem gängigen ERC-721-Token-Standard, die auf eine Registrierungsdatei zeigt. Diese Datei enthält die Metadaten des Agenten, die Adressen, mit denen man sprechen kann, und welche Vertrauensmodelle er unterstützt. In klaren Worten: Ein Agent kann sagen, wer er ist, für wen er handelt, und wie du ihn prüfen kannst, und du kannst das nachschlagen, statt ihn beim Wort zu nehmen.

**Reputation.** Eine Standard-Art, Feedback über einen Agenten zu veröffentlichen und zu lesen, sodass die Leistungs-Historie nicht in der privaten Sterne-Bewertung einer einzigen Plattform eingeschlossen ist. Jeder kann Signale beisteuern, und die Zusammenführung kann off-chain geschehen. Der Punkt ist Portabilität: Die Akte eines Agenten folgt ihm, statt jedes Mal zurückgesetzt zu werden, wenn er den Marktplatz wechselt.

**Validierung.** Andockpunkte, um unabhängige Prüfung der Arbeit eines Agenten zu bekommen. Der Standard listet mehrere Methoden: eine andere Partei die Aufgabe mit Geld auf dem Spiel neu ausführen lassen, Zero-Knowledge-Machine-Learning-Beweise nutzen — eine Art zu beweisen, dass eine Berechnung korrekt durchgeführt wurde, ohne die Daten oder das Modell dahinter preiszugeben — vertrauenswürdige Hardware-Enklaven nutzen, oder einen vertrauenswürdigen menschlichen Richter nutzen.

Warum sollte ein kleiner Unternehmensinhaber sich für einen Standard-Entwurf interessieren? Er zeigt, wo die Industrie das harte Problem sieht: nicht „kann ein Agent die Aufgabe ausführen", sondern „wie weiß ich, ob ich diesem Agenten glauben soll" — eine Geschäftsfrage, keine technische. Wenn er Erfolg hat, wirst du eine öffentliche Aufzeichnung prüfen können, statt ein Verkaufsdeck zu vertrauen, was verändert, wer die Macht im Gespräch hat. Und dieselben drei Fragen sind heute eine nützliche Checkliste, ganz ohne Blockchain: *Wer bist du, und für wen handelst du? Wie hast du dich früher verhalten? Kann deine Arbeit unabhängig geprüft werden?*

Zwei andere Stücke derselben Rohrleitung sind bereits live. Account Abstraction, der ERC-4337-Standard, bedeutet, dass ein Agent ein Budget mit Regeln halten kann, die durch Code erzwungen werden: eine harte Ausgabengrenze, eine Whitelist erlaubter Zahlungsempfänger, eine zweite menschliche Unterschrift über einer Schwelle. Und seit dem Pectra-Upgrade im Mai 2025 kann eine gewöhnliche Adresse auf solchen Code zeigen. Diese Kombination — ein Agent, der zahlen kann, in einer Box, die er nicht verlassen kann — ist die praktische Form einer trustless Agenten-Wirtschaft.

Behandle all das als Richtung, nicht als ein Produkt, das du dieses Quartal kaufst. ERC-8004 ist ein Entwurf. Die Konzepte aber sind jetzt nutzbar.

## Ein echtes Geschäftsbeispiel

### Die Mango, die sieben Tage zum Verfolgen brauchte, dann zwei Sekunden

2017 führten Walmart und IBM einen Pilotversuch in Lebensmittel-Lieferketten durch, und die Zahlen, die sie veröffentlichten, wurden in der Branche berühmt. Die Herkunft einer Mango zu verfolgen, die in Mittel- oder Südamerika bezogen wurde, brauchte früher etwa sieben Tage voller Anrufe, E-Mails und Papier-Hinterherjagen. Mit den Aufzeichnungen in einem gemeinsamen Hauptbuch dauerte dieselbe Verfolgung etwa 2,2 Sekunden. IBM beschrieb es als vollständige Ende-zu-Ende-Rückverfolgbarkeit. Ein paralleler Pilot verfolgte Schweinefleisch in China.

Zwei ehrliche Notizen. Die Zahl stammte aus einem kontrollierten Pilotversuch, nicht aus einem vollen Live-Rollout, und die 2,2 Sekunden sind die Zeit, um die Aufzeichnung abzufragen, nicht die Zeit, um eine kontaminierte Sendung zu beheben.

Sieh nun, was sich änderte. Zuvor führte jede Partei ihr eigenes Notizbuch: Der Hof schrieb das Erntedatum, der Abpacker die Charge, der Spediteur den Container, der Laden die Anlieferung. Um eine Frage zu beantworten, musstest du vier Firmen bitten, ihre privaten Notizbücher zu durchsuchen und hoffen, dass sie schnell und ehrlich antworteten. Danach schrieb jeder beim Weitergehen in dieselbe Aufzeichnung. Niemand konnte still seine Seite umschreiben, und „woher kommt das" wurde ein Nachschlagen statt einer Verhandlung.

Das ist der trustless-Wert in einem Satz: **Du hast eine Kette von Versprechen durch eine gemeinsame Aufzeichnung ersetzt, die du lesen kannst.**

Es zeigt auch die Grenze, die wichtiger ist als der Gewinn. Eine gemeinsame Aufzeichnung beweist, was aufgeschrieben wurde. Sie beweist nicht, dass das Aufgeschriebene wahr war. Wenn ein Lieferant einen falschen Hof oder ein falsches Datum eingibt, bewahrt das Hauptbuch die Lüge perfekt auf. Das schwächste Glied ist der Moment, in dem ein Mensch oder ein Sensor eine Tatsache ins System steckt. Jedes trustless-Projekt, das diesen Moment ignoriert, ist Dekoration.

## Wie man es macht

### 7.3 Wie es in der Praxis funktioniert: überprüfbare Identität, Reputation, programmierbare Zahlungen

Du brauchst keine Kryptowährung, um trustless zu denken. Vier Bausteine gelten für das gewöhnliche Geschäft.

**Baustein 1: Überprüfbare Identität.**
Die Frage ist: Ist das wirklich der, der er zu sein vorgibt, und kann ich das prüfen, ohne jemanden anzurufen? Digitale Zertifikate und digitale Signaturen beantworten dir das bereits jeden Tag. Wenn ein Lieferant ein Dokument mit einer anerkannten digitalen Signatur schickt, kannst du sowohl prüfen, wer es signiert hat, als auch, dass sich danach nichts geändert hat. Ein nachprüfbarer Nachweis (Verifiable Credential) geht weiter: Dein Buchhalter kann beweisen, dass er eine gültige Lizenz hält, oder ein Mitarbeiter kann beweisen, dass er eine Hintergrundprüfung bestanden hat, ohne das ganze Zertifikat zu übergeben und ohne dass du die ausstellende Stelle anrufst.

**Baustein 2: Manipulationssichere Aufzeichnungen.**
Die Frage ist: Kann jemand still die Geschichte umschreiben? Ein gemeinsames Hauptbuch ist eine Antwort. Ebenso ein einfacherer Trick namens Hash — ein kurzer Fingerabdruck, berechnet aus einer Datei. Wenn du den Fingerabdruck eines Dokuments in dem Moment aufzeichnest, in dem du es vereinbarst, und die Datei später geändert wird, wird der Fingerabdruck nicht übereinstimmen. Du kannst diesen Fingerabdruck später vorlegen und den Zustand des Dokuments damals beweisen. Das kostet fast nichts und braucht keine besondere Erlaubnis.

**Baustein 3: Programmierbare Zahlungen.**
Die Frage ist: Kann das Geld sich selbst bewegen, wenn die Bedingung erfüllt ist? Treuhand (Escrow) ist die alte Version: Ein Dritter hält Geld und gibt es bei einem Auslöser frei. Die neuere Version schreibt den Auslöser in Code, sodass zum Freigabezeitpunkt keine menschliche Entscheidung nötig ist. Meilenstein-Zahlung für einen Freiberufler ist der offensichtliche Fall: Die Zahlung wird freigegeben, wenn die Lieferung abgenommen wird, und die Abnahmeregel ist vorab aufgeschrieben.

**Baustein 4: Nachvollziehbarkeit.**
Die Frage ist: Können wir beide nachher dieselbe Wahrheit sehen? Jede Aktion sollte eine zeitgestempelte, geordnete, nicht editierbare Aufzeichnung hinterlassen. Wenn beide Seiten dieselbe Aufzeichnung lesen, werden Streitigkeiten kurz. Dein Buchhalter, dein Prüfer und dein Kunde können alle dasselbe prüfen, ohne dich um einen Gefallen zu bitten.

**Wie du heute klein anfängst:**

1. Wähle einen Prozess, bei dem du derzeit Bestätigungen hinterherjagst.
2. Schreibe die Freigabe-Bedingung als einen einzigen testbaren Satz. Wenn du sie nicht als testbaren Satz schreiben kannst, ist der Prozess nicht bereit.
3. Frage, ob eine Maschine den Auslöser messen kann. „Geliefert" bedeutet ein gescannter, unterschriebener Lieferschein. „Genehmigt" bedeutet ein Klick auf einen Genehmigungs-Button. „Abgeschlossen" bedeutet eine Statusänderung in deinem eigenen System.
4. Lege das Geld hinter eine Regel, die auf diese Messung wartet: einen Treuhandservice, einen Zahlungsplan in deinem Buchhaltungssystem oder einen Workflow, der den Auslöser vor der Freigabe verlangt.
5. Protokolliere jeden Schritt, wo beide Seiten ihn sehen können.
6. Erst dann automatisieren.

### 7.4 KI-Agenten, die miteinander interagieren: die Zukunft des automatisierten Geschäfts

Die interessante Version davon ist nahe. Dein Software-Agent spricht mit dem Software-Agenten eines Lieferanten, und sie wickeln eine Transaktion ab ohne einen Menschen bei jedem Schritt.

Damit das sicher funktioniert, müssen fünf Dinge existieren.

**Identität und Befugnis.** Nicht nur „das ist der Agent von Lieferant X", sondern „dieser Agent ist befugt, bis zu 500 Einheiten zu einem Preis unter 4,20 pro Stück zu verpflichten". Befugnis muss nachweisbar und begrenzt sein, nicht vorausgesetzt.

**Ein maschinenlesbares Geschäft.** Beide Seiten brauchen die Bedingungen in einer strukturierten Form — Menge, Preis, Lieferdatum, Strafe — nicht einen freundlichen E-Mail-Verlauf. Ein Mensch kann Mehrdeutigkeit verzeihen. Ein automatisiertes System wird entweder daran feststecken oder sie ausnutzen.

**Ein Zahlungsstrang, der warten kann.** Die Zahlung muss bedingt sein: gehalten, dann freigegeben auf Nachweis. Eine sofortige, unbedingte Zahlung entfernt jede Hebelwirkung und jeden Grund zu liefern.

**Nachweis.** Eine Lieferbestätigung, eine Abnahme-Aufzeichnung, eine unterschriebene Quittung, in einer Form, die beide Systeme lesen und die keiner still ändern kann.

**Ein Streitweg.** Etwas muss den Fall handhaben, in dem die beiden Agenten sich nicht einig sind, oder in dem die Welt nicht so lief, wie die Regel annahm. Ohne Eskalationsweg wird aus einer kleinen Uneinigkeit eine feststeckende Zahlung und ein verärgerter Lieferant.

Was jetzt realistisch ist: Agenten können bereits suchen, vergleichen, Angebote entwerfen und Bestellungen vorbereiten. Was noch nicht Routine ist, ist sie eigenständig Geld und rechtliche Bedingungen verpflichten zu lassen. Der vernünftige Weg ist, dass ein Mensch die endgültige Verpflichtung genehmigt, während der Agent alles vorbereitet. Das hält das Tempo und lässt das Risiko fallen.

### 7.5 Was das für deine Firma bedeutet: Smart Contracts, automatische Zahlungen, Nachvollziehbarkeit

**Smart Contracts, in klaren Worten.** Ein Smart Contract ist ein Programm, das eine Vereinbarung hält und sie ausführt, wenn der angegebene Zustand eintritt. Es ist nicht klug, und es ist kein Vertrag im Sinne des Anwalts. Es ist ein sehr wörtlicher Automat. Schreib die Regel sorgfältig, und es ist ein großer Diener. Schreib sie lasch, und es ist auch ein großer Diener — von dem, was du tatsächlich geschrieben hast.

**Automatische Zahlungen.** Die praktische Form ist eine Zahlung, die wartet. Sie wartet auf eine Lieferbestätigung, einen Genehmigungs-Klick, einen angenommenen Meilenstein, ein erreichtes Datum. Jede ist gedeckelt, protokolliert und für beide Seiten sichtbar, bevor sie sich bewegt.

**Nachvollziehbarkeit.** Jeder Schritt hinterlässt eine Aufzeichnung. Dein Buchhalter schließt den Monat schneller ab, weil nichts rekonstruiert werden muss. Eine Kundenstreitigkeit endet in Minuten, weil beide Seiten auf dieselbe Zeile schauen. Wenn ein Aufseher fragt, legst du die Aufzeichnung vor statt einer Geschichte.

**Wo es gut passt:** grenzüberschreitende Lieferanten-Zahlungen, wo Durchsetzung langsam ist; Freiberufler- und Auftragnehmer-Meilensteine; Marktplätze, wo Käufer und Verkäufer Fremde sind; Datenteilungs-Vereinbarungen, wo du beweisen musst, was du wann freigegeben hast; Versicherungen, die bei einem gemessenen Ereignis zahlen, wie einer Flugverspätung.

**Wo es schlecht passt:** alles, was Urteil, Verhandlung oder eine Beziehung braucht. Alles, wo der Auslöser nicht ehrlich gemessen werden kann. Alles, wo eine falsche automatische Zahlung schwer zurückzuholen ist.

## Ethik und Verantwortung

Trustless-Systeme verändern, wer rechenschaftspflichtig ist, und genau deshalb brauchen sie sorgfältiges Nachdenken.

**Code, der erzwingt, erzwingt auch Fehler.** Wenn deine Regel eine Zahlung bei einer Bedingung freigibt, die leicht zu fälschen ist, hast du einen Verlust automatisiert. Schreib die Regel für den unehrlichen Fall, nicht nur für den effizienten.

**Orakel sind Menschen.** Ein „maschinenmessbarer Auslöser" hängt oft davon ab, dass ein Mensch irgendwo Daten eingibt. Das schwächste Glied in einer trustless-Kette ist der Moment, in dem eine Person die Wahrheit hineintippt. Entwirf dafür, dass diese Person gehetzt, irrtümlich oder bestochen ist.

**Unveränderlichkeit kollidiert mit Privatsphäre.** Personenbezogene Daten auf eine dauerhafte, unveränderliche Aufzeichnung zu legen, kann mit Datenschutz-Rechten kollidieren, einschließlich dem Recht auf Löschung. Halte personenbezogene Daten von öffentlichen Hauptbüchern fern; speichere nur Verweise und Fingerabdrücke. Das rechtliche Detail ist in [Kapitel 10](ch10-privacy-and-gdpr.md).

**Entferne den Menschen nicht aus einem menschlichen Problem.** Unzufriedene Kunden wollen keine perfekt erzwungene Regel; sie wollen, dass jemand zuhört. Trustless ist für den langweiligen Mittelteil einer Transaktion, nicht für den Moment, in dem jemand verärgert ist.

**Sei transparent, und halte einen namentlichen Eigentümer.** Sag den Leuten, deren Arbeit jetzt vom System gemessen wird, und erkläre, wie eine Entscheidung umgestoßen werden kann; eine Regel, die niemand hinterfragen darf, wird irgendwann falsch sein, ohne dass jemand sie beheben kann. Automatische Durchsetzung entfernt keine Verantwortung — jemand in deiner Firma muss weiterhin das Ergebnis besitzen, wie [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md) darlegt.

## Zu vermeidende Fehler

### 7.7 Nicht alles muss trustless sein

1. **Eine Blockchain nutzen, wo eine Tabelle genügt.** Wenn die Parteien einander vertrauen, die Aufzeichnung klein ist und ein normaler Vertrag funktioniert, fügt ein verteiltes Hauptbuch nur Kosten und Komplexität hinzu.
2. **Trustless mit risikofrei verwechseln.** Code hat Fehler, Zuführungen können falsch sein, Schlüssel können verloren gehen, und es gibt oft keine Support-Nummer zum Anrufen.
3. **Einen schlechten Prozess automatisieren.** Ein trustless-System wird deinen schlechten Prozess schneller und konsequenter erzwingen, als es ein Mensch je tat.
4. **Personenbezogene Daten auf eine öffentliche Chain legen.** Sie kann später nicht gelöscht werden.
5. **Kein Not-Aus.** Jedes automatische Zahlungssystem braucht eine Möglichkeit, es mit einem Klick zu stoppen.
6. **Keine Ausgabengrenze.** Ein Agent mit einer offenen Wallet ist ein offener Scheckbuch.
7. **Dem Auslöser zu sehr vertrauen.** Frage, wie der Auslöser gefälscht werden könnte, und entscheide dann, ob das zählt.
8. **Einem Pitch hinterherjagen.** „Trustless" ist eine nützliche Design-Idee, kein Grund, einen Token zu kaufen. Wenn ein Vorschlag den Auslöser, die Aufzeichnung und den Streitweg nicht erklären kann, ist er Marketing.
9. **Jeden Vermittler ausschalten.** Manche Vermittler verdienen ihre Gebühr. Ein Notar, ein Zollagent oder ein Versicherer leisten vielleicht echte Arbeit, die Code nicht kann.
10. **Vergessen, wer rechenschaftspflichtig ist.** Auch bei automatischer Durchsetzung muss ein namentlicher Mensch das Ergebnis besitzen.

## Praktische Übung

### 7.8 Denk an einen Geschäftsprozess, der von trustless Automatisierung profitieren könnte

Wähle einen Prozess, bei dem du derzeit Zeit mit Prüfen, Hinterherjagen oder Streiten verbringst. Arbeite diese neun Fragen schriftlich durch.

1. **Wer sind die Parteien?** Nenne sie. Vermerke, ob sie einander bereits vertrauen.
2. **Was muss wahr sein, bevor Geld sich bewegt?** Ein Satz.
3. **Wer prüft das heute?** Eine Person? Wie lange dauert es? Wie oft ist es falsch?
4. **Was kostet diese Prüfung?** Zeit, Gebühren, Verzögerungen. Grobe Zahlen sind recht; markiere sie als grob.
5. **Kann eine Maschine den Auslöser messen?** Wenn ja, was ist das Signal? Wenn nein, kann der Prozess so umgestaltet werden, dass er es kann?
6. **Was ist die Nachweis-Spur?** Welche Aufzeichnung existiert, wo, und kann eine Seite sie ändern?
7. **Was passiert bei einem Streit?** Wer entscheidet, und wie schnell?
8. **Was ist der schlimmste Weg, wie das missbraucht werden könnte?** Schreib den unehrlichen Szenario vor dem effizienten.
9. **Was ist die Obergrenze?** Der maximale Verlust, wenn die Regel falsch ist.

Nun bewerte es. Wenn die Prüfkosten ein großer Teil des Transaktionswerts sind, der Auslöser maschinenmessbar ist und du eine niedrige maximale Verlustgrenze setzen kannst, ist der Prozess ein starker Kandidat. Wenn der Auslöser nicht von einer Maschine gemessen werden kann, oder der maximale Verlust hoch ist, behalte einen Menschen darin.

Schreibe eine Seite. Bring einen Kandidaten mit in dein nächstes Meeting.

## Checkliste

### 7.9 Wann eine trustless Herangehensweise in Betracht kommt

- [ ] **Du zahlst einen Vermittler hauptsächlich dafür, etwas zu halten oder zu prüfen**, und diese Prüfung könnte als Regel geschrieben werden.
- [ ] **Die Parteien vertrauen einander noch nicht**, und Vertrauen aufzubauen wäre langsam oder unmöglich.
- [ ] **Die Freigabe-Bedingung lässt sich als ein testbarer Satz angeben**, den eine Maschine messen kann.
- [ ] **Die Transaktion geschieht oft**, sodass die Einrichtungskosten auf viele Nutzungen verteilt werden.
- [ ] **Sie ist grenzüberschreitend oder unternehmensübergreifend**, wo lokale Durchsetzung langsam oder unklar ist.
- [ ] **Du brauchst eine gemeinsame, nicht editierbare Aufzeichnung**, die beide Seiten und dein Prüfer lesen können.
- [ ] **Du kannst eine harte Ausgabengrenze** und einen Ein-Klick-Stop vor dem Automatisieren setzen.
- [ ] **Keine personenbezogenen Daten müssen auf der dauerhaften Aufzeichnung liegen.**
- [ ] **Ein Streitweg existiert** und benennt einen Menschen, der die Regel überstimmen kann.
- [ ] **Du hast es ehrlich verglichen** mit einem normalen Vertrag und einem normalen Prozess, und trustless gewinnt weiterhin bei Kosten, Tempo oder Risiko.

## Wichtige Kernpunkte

- Trustless bedeutet nicht kein Vertrauen; es bedeutet, dass du eine Tatsache überprüfst, statt einer Person zu vertrauen, sie dir zu sagen.
- Die drei arbeitenden Teile sind überprüfbare Identität, manipulationssichere Aufzeichnungen und automatische Durchsetzung einer geschriebenen Bedingung.
- Ethereums Entwurf ERC-8004 und die Account-Abstraction-Standards zeigen, wohin Agent-zu-Agent-Geschäft geht: Identität, Reputation und unabhängige Validierung, mit Budgets, die durch Code begrenzt sind.
- Das schwächste Glied ist der Auslöser — der Moment, in dem ein Mensch oder ein Sensor dem System sagt, was wirklich geschah.
- Nutze trustless nicht, wo ein normaler Vertrag funktioniert; nutze es, wo Überprüfung teuer ist, der Auslöser messbar ist und der maximale Verlust gedeckelt ist.
