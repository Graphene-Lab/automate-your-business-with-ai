# Kapitel 3 — Die Sprache der KI, ohne große Wörter

## Einfach gesagt

Die meisten schlechten KI-Entscheidungen entstehen nicht durch schlechte Technik. Sie entstehen durch Wörter, die niemand genauer definieren wollte.

Ein Anbieter sagt: „Unsere KI-Plattform lässt sich über eine Low-Code-API in deine Systeme integrieren und nutzt ein großes Sprachmodell." Alle nicken. Niemand fragt, was das eigentlich bedeutet. Sechs Monate später ist das Projekt über Budget, die Daten liegen irgendwo Unerwartetes, und niemand kann sagen, wem was gehört.

Wörter sind die Schnittstelle. Wenn dein Team unter „Modell", „Training" und „Integration" nicht dasselbe versteht, kannst du über nichts davon gute Entscheidungen treffen. Du kannst zwei Anbieter nicht vergleichen. Du kannst keinen Vertrag schreiben. Du erkennst nicht, wenn etwas schiefgeht.

Dieses Kapitel ist ein Arbeitsglossar, kein Wörterbuch. Jedes Wort bekommt eine schlichte Bedeutung, einen Alltagsvergleich und die eine Frage, die du stellen solltest, wenn du es hörst.

Eine Regel zieht sich durch alles. **Eine echte Erklärung enthält immer ein Verb und ein Objekt.** Nicht „das ist KI-gesteuert", sondern „es liest deine Rechnungen und trägt die Summe in deine Buchhaltungsdatei ein". Wenn dir jemand kein Verb und kein Objekt geben kann, hat er dir nichts gesagt.

### 3.1 Daten, Information, Wissen

Drei Wörter, die Leute benutzen, als wären sie dasselbe. Es sind drei verschiedene Stufen, und der Unterschied zählt, wenn du planst.

**Daten** sind rohe Fakten ohne Bedeutung. Eine Spalte mit Zahlen. Ein Ordner mit PDFs. Eine Liste von Daten. Daten allein sagen dir nichts. Die Zahl 47 ist ein Datum.

**Information** ist Daten mit Zusammenhang. „Rechnung 47 ging über 1.200 € und wurde spät bezahlt." Jetzt bedeutet die Zahl etwas. Information ist Daten, die irgendwo eingeordnet sind.

**Wissen** ist Information plus ein Verständnis, was man damit anfangen soll. „Wenn dieser Kunde spät zahlt, dann meist, weil sein eigener Kunde spät zahlt; also mahnen wir ihn sachte, und am Ende zahlt er immer." Das ist Wissen. Es steckt im Kopf eines Menschen, und es hat Jahre gebraucht, um es aufzubauen.

Stell dir einen Aktenschrank vor. Daten sind das Papier. Information ist das Papier in einer beschrifteten Mappe. Wissen ist zu wissen, welche Mappen am Montagmorgen wichtig sind und welche bis März warten können.

**Warum das für dich wichtig ist.** KI arbeitet mit Daten. Dein Wissen übernimmt sie nicht automatisch. Du kannst einem System zehntausend Rechnungen füttern, und es wird Muster darin lernen. Warum dein größter Kunde immer absichtlich spät zahlt, wird es nicht lernen – denn das ist Wissen, das eine Person im Kopf hat und das nie aufgeschrieben wurde.

Frag vor jedem KI-Projekt: **Wie viel von dem, was diese Aufgabe zum Laufen bringt, ist als Daten aufgeschrieben, und wie viel steckt in jemandes Kopf?** Die Lücke zwischen diesen beiden Zahlen ist die Größe deines echten Problems. Sie zu schließen, ist meist schwerer – und wertvoller – als der KI-Teil.

**Frag den Anbieter:** „Welche Daten braucht ihr von uns, in welcher Form, und wie viele davon?"

### 3.2 Algorithmus, Modell, Training

**Algorithmus.** Ein Rezept. Eine klare, geordnete Abfolge von Schritten, die ein Problem löst. Kaffee kochen ist ein Algorithmus. Eine Division mit Rest ist ein Algorithmus. Ein Algorithmus braucht keinen Computer; er braucht nur Schritte. Das Wort kommt vom Namen des Mathematikers al-Chwarizmi aus dem 9. Jahrhundert, dessen Werk über schrittweises Rechnen ins Lateinische übersetzt wurde und uns schließlich das Wort gab.

**Modell.** In der üblichen KI-Sprache ist ein Modell das, was am Ende des Trainings herauskommt: eine Menge gelernter Einstellungen, mit denen du neue Fälle beantworten kannst. Stell es dir wie einen eingearbeiteten Mitarbeiter vor. Du musst ihn nicht jeden Morgen neu anlernen. Das Wissen steckt in ihm.

