# Kapitel 20 — KI sicher einführen

## In einfachen Worten

Wenn du KI in dein Unternehmen holst, lässt du eine neue Arbeitskraft mit deinen Daten umgehen. Wie jeder Arbeitnehmer muss auch diese neue Arbeitskraft vertrauenswürdig, beaufsichtigt und begrenzt sein. Dieses Kapitel handelt davon, wie man das tut — wie du KI nutzt, ohne die Daten deiner Kunden, deine Finanzen oder deine Geheimnisse preiszugeben.

Sicherheit ist kein Produkt, das man kauft. Sie ist ein Satz Gewohnheiten, die man aufbaut. Das Ziel ist einfach: **Gestalte deine Automatisierungen so, dass deine Daten auch dann geschützt bleiben, wenn etwas schiefgeht.** Diese Idee hat einen Namen — **Security by Design** — und bedeutet, dass du von Anfang an an Sicherheit denkst, nicht als nachträglichen Einfall nach einer Datenpanne.

Ein gutes Bild ist ein Haus. Du lässt die Haustür nicht weit offen, weil „noch nichts Schlimmes passiert ist". Du schließt Türen ab, du begrenzt, welche Räume Gäste betreten dürfen, du setzt ein Licht auf eine Zeitschaltuhr, und du hast einen Plan, falls du nach Hause kommst und ein Fenster offen ist. KI-Sicherheit ist dasselbe mehrschichtige Denken: Kontrolliere, wer reinkommt, schütze, was drinnen ist, beobachte, was geschieht, und wisse, was zu tun ist, wenn etwas bricht.

Dieses Kapitel behandelt die Kerngewohnheiten: sichere Automatisierungen entwerfen, kontrollieren, wer was tun darf, Daten verschlüsseln, damit Diebe sie nicht lesen können, beobachten und protokollieren, was die KI tut, für den Tag planen, an dem etwas schiefgeht, und deine Mitarbeiter schulen — denn der menschliche Faktor ist die erste Verteidigungslinie.

Eine ehrliche Wahrheit vorweg: Kein System ist vollkommen sicher. Das Ziel ist nicht Perfektion; es ist, dein Unternehmen zu einem schweren Ziel zu machen und nie zu einem leichten. Die meisten Angriffe suchen das leichte Ziel. Gute, einfache Sicherheit bewegt dich von leicht nach schwer.

## Ein bisschen Geschichte

**1970er–1980er: Sicherheit beginnt an der Außengrenze.** Frühe Computersicherheit konzentrierte sich darauf, Außenseiter draußen zu halten — Firewalls, Passwörter, abgeschlossene Serverräume. Das Modell war eine Burg: starke Mauern, alles drinnen ist sicher. Das funktionierte, bis Menschen sich verbinden und teilen mussten, was die Mauern riss.

**1990er: Die Außengrenze löst sich auf.** Das Internet und E-Mail bedeuteten, dass Daten sich zu bewegen begannen. Das Burgmodell brach. Viren und Eindringlinge kamen durch genau die Verbindungen, die Geschäfte möglich machten. Sicherheit musste den Daten folgen, nicht nur die Tür bewachen.

**2000er: „Least Privilege" und Verteidigung in die Tiefe.** Das Sicherheitsdenken wandte sich nach innen. Das Prinzip des **Least Privilege** (minimale Berechtigung) — gib jedem Nutzer und jedem Programm nur den Zugang, den es unbedingt braucht, keinen mehr — wurde zentral. Ebenso die **Verteidigung in die Tiefe**: viele überlappende Schichten, damit eine andere die Bedrohung auffängt, wenn eine versagt.

**2010er: „Von einem Einbruch ausgehen".** Experten erkannten, dass man Angreifer nicht immer draußen halten kann. Die neue Denkweise war, *anzunehmen*, dass ein Eindringling vielleicht schon drinnen ist, und sich darauf zu konzentrieren, was er erreichen kann zu begrenzen und ihn schnell zu erkennen. Protokollierung, Überwachung und schnelle Reaktion wurden genauso wichtig wie die Mauern.

