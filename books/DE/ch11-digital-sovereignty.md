# Kapitel 11 — Digitale Souveränität: Das Recht, deine KI zu kontrollieren

## In einfachen Worten

Souveränität bedeutet in ihrer ältesten Form das Recht, dich selbst zu regieren, ohne dass dir jemand anderes sagt, was du tun sollst. Digitale Souveränität nimmt diese Idee und wendet sie auf dein digitales Leben an: das Recht, deine eigenen Daten, deine eigene Software und die Maschinen, auf denen sie laufen, zu kontrollieren.

Auf die KI angewendet beantwortet digitale Souveränität drei schlichte Fragen zu jedem KI-Werkzeug, das du nutzt.

- **Wo sind meine Daten?** In welchem Land, auf den Servern welches Unternehmens, unter welchem Gesetz?
- **Wer kann darauf zugreifen?** Die Mitarbeiter des Anbieters, Subunternehmer oder eine ausländische Regierung?
- **Wie werden sie verarbeitet?** In einem Modell, das ich nicht sehen kann, oder in einem System, das ich prüfen und verändern kann?

Wenn du diese drei Fragen nicht beantworten kannst, hast du über diesen Teil deines Unternehmens keine Souveränität. Du hast die von jemand anderem geliehen, und du kannst sie verlieren, wann immer er es sich anders überlegt.

Das ist nicht dasselbe wie Self-Hosting, auch wenn sich beide überschneiden. Self-Hosting, behandelt in [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md), ist ein Weg, Kontrolle zu gewinnen. Digitale Souveränität ist das weitere Ziel: Kontrolle darüber, woher deine digitalen Fähigkeiten kommen und wer die Leine hält. Du kannst sie mit eigenen Servern anstreben, mit offener Software, mit Verträgen oder mit einer Mischung.

Ein nützlicher Vergleich ist das Essen. Du kannst Fertiggerichte aus einer Fabrik kaufen, die du nie zu Gesicht bekommst, und die meisten Tage ist das in Ordnung. Aber wenn du eine Allergie hast oder einfach wissen willst, was in deinem Essen steckt, beginnst du dich für das Rezept und die Küche zu interessieren. Digitale Souveränität heißt, sich um das Rezept und die Küche deiner KI zu kümmern — nicht aus Angst, sondern weil deine Daten, deine Kunden und deine Zukunft auf dem Spiel stehen.

Der gegenteilige Fall — unkontrollierte Drittanbieter-Dienste und Schatten-KI — ist in [Kapitel 9](ch09-third-party-services-and-shadow-ai.md) beschrieben. Die rechtlichen Pflichten bei personenbezogenen Daten stehen in [Kapitel 10](ch10-privacy-and-gdpr.md). Dieses Kapitel handelt von der strategischen Wahl: wie viel deiner KI du wirklich kontrollieren willst.

## Ein wenig Geschichte

**2000er bis 2010er: Bequemlichkeit löscht die Frage aus.** Als Unternehmen in die Cloud gingen, fragte fast niemand, wohin die Daten wandern. Die Werkzeuge waren gut und billig. Kontrolle war kein Kaufkriterium.

**2013: Snowden verändert die Stimmung.** Die Enthüllungen über Massenüberwachung machten Regierungen und Unternehmen klar, dass Daten, die in einem anderen Land gespeichert sind, von den Behörden dieses Landes erreicht werden können. Die Frage „Wo sind meine Daten" wurde eine Sicherheitsfrage, nicht nur eine Frage der Privatsphäre.

**2018: Die DSGVO macht den Standort rechtlich relevant.** Das europäische Datenschutzgesetz gab den Menschen Rechte über ihre Daten und machte Unternehmen dafür verantwortlich, wo sie lagen und wie sie behandelt wurden. Datenspeicherung in einer Region — Daten innerhalb einer Region zu halten — wurde eine echte Anforderung, kein Slogan.

**2019 bis 2022: „Souveräne Cloud" taucht auf.** Cloud-Anbieter begannen, souveräne Optionen anzubieten: Daten, die in einem bestimmten Land gehalten werden, betrieben nach lokalem Recht, manchmal mit lokalen Partnern. Souveränität wurde ein Produktmerkmal.