Das Wort wird auf zwei Arten benutzt, und vermischt man sie, entsteht Verwirrung. Im älteren Sinn ist ein Modell eine schriftliche Beschreibung, wie etwas funktioniert, etwa ein Finanzmodell in einer Tabelle. Im modernen KI-Sinn ist ein Modell eine Datei voller Zahlen, die so lange angepasst wurden, bis die Antworten stimmten. Wenn heute jemand „das Modell" sagt, meint er meist das Zweite.

**Training.** Der Weg von nichts zu einem Modell. Beispiele zeigen. Das System raten lassen. Mit der richtigen Antwort vergleichen. Nachjustieren. Viele Male wiederholen. Kapitel 2 hat den Mechanismus erklärt. Hier zählt die geschäftliche Bedeutung: **Training ist ein Schritt, für den du einmal bezahlst, und seine Qualität setzt die Obergrenze für alles danach.** Ein Modell, das mit schlechten Beispielen trainiert wurde, kann eine bessere Oberfläche nicht reparieren. Es kann nur neu trainiert werden – das heißt wieder bezahlen.

Drei Fragen, die fast jedes Gespräch klären:

1. **Was ist die Eingabe?** Was geht hinein?
2. **Was ist die Ausgabe?** Was kommt heraus?
3. **Womit wurde es trainiert?** Welche Beispiele, von wann, wie viele?

Kann ein Anbieter Frage drei nicht beantworten, kaufst du kein Modell. Du kaufst ein Versprechen.

### 3.3 Generative KI, LLM, Prompt

**Generative KI** ist KI, die neue Inhalte erzeugt, statt nur zu sortieren oder zu bewerten. Kapitel 2 hat sie definiert. Hier ist das Vokabular drumherum.

**LLM – großes Sprachmodell.** „Groß" heißt: Es hat sehr viele einstellbare Werte, gemessen in Milliarden. Diese Werte heißen **Parameter**. Ein Modell mit 13 Milliarden Parametern enthält 13.000.000.000 Zahlen. „Sprache" heißt: Es wurde mit Text trainiert. „Modell" heißt: Es ist das nutzbare Ergebnis des Trainings.

Ein LLM ist also eine sehr große Menge Zahlen, angepasst durch das Lesen enormer Textmengen, bis sie gut darin wurde, Text fortzusetzen. Das ist die ganze Sache. Es ist keine Datenbank mit Fakten. Es ist eine Text-Fortsetzungsmaschine.

**Prompt.** Der Text, den du dem Modell gibst. Deine Frage, deine Anweisung, deine Bitte. Mehr ist ein Prompt nicht.

Das Wort ist wichtiger, als es klingt, denn was du zurückbekommst, hängt stark vom Prompt ab. Ein vager Prompt gibt eine vage Antwort. Ein Prompt mit Zusammenhang, einem Beispiel und einem klaren Format gibt eine viel bessere. Gute Prompts zu schreiben, ist eine echte Geschäftsfähigkeit, und man lernt es in etwa einer Woche richtig.

Ein Prompt ist wie ein Briefing für eine freie Texterin. Ein schlechtes Briefing – „schreib irgendetwas über unser Produkt" – liefert etwas Unbrauchbares. Ein gutes Briefing – „schreib 150 Wörter für kleine Ladenbesitzer, in einfacher Sprache, in diesem Ton, und lass die Preise weg" – liefert etwas, das du gebrauchen kannst. Die Texterin ist dieselbe. Nur das Briefing hat sich geändert.

**Halluzination.** Wenn ein Modell selbstbewusst etwas Falsches behauptet. Das Wort ist ungenau, denn das Modell halluziniert nicht im medizinischen Sinn. Es setzt Text fort, so dass es richtig klingt, ohne ein eigenes Lager an Fakten, gegen das es prüfen könnte. Deshalb braucht generative KI für alles Wichtige eine Überprüfung.

**Kontextfenster.** Wie viel Text das Modell auf einmal berücksichtigen kann. Stell es dir wie einen Schreibtisch vor. Alles, was es ansehen soll, muss auf den Schreibtisch passen. Text, der nicht passt, ist schlicht nicht da. Moderne Schreibtische sind groß, aber nicht unendlich, und ein voller Schreibtisch arbeitet schlechter als ein aufgeräumter.

**Frag den Anbieter:** „Welches Modell benutzt ihr, wer hat es gebaut, und wohin gehen mein Prompt und meine Daten, wenn ich sie schicke?"

### 3.4 RPA, No-Code, Low-Code

Diese drei Wörter werden verkauft, als wären sie KI. Meistens sind sie es nicht.

**RPA – Roboter-Prozessautomatisierung.** Software, die nachmacht, was ein Mensch am Computer tut: dieses System öffnen, dieses Feld kopieren, es in jenes System einfügen, auf Speichern klicken. Sie funktioniert, indem sie Maus- und Tastaturaktionen nachahmt, oder dieselben Bildschirme benutzt, die ein Mensch benutzt. Der Begriff kam Anfang der 2000er Jahre auf.