**2020er: KI fügt eine neue Angriffsfläche hinzu.** KI bringt neue Wege, geschädigt zu werden — Tricks, die die KI selbst täuschen, Datenvergiftung und das Risiko, sensible Daten in Werkzeuge zu speisen, die du nicht kontrollierst. (Diese konkreten Bedrohungen behandelt [Kapitel 6](ch06-cybersecurity-in-the-ai-era.md).) Die alten Prinzipien — Least Privilege, Verteidigung in die Tiefe, von einem Einbruch ausgehen — gelten weiterhin, nun angewandt auf eine neue Art von Arbeitskraft.

Der Bogen: von einer Burg mit einer Mauer zu vielen Schichten, die annehmen, dass die Mauer durchbrochen werden kann. Die Lektion hat sich nie geändert: Schütze die Daten selbst, nicht nur die Tür.

## Neugier

### 20.7 Die Firma, die einen Angriff in einem Log fing, den niemand beobachtete

*Die konkrete Firma in dieser Geschichte ist illustrativ — ein realistisches Composite, keine genannte Firma. Das Muster dahinter ist real und gut dokumentiert.*

Stell dir eine mittelgroße Firma vor, die ein Protokollierungssystem hatte — eine Aufzeichnung von allem, was in ihrem Netzwerk geschah. Die Logs liefen ständig und zeichneten treu jeden Login, jede aufgerufene Datei, jede ungewöhnliche Anfrage auf. Monate lang las sie niemand. Sie waren da, wie eine Überwachungskamera, die niemand schaut.

Dann eines Tages sah ein neuer Techniker beim Aufräumen flüchtig in die Logs und bemerkte etwas Seltsames: Ein Programm meldete sich zu seltsamen Uhrzeiten nach außen, zog langsam und stetig Daten ab. Es tat das seit Wochen. Niemand hatte es bemerkt, weil niemand hinsah. Als sie schließlich hinsahen, fanden sie einen Eindringling, der weit länger still drinnen gewesen war, als jemand sich vorstellen konnte.

Die unbequeme Lektion ist nicht, dass die Firma nachlässig war. Sie ist, dass **der Beweis die ganze Zeit da war — und ignoriert wurde.** Die Firma hatte in die Kamera investiert, aber nicht ins Hinschauen.

Dieses Muster ist keine Fiktion. Der jährliche *Cost of a Data Breach*-Bericht von IBM hat Jahr für Jahr festgestellt, dass Datenpannen lange brauchen, um entdeckt zu werden — in den jüngsten Ausgaben im Bereich von **zweihundert Tagen** im Durchschnitt — und dass ein großer Anteil zuerst von jemandem außerhalb der Firma bemerkt wird, nicht vom eigenen Monitoring der Firma. Die Logs und Signale existieren oft. Was fehlt, ist ein Mensch, der sie ansieht.

Für deine KI-Automatisierungen ist die Lektion direkt: **Ein Log, den niemand liest, ist keine Sicherheit.** Wenn du Aufzeichnungen darüber sammelst, was deine KI tut, weise jemandem zu, tatsächlich hinzuschauen, und richte Alarme ein, damit die wichtigen Signale einen Menschen finden, statt darauf zu warten, entdeckt zu werden.

## Ein echtes Geschäftsbeispiel

*Das Folgende ist ein illustratives Composite häufiger realer Muster, keine einzelne genannte Firma.*

Ein kleiner Online-Händler wollte, dass KI Support-E-Mails an Kunden entwirft. Der einfache, riskante Weg war, der KI vollen Zugriff auf die gesamte Kundendatenbank zu geben — Namen, Adressen, Zahlungshistorie — und sie lesen zu lassen, was sie brauchte. Der Innehaber hielt inne und tat es stattdessen auf die sicherere Weise.

Sie gaben der KI **nur-Lese-Zugriff** auf genau die Bestelldetails, die sie brauchte, um eine Versandfrage zu beantworten — keine Zahlungsdatensätze, nicht die vollständige Kundendatei. Sie stellten es so ein, dass die KI entwerfen konnte, aber ein Mensch auf Senden drückte. Sie schalteten ein Protokoll ein, das jede Bestellung aufzeichnete, die die KI berührte. Sie sagten dem Support-Team, was die KI sehen konnte und was nicht, und baten sie, alles Seltsame zu melden.