**2022 bis 2023: Open-Weight-Modelle eröffnen einen neuen Weg.** Als starke KI-Modelle herunterladbar und für jedermann ausführbar wurden, konnte ein Unternehmen zum ersten Mal ein leistungsfähiges Modell vollständig nach seinen eigenen Bedingungen betreiben. Souveränität war nicht mehr nur ein Versprechen eines Cloud-Anbieters; sie wurde etwas, das man selbst bauen konnte.

**2024 bis 2025: Souveränität wird zur nationalen und unternehmerischen Strategie.** Länder und Bündnisse begannen, KI-Fähigkeit als strategisch zu behandeln. Europa startete geförderte Projekte zum Aufbau eigener offener Modelle, damit europäische KI nicht vollständig von ausländischen Anbietern abhängt. Der Abschnitt „Curiosity" behandelt eines davon.

Der Bogen ist klar. Bequemlichkeit hat uns aufgehören lassen zu fragen, wer unsere Werkzeuge kontrolliert. Eine Reihe von Schocks hat uns wieder fragen lassen. Jetzt ist Kontrolle eine Designentscheidung, die du bewusst treffen kannst.

## Curiosity

### 11.6 Einen eigenen Assistenten bauen — und ein Kontinent tut dasselbe

**Ein repräsentatives Muster (illustrativ).** Stell dir eine mittelgroße Professional-Firma vor — sagen wir ein Ingenieurbüro oder eine Anwaltskanzlei —, die einen internen KI-Assistenten braucht, um Fragen zu ihren eigenen Dokumenten zu beantworten: frühere Berichte, Normen, Verträge und Notizen. Die Daten sind vertraulich und dürfen das Gebäude nicht verlassen.

Statt diese Daten an einen öffentlichen KI-Dienst zu schicken, tut die Firma etwas anderes. Sie lädt ein Open-Weight-Modell herunter — ein Modell, dessen trainierte Dateien veröffentlicht sind, damit jeder es ausführen kann — und betreibt es auf ihren eigenen Servern. Sie verbindet das Modell über Retrieval mit ihren Dokumenten, sodass der Assistent aus den Dateien der Firma antwortet und nicht aus dem offenen Internet. Keine Frage verlässt das Netzwerk. Kein Anbieter liest die Arbeit. Die Firma wählt das Modell, kontrolliert die Daten und kann das System ändern oder ersetzen, wann immer sie will.

Dieses Muster ist real und wird immer üblicher, aber die konkrete Firma hier ist ein zusammengesetztes Beispiel, keine einzelne namentlich genannte Firma, denn Organisationen, die das tun, werben selten damit — der ganze Punkt ist, dass die Arbeit privat bleibt. Was zählt, ist, dass das Muster existiert und heute mit Standard-Tools aus dem Regal funktioniert, genau wie [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) es beschreibt.

**Eine echte, namentlich genannte Version auf nationaler Ebene.** Derselbe Instinkt treibt inzwischen ganze Länder. In Europa zielen zwei geförderte Projekte darauf ab, souveräne, offene KI-Modelle zu bauen, damit der Kontinent nicht von ausländischen Anbietern abhängt.

**OpenEuroLLM** ist ein europäisches Konsortium mit zwanzig Partnern, das am 1. Februar 2025 seine Arbeit aufnahm, gefördert im Rahmen des Digital Europe Programme der EU mit rund 55 Millionen €. Es wird von Jan Hajic von der Karls-Universität koordiniert und von Peter Sarlin von AMD Silo AI mitgeleitet. Das erklärte Ziel ist strategische Autonomie für Europa bei KI — der Aufbau von Fähigkeit, die Europa kontrolliert.

Daneben hat das Projekt **EuroLLM**, unterstützt von Horizon Europe, dem Europäischen Forschungsrat und der EuroHPC-Organisation für Hochleistungsrechnen, **EuroLLM-22B** hervorgebracht, ein vollständig offenes großes Sprachmodell, gebaut für alle 24 Amtssprachen der EU. Es wurde auf europäischen Supercomputern trainiert — dem System MareNostrum 5 — und als Open Source auf Hugging Face veröffentlicht, sodass jeder es herunterladen, prüfen und ausführen kann. Die Arbeit stützt sich auf die EuroHPC-Initiative „AI Factories", die Rechenleistung über Europa hinweg bündelt; ein Aufruf stellte drei Millionen GPU-Stunden auf dem Leonardo Booster am CINECA in Italien für den Aufbau offener Trainingsdaten bereit.