RPA ist keine KI. Sie lernt nicht und rät nicht. Sie folgt einer aufgenommenen Abfolge haargenau. Sie ist zugleich zuverlässig und spröde. Der Vergleich ist ein Makro in einer Tabelle: Es macht jedes Mal dieselben Schritte, schnell, und bricht, wenn das Layout sich ändert.

**Wann RPA passt:** die Aufgabe ist festgelegt, fällt in großer Menge an, und die Bildschirme ändern sich nicht. Auftragsdaten hundertmal am Tag aus einer E-Mail in dein Auftragsystem kopieren ist ein klassischer RPA-Job. Das ist billig und funktioniert.

**Wann RPA falsch ist:** alles, was variiert. Wenn die Eingabe nicht immer am selben Ort ist, bricht RPA – und das bricht oft.

Ein verbreitetes und sinnvolles Muster: **KI liest und versteht die unordentliche Eingabe; RPA macht das langweilige Tippen.** Die KI übernimmt die Abwechslung. Das RPA übernimmt die Wiederholung.

**No-Code.** Werkzeuge, bei denen du eine Automatisierung durch Klicken, Ziehen und Auswählen aus einem Menü baust, ohne Programmcode zu schreiben. Gut für einfache, klare Abläufe. Schnell gestartet.

**Low-Code.** Ähnlich, aber du kannst ein wenig Code schreiben, wenn das Menü nicht bietet, was du brauchst. Flexibler, etwas technischer.

Beide sind wirklich nützlich, und beide haben eine versteckte Kosten: Sie sind leicht begonnen und schwer zu Ende gebracht. Ein No-Code-Ablauf, der auf zwanzig Schritte, drei Systeme und vier Leute wächst, die daran herumbasteln, wird schwer zu verstehen und gefährlich zu ändern. Es gibt ein bekanntes Muster: Eine Firma baut Dutzende kleiner No-Code-Automatisierungen, niemand kann sie alle überblicken, und am Ende muss jemand alles neu bauen.

**Frag den Anbieter:** „Lernt das wirklich etwas, oder folgt es einer festen Abfolge? Wenn sich ein Bildschirm ändert, was bricht, und wer repariert es?"

### 3.5 Cloud, API, Integration

**Cloud.** Ein Computer von jemand anderem. Das ist die ehrliche Definition. Deine Dateien und Programme laufen auf Maschinen in einem großen Rechenzentrum, das eine andere Firma besitzt und wartet, und du zahlst nach Nutzung über das Internet.

Die Cloud hat echte Vorteile: keine Hardware, die man kaufen muss, Kapazität, die du in Minuten vergrößern kannst, automatische Wartung. Sie hat aber auch eine dauerhafte Folge: **deine Daten liegen auf Maschinen von jemand anderem, in einem Land, das du vielleicht nicht gewählt hast, unter einem Vertrag, den du wahrscheinlich nicht gelesen hast.** [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) behandelt, wie du Dinge selbst betreibst, und [Kapitel 11](ch11-digital-sovereignty.md) behandelt Kontrolle und Souveränität.

**API – Programmierschnittstelle.** Ein festgelegter Weg, wie ein Programm ein anderes bittet, etwas zu tun.

Stell dir eine Restaurantküche vor. Du kannst nicht hineingehen und selbst kochen. Du gehst ans Fenster und bestellst von einer festen Karte. Die Küche sagt dir genau, was du bestellen kannst und wie. Dieses Fenster ist die API: Sie lässt die Außenwelt die Küche benutzen, ohne sie kaputtzumachen.

In der Praxis fragt deine Website die API des Versandunternehmens: „Was kostet es, dieses Paket nach Madrid zu schicken?", und bekommt in Sekunden eine Zahl zurück. Niemand ruft jemanden an.

Zwei Dinge zum Merken. Erstens: Hat das Produkt eines Anbieters keine API, kannst du es selbst an nichts anschließen, und du hängst für immer an diesem Anbieter. Zweitens: Jeder API-Aufruf bedeutet, dass Daten eine Grenze überschreiten. Jeder ist eine kleine Tür. Manche Türen sind verschlossen und protokolliert. Manche nicht.

**Integration.** Systeme so verbinden, dass Daten zwischen ihnen hin- und herwandern, ohne dass ein Mensch sie tragen muss. Hier verbringen die meisten Projekte tatsächlich ihre Zeit und ihr Geld, und Anbieter sagen selten, welches Niveau sie meinen:

1. **Dateien.** Eine Tabelle exportieren, irgendwo hochladen. Einfach, langsam, fehleranfällig.
2. **API.** Eine Live-Verbindung. Schnell, zuverlässig, braucht Einrichtungsarbeit.
3. **Nativ.** In dieselbe Plattform eingebaut. Am besten, aber du bindest dich an diese Plattform.

**Frag den Anbieter:** „An welche Systeme verbindet ihr euch heute, mit welcher Methode, wer richtet es ein, und was passiert mit der Verbindung, wenn wir gehen?"