Nach drei Wochen zeigte das Protokoll, dass die KI — von einem cleveren Kunden — gebeten worden war, die Adresse eines anderen Kunden preiszugeben, indem er sich als diese Person ausgab. Die KI hatte sich geweigert, weil ihr der Zugriff auf diese Daten von vornherein nicht gegeben war. Der Versuch scheiterte harmlos, und das Protokoll fing ihn ein, sodass das Team lernte, dass es diesen Trick gab.

Hätte der Inhaber den einfachen Weg genommen und der KI die ganze Datenbank gegeben, hätte derselbe Trick vielleicht funktioniert. Das sichere Design — minimaler Zugriff, ein Mensch beim Senden, ein beobachtetes Protokoll — verwandelte eine mögliche Datenpanne in ein Nicht-Ereignis. So sieht Security by Design in der Praxis aus.

## Wie man es macht

### 20.1 Security-by-Design-Prinzipien: wie man eine Automatisierung entwirft, die keine Daten preisgibt

Security by Design bedeutet, dass du Sicherheit von der ersten Skizze an in die Automatisierung einbaust. Stelle diese Fragen, bevor du irgendetwas baust:

- **Welche Daten braucht diese Automatisierung wirklich?** Nutze so wenig wie möglich. Wenn sie nur eine Bestellnummer braucht, gib ihr nicht die ganze Kundendatei.
- **Was ist das Schlimmste, das passieren kann, wenn sie leckt oder getäuscht wird?** Stell dir das Versagen vor. Gestalte so, dass der Worst Case klein ist.
- **Wohin gehen die Daten?** Kenne jedes System, das die Daten berühren, besonders außerhalb deiner Kontrolle. Speise keine sensiblen Daten in ein Werkzeug, für das du nicht einstehen kannst.
- **Kann ein Mensch sie stoppen?** Baue einen Not-Aus ein — einen Weg, die Automatisierung sofort abzuschalten, wenn sie sich falsch verhält.
- **Scheitert sie sicher?** Wenn etwas bricht, sollte die Automatisierung stoppen und schützen, nicht sich öffnen. Eine Tür, die verriegelt, wenn der Strom ausfällt, ist „fail-safe".

Das Kernprinzip ist **Least Privilege**: minimaler Zugriff, minimale Reichweite, minimale Daten. Eine Automatisierung, die nie Zugriff auf die sensiblen Daten hatte, kann sie nicht leaken, egal wie clever der Angriff ist. Designe den Zugriff heraus, und das Risiko geht mit ihm.

### 20.2 Zugriffskontrolle: wer was tun darf

Zugriffskontrolle bedeutet einfach zu entscheiden, wer was tun darf, und es durchzusetzen. Sie ist das Schloss in jedem Raum, nicht nur an der Haustür.

Drei klare Regeln:

- **Gib jeder Person und jedem Werkzeug nur den Zugriff, den seine Arbeit braucht.** Ein Support-Werkzeug, das Versandfragen beantwortet, braucht Bestelldaten, keine Abrechnungsdaten. Ein junior Mitarbeiter sollte nicht denselben Zugriff haben wie der Inhaber.
- **Trenne Zuständigkeiten.** Die Person, die die KI einrichtet, sollte nicht die einzige sein, die ihre Aktionen genehmigen kann, und die einzige, die die Logs sehen kann. Verteile die Schlüssel, damit kein einzelnes kompromittiertes Konto alles tun kann.
- **Prüfe den Zugriff, wenn sich Menschen ändern.** Wenn Mitarbeiter eintreten, wechseln oder gehen, aktualisiere ihren Zugriff am selben Tag. Alter Zugriff, der bestehen bleibt, ist eine der häufigsten Ursachen für Datenpannen.