Warum erzähle ich diese Geschichte hier? Weil sie zeigt, dass „baue dein eigenes, halte es offen, halte es unter deiner Kontrolle" kein paranoides Hobby ist. Es ist inzwischen offizielle Strategie auf der Ebene von Nationen. Dieselbe Logik, die ein Land dazu bringt, ein eigenes offenes Modell zu bauen, bringt eine kleine Firma dazu, ein offenes Modell auf ihrem eigenen Server zu betreiben. Der Maßstab unterscheidet sich; das Prinzip ist identisch.

## Ein echtes Geschäftsbeispiel

### Die Klinik, die ihre Daten nirgendwo hinschicken konnte

Eine private medizinische Klinik will KI nutzen, um Patientenakten zusammenzufassen und Routinekorrespondenz zu entwerfen. Die Daten sind Gesundheitsdaten — die am strengsten geschützte Art vor dem Gesetz, wie [Kapitel 10](ch10-privacy-and-gdpr.md) erklärt. Sie an einen KI-Dienst eines Drittanbieters zu schicken, wirft ernste rechtliche und ethische Probleme auf, und die Klinik fühlt sich dabei unabhängig vom Gesetz unwohl.

Also wählt die Klinik Kontrolle. Sie betreibt ein offenes Modell auf ihrem eigenen Server, innerhalb ihres eigenen Netzwerks, hinter ihrer eigenen Firewall. Das Modell liest nur die Notizen der Klinik und antwortet nur dem Klinikpersonal. Nichts geht über das Internet an einen Anbieter. Die Klinik kann Patienten, Aufsichtsbehörden und ihrem eigenen Gewissen wahrheitsgemäß sagen: Diese Daten haben unser Gebäude nie verlassen.

Die Kosten sind real. Die Klinik musste Hardware kaufen und jemanden finden, der sie wartet. Das Modell ist gut, aber nicht das absolut beste verfügbare. Manche Aufgaben brauchen weiterhin einen Menschen. Aber die Klinik hat das eine gewonnen, das sie bei keinem Anbieter kaufen konnte: Gewissheit darüber, wohin ihre sensibelsten Daten gehen.

Jetzt vergleiche die Klinik mit einer Firma, die nicht darüber nachgedacht hat und Patientendaten in einen kostenlosen Chatbot eingefügt hat. Der Unterschied ist nicht Intelligenz. Der Unterschied ist, dass die eine Firma zuerst die drei Souveränitätsfragen gestellt hat und die andere nie.

## Wie man es macht

### 11.1 Was digitale Souveränität ist: eine einfache Definition

Digitale Souveränität ist die Fähigkeit, deine eigenen digitalen Ressourcen und Entscheidungen zu kontrollieren, statt von denen anderer abzuhängen.

Im Einzelnen hat sie drei Ebenen.

**Datensouveränität.** Du kontrollierst, wo deine Daten gespeichert sind, wer darauf zugreifen kann und unter welches Gesetz sie fallen. Du kannst sie verschieben oder löschen.

**Operationale Souveränität.** Du kontrollierst die Systeme, die deine Daten verarbeiten. Du kannst sie betreiben, verändern und am Laufen halten, selbst wenn ein Lieferant verschwindet.

**Strategische Souveränität.** Du kontrollierst deine eigene Richtung. Deine Zukunft wird nicht als Geisel gehalten von der Preisgestaltung eines Anbieters, den Regeln einer ausländischen Regierung oder den Geschäftsentscheidungen eines Lieferanten.

Souveränität ist nicht Alles-oder-Nichts. Sie ist ein Regler, kein Schalter. Du kannst über den einen Prozess hochgradig souverän sein und über einen anderen kaum. Das Ziel ist, bewusst zu entscheiden, wo du den Regler für jeden Teil deines Unternehmens haben willst, statt in das zu driften, was gerade am bequemsten ist.

Das Gegenteil von Souveränität ist eine Abhängigkeit, die du nicht gewählt hast — ein Zustand, in dem eine Änderung in den Plänen von jemand anderem eine Änderung bei dir erzwingt.

### 11.2 Warum es für Unternehmen zählt: wissen, wo die Daten sind, wer zugreift, wie sie verarbeitet werden