## Ein bisschen Geschichte

Die Wörter sind älter als die Technik, und das zu wissen, hilft.

**Algorithmus** kommt von al-Chwarizmi, einem persischen Mathematiker aus dem 9. Jahrhundert, dessen Bücher schrittweises Rechnen beschrieben. Das Wort ist über tausend Jahre älter als der Computer. **Daten** kommt vom lateinischen Wort für „Gegebenes" – Fakten im schlichten Sinn, lange bevor es etwas Gespeichertes bedeutete. **Neuronales Netz** kommt aus den 1940er Jahren, aus frühen Versuchen, eine Gehirnzelle als kleinen Ein/Aus-Schalter zu beschreiben; der Ausdruck blieb hängen, obwohl moderne Systeme echten Gehirnen kaum ähneln. **Maschinelles Lernen** wurde 1959 von Arthur Samuel benannt, einem amerikanischen Forscher, der an einem Dame-Programm arbeitete. **Großes Sprachmodell** kam um 2018 in den allgemeinen Gebrauch, als Modelle auftauchten, die mit Text in Web-Größe trainiert waren. **Prompt** ist aus dem älteren Computing entlehnt, wo es die Stelle meinte, an der man tippt; jetzt bedeutet es die Anweisung, die du einem Modell gibst – eine viel größere Aufgabe als Tippen je war. **RPA** erschien Anfang der 2000er Jahre, um Software zu beschreiben, die einen Menschen am Bildschirm nachahmt, und **Low-Code** und **No-Code** kamen um 2014 ins Geschäftsvokabular.

Die Lehre aus dem Vokabular ist einfach. Fast keines dieser Wörter wurde von den Leuten erfunden, die die Technik gebaut haben. Sie wurden entlehnt, gedehnt und dann verkauft. Deshalb fühlen sie sich vage an. Sie sind vage. Deine Aufgabe ist es, jedes einzelne festzunageln, bevor du irgendetwas unterschreibst.

## Neugier

### 3.6 Ein Modell, das nur mit Daten aus den 1930ern trainiert war, schrieb Python – wie geht das?

Im April 2026 veröffentlichte ein kleines Forschungsteam ein ungewöhnliches Sprachmodell. Es hieß **talkie**, und sein ganzer Witz lag in dem, was es nicht wusste.

Das Team – Nick Levine, David Duvenaud von der Universität Toronto, und Alec Radford – trainierte ein Modell mit 13 Milliarden Parametern auf englischen Text, der nur vor 1931 veröffentlicht wurde. Etwa 260 Milliarden Tokens davon. Ein **Token** ist ein kleines Textstück, grob ein Wort oder ein Teil eines Wortes. Die Quellen waren digitalisierte Bücher, Zeitungen, Zeitschriften, Fachjournale, Patente und Rechtsprechung.

Nichts von nach 1930 kam hinein. Keine Computer. Kein Internet. Und entscheidend: keine Programmiersprache, denn Python wurde erst Ende der 1980er Jahre erfunden.

Dann testeten sie, ob es Python schreiben kann.

**Das Ergebnis.** Es konnte ein bisschen. Das Team gab dem Modell einen Standard-Programmiertest namens HumanEval, mit einem Kniff: Jede Aufgabe kam mit ein paar zufälligen Beispielfunktionen, die direkt in der Frage standen. Das Modell hatte im Training nie Python gesehen. Aber es konnte die Beispiele vor sich ansehen und die Struktur nachbauen.

Die Ergebnisse waren ehrlich und bescheiden. Das Oldtimer-Modell schnitt weit unter modernen Modellen ab. Jede richtige Antwort, die es hervorbrachte, war ein einfaches Ein-Zeilen-Programm, wie zwei Zahlen addieren, oder eine kleine Änderung an einem der gezeigten Beispiele. Wie das Team es formulierte, ist es noch ein weiter Weg, bis diese Fähigkeit erwähnenswert ist.

Aber ein Beispiel war wirklich verblüffend. Gezeigt bekam es eine Funktion, die eine Rotationschiffre kodierte – einen Code, bei dem jeder Buchstabe um einen festen Betrag verschoben wird –, und das Modell erzeugte die Dechiffrier-Funktion, indem es ein einziges Zeichen änderte und aus einer Addition eine Subtraktion machte. Es hatte nie Python gesehen. Es hatte nie einen Computer gesehen. Aus der Form des Beispiels vor ihm begriff es, dass Dechiffrieren das Umgekehrte von Chiffrieren ist.

**Wie ist das möglich?** Die Antwort ist ein Verhalten namens **In-Context-Lernen**: ein Muster aus den Beispielen aufgreifen, die direkt in der Frage stehen, statt aus dem Training.

Hier die schlichte Version. Um Text gut zu lesen, muss ein Modell extrem gut darin werden, Struktur zu bemerken. Welches Wort auf welches folgt. Was sich öffnet und was sich schließt. Was eine Definition ist und was ein Beispiel. Was eine Ursache ist und was eine Wirkung. Das alles lernt es aus gewöhnlichen Büchern und Zeitungen.