Nutze die Werkzeuge, die deine Systeme schon haben — Benutzerrollen, Berechtigungen und Login-Kontrollen. Schalte **Zwei-Faktor-Authentifizierung** (ein zweiter Schritt über ein Passwort hinaus, wie ein Code auf dem Handy) ein, wo immer du kannst. Sie stoppt die meisten Angriffe mit gestohlenen Passwörtern.

### 20.3 Verschlüsselung: Daten auf dem Transport und im Ruhezustand schützen

**Verschlüsselung** bedeutet, Daten so zu verwürfeln, dass nur jemand mit dem richtigen Schlüssel sie lesen kann. Für einen Dieb sehen verschlüsselte Daten nach Unsinn aus. Sie schützt Daten in zwei Zuständen:

- **Auf dem Transport** — Daten, die zwischen Orten wandern, wie eine E-Mail oder ein Datei-Upload. Verschlüsselung hier bedeutet, dass ein Dieb, der das Kabel anzapft, Müll sieht. Achte auf „https" und sichere Verbindungen.
- **Im Ruhezustand** — Daten, die still liegen, wie Dateien auf einer Festplatte oder Datensätze in einer Datenbank. Verschlüsselung hier bedeutet, dass ein Dieb, der die Festplatte stiehlt, sie trotzdem nicht lesen kann.

Für ein kleines Unternehmen sind die praktischen Schritte einfach: nutze Werkzeuge, die standardmäßig verschlüsseln (die meisten seriösen Dienste tun das), prüfe, dass Verbindungen sicher sind (https), und frag jeden Anbieter direkt: „Sind meine Daten auf dem Transport und im Ruhezustand verschlüsselt?" Ein seriöser Anbieter antwortet ja und erklärt wie. Wenn er das nicht kann, ist das eine Warnung.

Eine Warnung: Verschlüsselung schützt Daten vor Außenseitern. Sie schützt nicht vor jemandem, der den Schlüssel hat und ihn missbraucht. Deshalb arbeiten Zugriffskontrolle (20.2) und Verschlüsselung zusammen — Verschlüsselung verbirgt die Daten, Zugriffskontrolle begrenzt, wer den Schlüssel hält.

### 20.4 Monitoring und Protokollierung: immer wissen, was die KI tut

Ein **Log** ist eine Aufzeichnung dessen, was geschah: wer was wann mit welchen Daten tat. **Monitoring** ist das Beobachten dieser Logs, live oder regelmäßig, um Ärger zu erkennen.

Warum das für KI wichtig ist: Eine KI-Automatisierung handelt den ganzen Tag mit deinen Daten. Ohne ein Protokoll kannst du nicht sagen, was sie berührt, was sie geändert hat oder ob sie getäuscht wurde. Mit einem Protokoll hast du eine Aufzeichnung, die du prüfen kannst, und eine Spur, die ein Angreifer nicht verbergen kann.

Mache die Protokollierung nützlich:

- **Protokolliere die wichtigen Aktionen** — welche Daten die KI las, was sie schrieb, was sie sandte, und jede Anfrage, die sie ablehnte.
- **Richte Alarme ein**, damit die wichtigen Signale einen Menschen finden. Lass niemanden auf einen Bildschirm starren; lass das System schreien, wenn etwas Ungewöhnliches geschieht.
- **Sieh tatsächlich hin.** Wie die Neugier-Geschichte zeigt, ist ein Log, den niemand liest, keine Sicherheit. Weise jemandem zu, regelmäßig zu prüfen, wenn auch nur kurz.
- **Halte die Logs sicher**, damit ein Eindringling sie nicht löschen kann.

Monitoring verwandelt ein stilles System in ein sichtbares. Du kannst nicht schützen, was du nicht sehen kannst.

### 20.5 Notfallpläne: was zu tun ist, wenn etwas schiefgeht

Irgendwann wird etwas schiefgehen. Die Frage ist nicht „ob", sondern „wann", und wie bereit du bist. Ein **Notfallplan** ist ein schriftlicher Plan für den schlechten Tag, gemacht an einem ruhigen Tag, damit du nicht in Panik improvisierst.

Ein einfacher Plan hat fünf Schritte:

1. **Erkennen.** Woran erkennst du, dass etwas nicht stimmt? (Ein Alarm, ein Mitarbeiterbericht, eine Kundenbeschwerde.)
2. **Eindämmen.** Wie stoppst du den Schaden jetzt sofort? (Automatisierung abschalten, Verbindung kappen, Konto sperren.)
3. **Bewerten.** Was wurde offengelegt oder geschädigt? Prüfe die Logs.
4. **Beheben und wiederherstellen.** Repariere die Ursache und stelle den normalen, sicheren Betrieb wieder her.
5. **Melden und lernen.** Sage den Menschen Bescheid, die es wissen müssen — und wisse, wen du gesetzlich informieren musst. (Datenschutzgesetze wie die DSGVO haben Meldepflichten; siehe [Kapitel 10](ch10-privacy-and-gdpr.md).) Dann schreibe auf, was geschah und wie man es beim nächsten Mal verhindert.

Schreibe den Plan auf eine Seite. Benenne, wer was tut. Halte Notfallkontakte bereit. Mache einmal im Jahr eine kurze Übung, damit jeder seinen Teil kennt. Ein eingeübter Plan verwandelt eine Krise in ein beherrschbares Ereignis.

### 20.6 Mitarbeiterschulung: der menschliche Faktor ist die erste Verteidigung

Das stärkste Schloss kann von einer einzigen nachlässigen Person geknackt werden. Deine Mitarbeiter sind sowohl dein größtes Risiko als auch deine beste Verteidigung. Schulung verwandelt sie vom schwachen Punkt zur ersten Linie.

Was zu lehren ist, in klaren Worten:

- **Tricks erkennen.** Angreifer täuschen Menschen mit gefälschten E-Mails, dringenden Bitten und „Ich bin von der IT, gib mir dein Passwort"-Anrufen. Bring den Mitarbeitern bei, sie zu erkennen und anzuzweifeln.
- **Sorgfältig mit Daten umgehen.** Wer was sehen darf, und warum. Gib Kundendaten niemals außerhalb genehmigter Kanäle weiter.
- **Melden, nicht verstecken.** Mache es sicher und erwartet, einen Fehler oder eine seltsame Anfrage zu melden. Ein Mitarbeiter, der früh eine verdächtige E-Mail meldet, rettet die Firma. Einer, der sie versteckt, lässt ein kleines Problem wachsen.
- **Die Grenzen der KI kennen.** Mitarbeiter sollen wissen, was die KI sehen kann und was nicht, und sie niemals bitten, etwas außerhalb ihrer sicheren Grenzen zu tun.
- **Passwort- und Login-Hygiene.** Starke Passwörter, Zwei-Faktor-Authentifizierung, kein Teilen von Logins.

Halte die Schulung kurz, regelmäßig und praktisch — nicht einen Vortrag einmal im Jahr. Eine monatliche Fünf-Minuten-Erinnerung und ein klarer Meldekanal bewirken mehr als ein langer Jahreskurs, an den sich niemand erinnert.

## Ethik und Verantwortung

Sicherheit ist eine ethische Pflicht, nicht nur eine technische.

**Schütze die Menschen, deren Daten du hältst.** Kunden, Mitarbeiter und Partner haben dir ihre Informationen anvertraut. Eine Datenpanne schädigt echte Menschen. Diese Daten sicher zu behandeln, ist eine Frage von Ehrlichkeit und Fürsorge.

**Melde ehrlich, wenn etwas schiefgeht.** Wenn du Kunden oder Aufsichtsbehörden informieren musst, tu es unverzüglich und wahrheitsgemäß. Eine Datenpanne zu vertuschen, ist schlimmer als die Panne selbst, ethisch und rechtlich.

**Nutze Sicherheit nicht als Ausrede, um dich zu verstecken.** „Wir sind sicher" darf nie bedeuten „ihr könnt nicht nachprüfen". Verantwortlichkeit und Transparenz gehören zusammen.