Souveränität zählt, weil die drei Fragen echte Folgen haben.

**Wo die Daten sind.** Daten, die in einem anderen Land gespeichert sind, fallen unter die Gesetze dieses Landes. Eine ausländische Behörde kann möglicherweise Zugriff erzwingen. Der Standort des Rechenzentrums eines Anbieters ist kein Detail am Rande; er bestimmt den rechtlichen Boden, auf dem deine Daten stehen.

**Wer darauf zugreift.** Ein Drittanbieter-Dienst kann eigenen Mitarbeitern, Support-Teams und Subunternehmern den Zugriff auf deine Daten erlauben, in Ländern, denen du nie zugestimmt hast. Du siehst vielleicht nie eine Liste von ihnen. Souveränität heißt, dass du diesen Zugriff kennst oder kontrollierst.

**Wie sie verarbeitet werden.** Wenn die Verarbeitung in einem geschlossenen System stattfindet, das du nicht prüfen kannst, kannst du nicht verifizieren, was es mit deinen Daten tut oder ob es fair ist. Wenn du das System betreibst, kannst du hineinschauen.

Das zählt aus drei praktischen Gründen. **Compliance:** Gesetze wie die DSGVO verlangen, dass du die Datenverarbeitung kennst und kontrollierst. **Sicherheit:** Jede zusätzliche Partei mit Zugriff ist eine zusätzliche Chance auf eine Verletzung. **Geschäftskontinuität:** Wenn ein Anbieter ausfällt, die Preise erhöht oder durch Sanktionen abgeschnitten wird, ist Souveränität der Unterschied zwischen einem Rückschlag und einer Krise.

Souveränität ist keine Ideologie. Sie ist Risikomanagement für den Teil deines Unternehmens, der auf Daten läuft.

### 11.3 Proprietäre Modelle vs. Open-Source-Modelle: was sich wirklich ändert

Die Wahl zwischen einem proprietären Modell und einem Open-Source-Modell ändert mehrere Dinge auf einmal.

**Ein proprietäres Modell** ist ein geschlossenes Produkt. Du nutzt es über einen Dienst oder eine API. Du kannst nicht sehen, wie es funktioniert, du kannst es nicht selbst ausführen und du kannst es nicht verändern. Du hängst für Zugang, Preis und Kontinuität vom Eigentümer ab. Die Bequemlichkeit ist hoch; die Kontrolle ist niedrig. Wenn der Eigentümer die Bedingungen ändert oder den Dienst einstellt, passt du dich an oder du hörst auf.

**Ein Open-Source- oder Open-Weight-Modell** veröffentlicht seinen Code oder seine trainierten Dateien, sodass du es selbst herunterladen und ausführen kannst. Du kannst es prüfen, auf eigener Hardware betreiben, feinabstimmen und weiter nutzen, selbst wenn der ursprüngliche Ersteller verschwindet. Die Kontrolle ist hoch; die Bequemlichkeit ist geringer, weil du es betreiben und warten musst.

Was sich wirklich ändert, ist **wer die Macht hält und wer die Last trägt.** Proprietär gibt die Macht an den Anbieter ab und nimmt dir die Last ab. Offen gibt dir die Macht und gibt dir die Last.

Keines ist automatisch besser. Proprietär ist richtig, wenn du Fähigkeit ohne Wartung willst und die Daten nicht sensibel sind. Offen ist richtig, wenn du Kontrolle, Transparenz oder Unabhängigkeit brauchst und die Arbeit stemmen kannst. Viele Unternehmen nutzen beides: proprietär für bequeme Aufgaben mit wenig Risiko, offen und selbst betrieben für die Daten und Prozesse, die am meisten zählen.

Eine Warnung: „offen" ist ein Spektrum, und die Lizenz zählt. Manche offenen Modelle schränken die kommerzielle Nutzung ein oder wie du deine Nutzung beschreiben darfst. Lies die Lizenz, bevor du darauf aufbaust.

### 11.4 Die Rolle von Open Source: Transparenz, Kontrolle, Gemeinschaft

Open Source ist das wichtigste Werkzeug digitaler Souveränität, aus drei Gründen.