Struktur, so zeigt sich, wandert mit. Ein Modell, das sehr gut darin geworden ist zu bemerken „dieser Block öffnet sich hier, schließt dort, und dieser Wert fließt in jenen", kann dieselbe Fähigkeit auf einen Python-Block anwenden, den es nie gesehen hat. Es nutzt kein Python-Wissen. Es nutzt Struktur-Wissen auf Python-Material.

Deshalb konnte es die Chiffrier-Funktion umkehren. Es war kein Programmieren. Es war Musterfolgen, angewandt auf ein Thema, das in seinen Trainingsdaten nicht existierte.

**Warum die Forscher das taten.** Der Grund ist praktisch und klug: Ein Modell, das nur auf Text vor 1931 trainiert wurde, kann den Test nicht auswendig gelernt haben. Moderne Modelle werden auf dem modernen Web trainiert, das die Antworten auf die meisten öffentlichen Testfragen enthält. Das heißt **Datenkontamination**, und sie macht moderne Benchmarks unzuverlässig. Ein Modell kann gut abschneiden, weil es die Antwort schon gesehen hat, nicht weil es schlussfolgern kann. Talkie ist von der Konstruktion her sauber. Was immer es tut, es hat es wirklich getan.

**Die ehrlichen Grenzen.** Das Team berichtete auch, dass talkie insgesamt schlechter abschnitt als sein „moderner Zwilling" – ein baugleiches Modell, trainiert auf modernen Webdaten –, selbst nachdem sie korrigiert hatten, dass moderne Fragen ein 1930er-Modell verwirren. Einen Teil der Lücke schoben sie auf OCR-Rauschen: 1930 war nichts digital, also musste jede Seite gescannt und abgeschrieben werden, was Fehler einführt, die nativer digitaler Text nicht hat. Als Amateur-Forschungsprojekt, sagten sie, hätten sie nie erwartet, die Lücke ganz zu schließen. Sie schätzten aber, dass das historische Korpus auf weit über eine Billion Tokens anwachsen könnte, genug für ein Modell, das dem ursprünglichen ChatGPT etwa vergleichbar ist.

**Die geschäftliche Lehre.** Zwei Dinge.

Erstens: Diese Modelle sind eher Strukturfolger als Faktensammler. Das erklärt sowohl ihre Stärke als auch ihre Unzuverlässigkeit. Struktur wandert gut mit. Wahrheit kommt nicht mit.

Zweitens: **Datenkontamination ist ein echtes Problem bei Anbieterbehauptungen.** Wenn ein Anbieter sagt „unser Modell erreicht 94 % bei diesem Benchmark", frag, ob der Benchmark in den Trainingsdaten war. Das ist keine kleine Formalie. Es ist der Unterschied zwischen einer gemessenen Fähigkeit und einer auswendig gelernten Antwort. Frag das in jedem Anbietergespräch.

## Ein echtes Geschäftsbeispiel

### Wenn die Wörter das Produkt sind: „AI-Washing"

Im September 2024 kündigte die US-Bundeshandelskommission (Federal Trade Commission) eine Durchgriffsaktion an, die sie **Operation AI Comply** nannte. Das Ziel waren Firmen, die übertriebene oder irreführende Behauptungen darüber aufstellten, was ihre Produkte mit künstlicher Intelligenz können. Der eigene Name der FTC für diese Praxis ist **AI-Washing**.

Das Muster, das die Aufseher beschrieben, ist einfach, und es lohnt sich, es wiederzuerkennen, denn so beginnen schlechte KI-Käufe.

Eine Firma hat ein ganz gewöhnliches Produkt. Vielleicht ein Terminplanungstool, oder ein Tool für Marketing-Automatisierung, oder ein Chatbot, gebaut aus einer festen Liste von Antworten. Die Firma setzt „KI-gesteuert" ins Marketing. Am Produkt ändert sich nichts. Der Preis steigt. Die Verkäufe steigen.

Die Sicht der FTC ist: Das ist ein Verbraucherschutzproblem, kein technisches. Wenn du eine Fähigkeit behauptest, die du nicht hast, ist das eine irreführende Behauptung, und das Etikett „KI" schützt dich nicht davor.

**Warum das ein Geschäfts- und nicht nur ein Rechtsbeispiel ist.** Weil dieselbe Falle in beide Richtungen läuft. Anbieter benutzen die Wörter locker, um zu verkaufen. Einkäufer benutzen die Wörter locker, um intern ein Budget zu rechtfertigen. Ein Manager, der nicht erklären kann, was die Technik tut, schreibt „KI-gesteuerte Automatisierung" in einen Vorschlag, bekommt das Budget genehmigt und muss dann etwas zum Laufen bringen, das niemand definiert hat.

Die Durchgriffsaktion der Aufseher ist für dich nützlich als umgekehrte Checkliste. Frag vor dem Kauf:

1. **Welche konkrete Behauptung wird aufgestellt?** Schreib sie in einem Satz mit einem Verb und einem Objekt auf.
2. **Woran würden wir erkennen, dass die Behauptung falsch ist?** Wenn niemand einen Test nennen kann, ist die Behauptung Dekoration.
3. **Steht die Behauptung im Vertrag?** Marketingsprache ist kein Versprechen. Wenn eine Fähigkeit zählt, sollte sie mit einer Zahl und einem Datum aufgeschrieben sein.
4. **Wer ist verantwortlich, wenn es nicht liefert?** Nenn eine Person, keine Firma.

Ein ehrlicher Anbieter beantwortet alle vier locker. Ein wäschender Anbieter wird vage. Vagheit als Antwort auf konkrete Fragen ist selbst die Antwort.

## So machst du es

### Der Schlichtwort-Test

Benutz das, wann immer ein Fachbegriff in einem Meeting auftaucht.

**Schritt 1: Bleib bei dem Wort stehen.** Lass es nicht durchgehen, nur weil es wichtig klingt.

**Schritt 2: Verlange einen Satz mit einem Verb und einem Objekt.** Nicht „es nutzt ein großes Sprachmodell", sondern „es liest unsere Support-E-Mails und entwirft eine Antwort". Wenn der Sprecher keinen hervorbringen kann, hat das Wort noch keinen Inhalt.

**Schritt 3: Frag, was hineingeht und was herauskommt.** Jedes echte System hat eine Eingabe und eine Ausgabe. Schreib beide auf.

**Schritt 4: Frag, was es bricht.** Jede Technik hat eine Fehlerart. Ein ehrlicher Anbieter nennt seine.

**Schritt 5: Schreib deine eigene Definition in eine Zeile und lies sie vor.** Wenn ein kluger Kollege sie nicht verstehen könnte, ist die Definition nicht fertig.

### Deine Arbeits-Übersetzungstabelle

| Was du hörst | Schlichte Bedeutung | Was du fragen solltest |
|---|---|---|
| KI-gesteuert | Nutzt eine gelernte Komponente, vielleicht winzig | Welchen Teil genau? |
| Modell | Eine Datei gelernter Einstellungen, die neue Fälle beantwortet | Womit trainiert, wann, wie viel? |
| Training | Einstellungen an Beispielen anpassen, bis die Antworten passen | Wer hat es gemacht, und wer hat es geprüft? |
| LLM | Ein sehr großes Text-Fortsetzungssystem | Welches, von wem gebaut, wo laufend? |
| Prompt | Die Anweisung, die du dem Modell gibst | Können wir unsere eigenen schreiben und wiederverwenden? |
| Halluzination | Eine selbstbewusste Aussage, die falsch ist | Wie erkennt und korrigiert ihr sie? |
| RPA | Software, die einen Menschen nachahmt, der Bildschirme anklickt | Was bricht, wenn sich der Bildschirm ändert? |
| No-Code | Durch Klicken bauen, kein Programmieren | Was kann es nicht? |
| Low-Code | Meist Klicken, etwas Programmieren erlaubt | Wer wartet es hier? |
| Cloud | Läuft auf Computern von jemand anderem | Welches Land, wessen Vertrag, welche Daten gehen hinaus? |
| API | Ein festgelegtes Fenster, damit ein System ein anderes benutzt | Gibt es sie? Können wir sie selbst nutzen? |
| Integration | Daten wandern zwischen Systemen ohne einen Menschen | Welche Methode, wer richtet es ein, was, wenn wir gehen? |
| Token | Ein kleines Textstück | Wie viele pro typischer Nutzung, und was kostet das? |
| Kontextfenster | Wie viel Text das Modell auf einmal ansehen kann | Was passiert, wenn unser Dokument zu groß ist? |

### Baue ein gemeinsames Glossar für deine Firma

Mach das einmal und halte es am Leben.

1. Starte eine einzige Seite. Jeder Begriff, der in einer KI-Diskussion auftaucht, kommt darauf.
2. Jeder Eintrag bekommt drei Zeilen: die schlichte Bedeutung, was er *in unserer Firma* bedeutet, und eine Frage, die wir noch nicht beantworten können.
3. Eine namentlich genannte Person besitzt die Seite. Kein Gremium.
4. Lies die Seite vor jedem Anbietermeeting. Während des Meetings ergänze sie.
5. Nimm Einträge raus, die du nie benutzt. Halte sie unter zwei Seiten.

Ein gemeinsames Glossar ist eine kleine Sache mit großer Wirkung. Es macht aus „wir haben KI gekauft" ein „wir nutzen ein Textmodell, um Antworten zu entwerfen, und ein regelbasiertes Tool, um sie abzulegen, und ein Mensch prüft beides".

## Ethik und Verantwortung

### 3.7 Privatsphäre, Sicherheit, Bias – die Kurzfassung