**Balanciere Sicherheit und Nutzbarkeit.** Sicherheit, die so schwer ist, dass niemand arbeiten kann, wird umgangen, und umgangene Sicherheit ist gar keine Sicherheit. Mache den sicheren Weg zum einfachen Weg.

**Schule mit Respekt, nicht mit Schuld.** Wenn jemand einen Fehler macht, lehre, bestrafe nicht. Eine Kultur der Schuld versteckt Fehler; eine Kultur des Lernens bringt sie früh ans Licht.

Sichere deine Daten so, wie du möchtest, dass deine eigenen geschützt werden.

## Zu vermeidende Fehler

**Zu viel Zugriff.** Der KI oder den Mitarbeitern mehr Zugriff geben als nötig. Nutze Least Privilege.

**Kein Mensch beim Senden.** Die KI allein auf kundengerichtete Nachrichten handeln lassen. Halte eine menschliche Prüfung bei.

**Sensible Daten in ungeprüfte Werkzeuge speisen.** Kundendaten in ein Werkzeug einfügen, für das du nicht einstehen kannst. Wisse, wohin Daten gehen.

**Ein Log, den niemand liest.** Aufzeichnungen sammeln und nie hinschauen. Weise jemanden zu und richte Alarme ein.

**Kein Notfallplan.** Am schlechten Tag improvisieren. Schreibe den Plan an einem ruhigen Tag.

**Logins teilen.** Ein Konto, das sich viele Personen teilen, zerstört Verantwortlichkeit. Gib jedem sein eigenes.

**Keine Zwei-Faktor-Authentifizierung.** Konten für gestohlene Passwörter offen lassen. Schalte 2FA überall ein.

**Personalwechsel ignorieren.** Alter Zugriff bleibt bestehen, nachdem jemand gegangen ist. Aktualisiere den Zugriff am Tag, an dem sich Rollen ändern.

**Beschuldigen statt schulen.** Fehler bestrafen, sodass Leute sie verstecken. Lehre und fördere das Melden.

**Annehmen, der Anbieter sei sicher.** Vertrauen ohne zu fragen. Frag Anbieter nach Verschlüsselung und Zugriff.

**Sicherheit als nachträglicher Einfall.** Erst die Automatisierung bauen und später an Sicherheit denken. Designe Sicherheit von Anfang an ein.

**Kein Not-Aus.** Kein Weg, die Automatisierung schnell zu stoppen, wenn sie sich falsch verhält. Baue den Aus-Schalter.

## Praktische Übung

### 20.8 Übung: Schreibe deinen KI-Sicherheitsplan

Schreibe einen einseitigen Sicherheitsplan für eine KI-Automatisierung, die du nutzt oder zu nutzen planst. Fülle jede Zeile.

**1. Die Automatisierung.** Benenne sie und welche Daten sie berührt.

**2. Minimaler Zugriff.** Liste genau, welche Daten sie braucht. Streiche alles andere. Schreibe den Zugriff auf, den du tatsächlich gewähren wirst.

**3. Menschliche Prüfung.** Wo ist der Mensch im Ablauf? Was kann die KI allein, und was braucht eine Person zur Genehmigung?

**4. Datenort.** Wohin gehen die Daten? Liste jedes System, besonders außerhalb deiner Kontrolle. Notiere jedes, für das du nicht einstehen kannst, und entferne es.

**5. Verschlüsselung.** Sind die Daten auf dem Transport und im Ruhezustand verschlüsselt? Prüfe es bei jedem Anbieter und schreibe die Antwort.

**6. Zugriffskontrolle.** Wer kann was? Liste Rollen. Notiere, wo du Zwei-Faktor-Authentifizierung einschalten wirst.

**7. Protokollierung.** Was wirst du protokollieren? Wer wird schauen, und wie oft? Was wird einen Alarm auslösen?

**8. Not-Aus.** Wie schaltest du sie sofort aus? Schreibe die genauen Schritte.

**9. Notfallplan.** Schreibe die fünf Schritte — erkennen, eindämmen, bewerten, beheben, melden — mit Namen dafür, wer jedes tut. Notiere jede gesetzliche Meldepflicht (siehe [Kapitel 10](ch10-privacy-and-gdpr.md)).