**Transparenz.** Weil der Code oder die Gewichte veröffentlicht sind, kannst du sie selbst oder eine dritte Partei lesen und prüfen, was das System tatsächlich tut. Man verlangt nicht von dir, einer Blackbox zu vertrauen. Das ist derselbe Instinkt hinter den Prüfideen in [Kapitel 7](ch07-trustless-trust-without-trusting.md).

**Kontrolle.** Du kannst es dort betreiben, wo du willst, es an deine Bedürfnisse anpassen und es so lange behalten, wie du willst. Niemand kann es dir wegnehmen oder ein Upgrade erzwingen, das du nicht verlangt hast.

**Gemeinschaft.** Ein offenes Projekt wird von vielen Menschen gepflegt, nicht von der Roadmap eines einzelnen Unternehmens. Fehler werden von Außenstehenden gefunden. Das Projekt kann das ursprüngliche Team überleben. Du bist nicht allein, wenn etwas kaputtgeht.

Open Source senkt auch die Einstiegshürde. Eine kleine Firma kann dasselbe offene Modell nutzen wie eine große. Das gleicht das Spielfeld auf eine Weise aus, die proprietäre Produkte nicht tun.

Aber Open Source ist im echten Sinne nicht kostenlos. Jemand muss es installieren, aktualisieren, absichern und unterstützen. Wenn du niemanden hast, der das tut, kann Open Source zur Belastung werden. Souveränität, die du nicht warten kannst, ist schlimmer als bequeme Abhängigkeit. Nutze Open Source dort, wo du die Fähigkeit hast oder einstellen kannst.

### 11.5 Wie man eine souveräne KI-Infrastruktur aufbaut: die konkreten Schritte

Wenn du dich entscheidest, Kontrolle zu gewinnen, hier ist ein praktischer Pfad.

1. **Entscheide, was souverän sein muss.** Liste die Daten und Prozesse auf, die nicht von Außenstehenden abhängen dürfen — sensible Daten, Kern-Workflows, regulierte Arbeit. Nicht alles braucht diese Behandlung.
2. **Wähle offene Modelle.** Nimm Open-Weight-Modelle, deren Lizenz zu deiner Nutzung passt. Passe die Größe an deine Aufgabe an, wie [Kapitel 8](ch08-self-hosting-keep-your-data-under-control.md) erklärt.
3. **Betreib sie auf Infrastruktur, die du kontrollierst.** Das kann ein Server in deinem Büro sein, eine Maschine in deinem eigenen Cloud-Konto unter deinen eigenen Schlüsseln oder eine lokale Workstation für einen kleinen Start.
4. **Halte die Daten lokal und verbunden.** Nutze Retrieval, sodass der Assistent aus deinen eigenen Dokumenten antwortet, ohne sie hinauszuschicken.
5. **Kontrolliere Zugriff und Schlüssel.** Du hältst die Zugangsdaten. Kein Dritter hat eine Hintertür. Protokolliere, wer was tut.
6. **Plane die Wartung.** Bestimme namentlich, wer das System installiert, aktualisiert, absichert und sichert. Schreibe das Runbook.
7. **Halte für alles einen Ausgang offen.** Selbst für die Teile, die du proprietär hältst, sorge dafür, dass du Daten exportieren und Werkzeuge austauschen kannst. Souveränität schließt die Fähigkeit zu gehen ein.
8. **Prüfe den rechtlichen Boden.** Bestätige Datenspeicherung sowie die Pflichten des AI Act und der DSGVO für das Setup, wie [Kapitel 5](ch05-rules-and-legal-responsibility.md) und [Kapitel 10](ch10-privacy-and-gdpr.md) behandeln.
9. **Fang klein an und wachse.** Teste einen souveränen Workflow, beweise, dass er funktioniert, und erweitere dann. Baue nicht die ganze Firma auf einmal um.

Das Ziel ist nicht vollständige Unabhängigkeit. Es ist bewusste Kontrolle über die Teile, die zählen, mit einer klaren Linie zwischen dem, was du selbst betreibst, und dem, was du mietest.

## Ethik und Verantwortung

Souveränität trägt ihre eigenen ethischen Pflichten, und es ist leicht, sie falsch zu verstehen.

**Kontrolle ist nicht dasselbe wie gut.** Ein souveränes System kann trotzdem voreingenommen, falsch oder unfair sein. Es selbst zu betreiben macht es nicht ethisch. Die Pflichten in [Kapitel 4](ch04-ethical-ai-doing-the-right-thing.md) gelten weiterhin.