Drei Wörter, die du ständig hören wirst. Hier die schlichte Einführung. Die ausführliche Behandlung liegt woanders, und du solltest diese Kapitel lesen, bevor du etwas einsetzt, das Kundendaten berührt.

**Privatsphäre** geht darum, wer persönliche Informationen sehen und benutzen darf. Die praktische Frage für jedes KI-Tool ist einfach: *Wenn ich etwas hineinkopiere, wohin geht es, wer kann es lesen, und was behalten sie?* Stecke niemals persönliche Daten eines Kunden in ein Tool, das du nicht geprüft hast. [Kapitel 10](ch10-privacy-and-gdpr.md) behandelt Datenschutzrecht und DSGVO ordentlich.

**Sicherheit** geht darum, Systeme vor Angriff, Missbrauch und Unfall zu schützen. KI bringt neue Angriffswege, etwa ein Modell mit sorgfältig formulierter Eingabe hereinzulegen oder die Daten zu vergiften, aus denen es lernt. [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md) behandelt das vollständig.

**Bias** (Verzerrung) ist, wenn ein System manche Menschen in einem Muster schlechter behandelt als andere, weil die Beispiele, aus denen es lernte, unausgewogen waren. Wenn frühere Einstellungsentscheidungen eine Gruppe begünstigt haben, wird ein darauf trainiertes Modell lernen, diese Gruppe zu begünstigen. Bias ist kein moralischer Fehler der Maschine. Er ist ein Spiegel, den man den Beispielen vorhält. [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md) behandelt Bias, Transparenz, Erklärbarkeit und menschliche Verantwortung als Teil des ganzen ethischen Rahmens.

Die eine Sache, die du aus diesem Abschnitt mitnimmst: **Du kannst ein Risiko nicht managen, das du nicht benennen kannst.** Die Wörter zu lernen, ist kein Selbstzweck. Es ist die erste Voraussetzung, um die richtigen Fragen zu stellen.

## Zu vermeidende Fehler

**Fehler 1: „KI" als Funktion hinnehmen.** Es ist keine Funktion. Es ist eine Kategorie mit Dutzenden sehr verschiedener Technologien. Frag, welche.

**Fehler 2: Zu denken, No-Code heißt kein Denken.** No-Code entfernt das Programmieren. Es entfernt nicht das Design, die Wartung oder das Risiko eines unübersichtbaren Knäuels aus Automatisierungen.

**Fehler 3: RPA mit KI verwechseln.** Wenn es einer aufgenommenen Abfolge folgt, lernt es nichts. Das kann genau das sein, was du willst, oder genau das, was scheitern wird.

**Fehler 4: Zu denken, eine API heißt, du bist integriert.** Eine API ist eine Möglichkeit, keine Verbindung. Jemand muss die Verbindung immer noch bauen und warten.

**Fehler 5: Nicht zu fragen, wo die Cloud wirklich ist.** „Die Cloud" ist ein Rechenzentrum, in einem Land, unter einem Vertrag. Frag nach welchem.

**Fehler 6: Einen Anbieter deine Begriffe definieren lassen.** Wenn das Vokabular des Anbieters das einzige im Raum ist, kontrolliert der Anbieter das Meeting.

**Fehler 7: Den Schlichtwort-Test auslassen, weil er sich langsam anfühlt.** Fünf Minuten „was heißt das eigentlich?" sind billiger als sechs Monate an einem Projekt, das niemand beschreiben kann.

**Fehler 8: Einem Benchmark glauben, ohne nach Kontamination zu fragen.** Das Talkie-Experiment existiert gerade deshalb, weil moderne Testergebnisse aufgeblasen sein können, weil die Antworten schon in den Trainingsdaten stecken.

## Praktische Übung

### 3.8 Übersetze einen technischen Satz in schlichte Wörter

Das ist die nützlichste Fähigkeit in diesem Kapitel. Übe sie an diesen sechs Sätzen. Schreib deine Antwort, bevor du die Musterantwort liest.

**Satz 1:** „Unsere Plattform nutzt ein großes Sprachmodell, um intelligente Dokumentenverarbeitung in großem Stil zu liefern."

*Musterantwort:* „Es liest Dokumente und zieht die Felder heraus, die du willst. Es nutzt ein großes Textmodell, das jemand anderes gebaut hat. ‚In großem Stil' heißt: Es kann viele auf einmal."

**Satz 2:** „Die Lösung ist ein Low-Code-RPA-Bot mit Cloud-API-Integration."

*Musterantwort:* „Ein Roboter, der Daten von einem Bildschirm auf einen anderen kopiert. Du richtest ihn meist durch Klicken ein. Er redet über das Internet mit anderen Systemen durch eine festgelegte Verbindung. Er läuft auf den Computern des Anbieters."

**Satz 3:** „Wir nutzen retrieval-augmented generation, um das Modell mit eurer Wissensbasis zu unterfüttern."