**10. Mitarbeiterschulung.** Was wirst du dem Team über diese Automatisierung beibringen, und wie werden sie ein Problem melden?

Setze es auf eine Seite. Teile es mit den beteiligten Personen. Halte es dort, wo du es am schlechten Tag finden kannst. Ein Plan, den du an einem ruhigen Tag geschrieben hast, ist zehnmal so viel wert wie ein Plan, den du in einer Krise erfindest.

## Checkliste

### 20.9 Checkliste: die 15 Sicherheitsfragen

Bevor du eine KI-Automatisierung echte Daten berühren lässt, beantworte diese fünfzehn Fragen. Jede einzelne muss ein klares „Ja" sein.

- [ ] **1. Minimaler Zugriff:** Hat die Automatisierung nur die Daten, die sie wirklich braucht, und nichts weiter?
- [ ] **2. Mensch beim Senden:** Prüft ein Mensch alles, was einen Kunden erreicht?
- [ ] **3. Datenort:** Kenne ich jedes System, das die Daten berührt, einschließlich außerhalb meiner Kontrolle?
- [ ] **4. Geprüfte Werkzeuge:** Habe ich abgelehnt, sensible Daten in ein Werkzeug zu speisen, für das ich nicht einstehen kann?
- [ ] **5. Auf dem Transport verschlüsselt:** Sind Daten beim Wandern zwischen Systemen verschlüsselt?
- [ ] **6. Im Ruhezustand verschlüsselt:** Sind Daten beim Speichern verschlüsselt?
- [ ] **7. Einzelne Logins:** Hat jede Person ihren eigenen Login, ohne Teilen?
- [ ] **8. Zwei-Faktor-Authentifizierung:** Ist 2FA für die wichtigen Konten eingeschaltet?
- [ ] **9. Getrennte Zuständigkeiten:** Sind Einrichtung, Genehmigung und Log-Prüfung auf mehrere Personen verteilt?
- [ ] **10. Zugriffsprüfung:** Aktualisiere ich den Zugriff am Tag, an dem Mitarbeiter eintreten, wechseln oder gehen?
- [ ] **11. Protokollierung:** Erfasse ich, was die KI liest, schreibt, sendet und ablehnt?
- [ ] **12. Beobachtete Logs:** Prüft jemand tatsächlich die Logs, mit Alarmen für die wichtigen Signale?
- [ ] **13. Not-Aus:** Kann ich die Automatisierung sofort ausschalten, und weiß ich wie?
- [ ] **14. Notfallplan:** Habe ich einen schriftlichen, benannten Plan zum Erkennen, Eindämmen, Bewerten, Beheben und Melden?
- [ ] **15. Geschulte Mitarbeiter:** Wurde das Team gelehrt, Tricks zu erkennen und Probleme sicher zu melden?

Wenn eine Antwort „Nein" ist, ist die Automatisierung nicht bereit. Behebe es, bevor du live gehst. Sicherheit ist kein Produkt, das man einmal kauft; sie ist fünfzehn Fragen, die man immer wieder mit Ja beantwortet.

## Wichtige Kernpunkte

- Security by Design bedeutet, Sicherheit von Anfang an einzubauen — minimaler Zugriff, ein Mensch beim Senden und ein Not-Aus —, damit der Worst Case klein bleibt.
- Ein Log, den niemand liest, ist keine Sicherheit: sammle Aufzeichnungen, richte Alarme ein und weise jemandem zu, tatsächlich hinzuschauen.
- Verschlüsselung verbirgt Daten vor Außenseitern (auf dem Transport und im Ruhezustand), während Zugriffskontrolle begrenzt, wer den Schlüssel hält — du brauchst beide zusammenarbeitend.
- Schreibe deinen Notfallplan an einem ruhigen Tag: erkennen, eindämmen, bewerten, beheben, melden, lernen — mit Namen an jedem Schritt.
- Der menschliche Faktor ist die erste Verteidigung: schule Mitarbeiter, Tricks zu erkennen und sicher zu melden, und mache den sicheren Weg zum einfachen Weg.