**Souveränität darf nicht zu Geheimnistuerei werden.** „Wir kontrollieren es" ist kein Grund zu verbergen, wie du mit den Daten von Menschen umgehst. Du schuldest Kunden und Aufsichtsbehörden weiterhin Transparenz. Kontrolliere das System; versteck dich nicht vor Prüfung.

**Nutze Souveränität nicht, um Zusammenarbeit zu umgehen.** Manche Probleme — Betrug, Schaden, rechtliche Anfragen — verlangen die Zusammenarbeit mit Behörden. Souveränität dient dem Schutz der Unschuldigen, nicht der Blockade legitimer Aufsicht.

**Sei ehrlich über deine Grenzen.** Wenn du volle Souveränität behauptest, aber das System nicht patchen, sichern oder prüfen kannst, ist die Behauptung leer und irreführend. Sag, was du kontrollierst und was nicht.

**Wiege das Gemeinwohl ab.** Offene Modelle und geteilte Forschung nützen allen. Eine Welt, in der jede Firma eine geschlossene Silo baut, verliert etwas. Der gesündeste Ansatz ist, das Sensible zu kontrollieren und zum Geteilten beizutragen.

## Zu vermeidende Fehler

### 11.7 Souveränität um ihrer selbst willen

Der häufigste Fehler ist, Souveränität als Ideal zu jagen statt als Werkzeug.

Souveränität kostet Geld, Zeit und Fähigkeiten. Wenn du sie überall anstrebst, gibst du viel aus, um Dinge zu kontrollieren, die nie Kontrolle brauchten. Du baust vielleicht ein teures On-Premise-System für Daten, die nie sensibel waren, während ein billiger, vertraglich gebundener Dienst dir gute Dienste geleistet und deine Leute für echte Arbeit freigemacht hätte.

Der Test ist nicht „Kann ich das kontrollieren?". Er ist „Was verliere ich, wenn ich das nicht kontrollieren kann?". Wenn die Antwort wenig ist, gib nichts aus, um es zu kontrollieren. Spare dein Souveränitätsbudget für die Daten und Prozesse, wo Kontrollverlust wirklich wehtut — sensible Daten, regulierte Arbeit und die Systeme, ohne die dein Unternehmen nicht laufen kann.

Souveränität ist ein Mittel, kein Zweck. Kaufe sie dort, wo das Risiko die Kosten rechtfertigt, und sei bequem abhängig, wo nicht.

Über diese Falle hinaus achte auf Folgendes:

1. **Eine Festung bauen, die du nicht warten kannst.** Souveränität ohne Wartungsverantwortlichen wird ein kaputtes System und ein falsches Sicherheitsgefühl.
2. **Open Source mit kostenlos verwechseln.** Jemand muss es betreiben. Plane das ein.
3. **Die Lizenz ignorieren.** Offen heißt nicht immer, dass du es nutzen darfst, wie du willst.
4. **Annehmen, lokal gleich sicher.** Ein souveräner Server braucht trotzdem Sicherheit, wie [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md) behandelt.
5. **Aus Prinzip alle Anbieter kappen.** Viele Anbieter haben ihren Platz verdient. Totale Unabhängigkeit ist selten ihr Geld wert.
6. **Kein Ausstiegsplan für die gemieteten Teile.** Souveränität schließt die Fähigkeit ein, jeden einzelnen Anbieter zu verlassen.
7. **Kunden zu viel versprechen.** Behaupte keine Kontrolle, die du nicht hast.
8. **Ignorieren, dass offene Modelle trotzdem leak können.** Ein Modell, das auf schlechten Daten trainiert wurde, kann weiterhin personenbezogene Daten offenlegen, wie [Kapitel 10](ch10-privacy-and-gdpr.md) anmerkt.

## Praktische Übung

### 11.8 Definiere dein gewünschtes Maß an Souveränität

Nimm eine Stunde und bilde deine KI-Nutzungen auf einem einfachen Kontrollregler ab.

Liste jede KI-Nutzung in deinem Unternehmen auf. Beantworte für jede drei Fragen und lege ein Zielniveau fest.