*Musterantwort:* „Bevor es antwortet, schlägt es die passenden Seiten aus deinen eigenen Dokumenten nach und nutzt sie als Grundlage. Das reduziert ausgedachte Antworten. Es funktioniert nur, wenn deine Dokumente gut und aktuell sind."

**Satz 4:** „Das Modell ist auf eure Domain-Daten feinabgestimmt."

*Musterantwort:* „Sie nahmen ein vorhandenes allgemeines Modell und trainierten es mit euren Beispielen weiter, damit es besser zu eurer Firma passt. Dafür zahlst du. Es heißt auch, dass deine Daten an jemanden geschickt wurden, der das Training gemacht hat."

**Satz 5:** „Unsere KI liefert erklärbare, transparente Entscheidungen."

*Musterantwort:* „Sie behaupten, du kannst sehen, warum es entschieden hat, wie es entschieden hat. Lass es dir zeigen, an einem echten Fall, jetzt gerade. Wenn sie das nicht können, ist die Behauptung Dekoration."

**Satz 6:** „Es ist ein Multi-Agenten-System mit Orchestrierung."

*Musterantwort:* „Mehrere KI-Komponenten arbeiten an einer Aufgabe hintereinander oder parallel, und etwas koordiniert sie. Frag: Wie viele Komponenten, was macht jede einzelne, und was passiert, wenn eine ausfällt?"

**Jetzt mach deine eigene.** Such dir einen Satz aus einer Anbieter-E-Mail, die du im letzten Monat bekommen hast. Übersetze ihn mit derselben Methode: Verb und Objekt, Eingabe, Ausgabe, was bricht. Schick deine Übersetzung an den Anbieter zurück und frag, ob sie stimmt. Seine Reaktion wird dir eine Menge verraten.

## Checkliste

### 3.9 Dein Mindest-Glossar

- [ ] Ich kann Daten, Information und Wissen erklären, und ich weiß, wie viel meines Geschäftswissens aufgeschrieben ist.
- [ ] Ich kann Algorithmus als „ein Rezept" definieren: eine geordnete Abfolge von Schritten.
- [ ] Ich kann Modell definieren als „das trainierte Ding, mit dem du neue Fälle beantwortest".
- [ ] Ich kann Training definieren als „Einstellungen an Beispielen anpassen, bis die Antworten passen".
- [ ] Ich weiß, dass ein LLM ein Text-Fortsetzungssystem ist, keine Datenbank mit Fakten.
- [ ] Ich weiß, dass ein Prompt die Anweisung ist, die ich dem Modell gebe, und dass seine Qualität das Ergebnis verändert.
- [ ] Ich weiß, was ein Token ist, und grob, was Tokens pro typischer Nutzung kosten.
- [ ] Ich weiß, was ein Kontextfenster ist, und was passiert, wenn ein Dokument zu groß dafür ist.
- [ ] Ich weiß, dass „Halluzination" eine selbstbewusste falsche Aussage bedeutet, und dass sie eine Überprüfung braucht.
- [ ] Ich kann RPA von KI unterscheiden, und ich weiß, dass RPA billig und spröde ist.
- [ ] Ich weiß, dass No-Code und Low-Code das Programmieren entfernen, nicht das Design oder die Wartung.
- [ ] Ich weiß, dass „die Cloud" Computer von jemand anderem bedeutet, in einem bestimmten Land, unter einem bestimmten Vertrag.
- [ ] Ich weiß, dass eine API ein festgelegtes Fenster ist, damit ein System ein anderes benutzt, und ich frage immer, ob es eine gibt.
- [ ] Ich kenne die drei Stufen der Integration: Dateien, API, nativ.
- [ ] Ich benutze den Schlichtwort-Test: ein Verb, ein Objekt, eine Eingabe, eine Ausgabe und was bricht.
- [ ] Ich habe ein einseitiges gemeinsames Glossar mit einer namentlich genannten Besitzerin begonnen.
- [ ] Ich weiß, dass Privatsphäre, Sicherheit und Bias je ein eigenes Kapitel haben, und ich habe sie gelesen oder werde sie lesen.

## Kernaussagen

- Die meisten schlechten KI-Entscheidungen kommen von undefinierten Wörtern, nicht von schlechter Technik.
- Eine echte Erklärung enthält immer ein Verb und ein Objekt; wenn du keines nennen kannst, wurde dir nichts gesagt.
- Modelle sind Strukturfolger, keine Faktenhüter – deshalb übertragen sie Fähigkeiten über Themen hinweg, und deshalb behaupten sie Falsches selbstbewusst.
- Das Talkie-Experiment zeigt, dass ein Modell ohne Wissen über Computer trotzdem ein bisschen Python schreiben kann, und es existiert, weil moderne Benchmark-Ergebnisse durch kontaminierte Daten aufgeblasen sein können.
- Nagel jeden Begriff fest, bevor du unterschreibst: was hineingeht, was herauskommt, was ihn bricht, und wem er gehört.