- **Wie sensibel sind die Daten?** Niedrig (öffentlich oder harmlos), Mittel (intern), Hoch (kundengeheim, reguliert oder personenbezogen).
- **Wie kritisch ist der Prozess?** Niedrig (nice to have), Mittel (täglich genutzt), Hoch (das Geschäft steht ohne ihn still).
- **Was kostet der Kontrollverlust?** Niedrig, Mittel oder Hoch.

Jetzt setze für jede ein Ziel:

- **Hohe Sensibilität oder hohe Kritikalität → zielt hoch.** Betreib es selbst oder unter einem Vertrag, der dir echte Kontrolle und einen Ausgang gibt.
- **Niedrige Sensibilität und niedrige Kritikalität → zielt niedrig.** Ein bequemer Drittanbieter-Dienst ist in Ordnung; verschwende kein Geld damit, ihn zu kontrollieren.
- **Gemischt → zielt mittig.** Nutze einen Anbieter, aber halte die Daten exportierbar und den Workflow austauschbar.

Schreibe pro Nutzung einen Satz: *„Für [Nutzung] will ich [hohe/mittlere/niedrige] Souveränität, weil [Grund]."*

Das Ergebnis ist deine Souveränitätskarte. Sie sollte eine bewusste Mischung zeigen, nicht eine einzelne Antwort. Wenn alles „hoch" ist, gibst du zu viel aus. Wenn alles „niedrig" ist, bist du bei den Dingen, die zählen, ungeschützt. Passe an, bis die Karte zu deinem echten Risiko passt.

## Checkliste

### 11.9 Die Säulen digitaler Souveränität

Nutze dies, um zu prüfen, ob ein gegebenes KI-Setup dir echte Kontrolle gibt.

- [ ] **Du weißt, wo die Daten gespeichert sind** — das Land und der Betreiber.
- [ ] **Du weißt, wer darauf zugreifen kann** — Anbietermitarbeiter, Subunternehmer und jeder staatliche Zugriff.
- [ ] **Du kannst die Daten verschieben oder löschen**, wann immer du willst.
- [ ] **Du kannst deine Daten exportieren** in einem gängigen, nutzbaren Format (kein Lock-in).
- [ ] **Du weißt, wie die Daten verarbeitet werden** — oder du betreibst die Verarbeitung selbst.
- [ ] **Du nutzt offene Modelle, wo Kontrolle zählt**, und du hast ihre Lizenzen gelesen.
- [ ] **Du hältst die Schlüssel und Zugangsdaten** zu den Systemen, die zählen.
- [ ] **Du hast einen namentlich benannten Wartungsverantwortlichen** für alles, was du selbst betreibst, mit einem schriftlichen Runbook.
- [ ] **Du hast einen Ausstiegsplan** für jeden Anbieter, damit kein einzelner Provider dich als Geisel halten kann.
- [ ] **Du hast den rechtlichen Boden geprüft** — Datenspeicherung, DSGVO und AI Act.
- [ ] **Du hast ein bewusstes Souveränitätsniveau** für jede Nutzung festgelegt, nicht einen Standardwert.
- [ ] **Du kannst deine eigenen Behauptungen verifizieren** — wenn du sagst, die Daten bleiben drin, kannst du es beweisen.

Wenn bei einer Nutzung mit hohem Risiko eine Säule fehlt, ist das deine Priorität zur Behebung.

## Kernaussagen

- Digitale Souveränität bedeutet zu kontrollieren, wo deine Daten sind, wer darauf zugreift und wie sie verarbeitet werden — und in der Lage zu sein, diese drei Fragen für jedes KI-Werkzeug zu beantworten.
- Sie ist ein Regler, kein Schalter: Stelle sie bewusst hoch ein für sensible und kritische Arbeit, und niedrig, wo Bequemlichkeit harmlos ist.
- Open-Source- und Open-Weight-Modelle geben dir Transparenz, Kontrolle und Gemeinschaft, aber nur, wenn du die Fähigkeit hast, sie zu betreiben und zu warten.
- Souveränität ist ein Mittel, kein Zweck; sie überall zu jagen verschwendet Geld, also kaufe sie nur dort, wo Kontrollverlust wirklich wehtut.
- Echte Souveränität schließt immer einen Ausgang ein: Halte deine Daten exportierbar, damit kein einzelner Anbieter dein Unternehmen als Geisel halten kann.
