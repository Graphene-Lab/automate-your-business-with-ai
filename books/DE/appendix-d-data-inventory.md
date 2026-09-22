# Anhang D — Dateninventar

Du kannst keine Daten schützen, die du nicht findest. Dieses Inventar listet jedes wichtige Datenelement auf, das dein Unternehmen besitzt, wo es liegt und wer es erreichen kann. Fülle es aus, bevor du ein KI-Werkzeug anschließt. Wenn ein Datum nicht auf dieser Liste steht, gib es nicht an die KI.

## So benutzt du es

1. Gehe deine Werkzeuge durch: E-Mail, Laufwerke, Buchhaltung, CRM, HR-Systeme, Tabellenkalkulationen.
2. Füge eine Zeile pro Datenelement hinzu (eine Kundenliste, eine Gehaltsdatei, ein Vertragsordner).
3. Markiere jedes Element als **Personenbezogen** (bezieht sich auf eine Person) oder **Sensibel** (besondere Kategorien — siehe unten).
4. Prüfe den Zugriff: Wer kann es heute öffnen, und wer *sollte* es können?
5. Prüfe vor jedem KI-Projekt. Diese Liste sagt dir, was sicher zu benutzen ist und was nicht.

## Leere Vorlage

| Datenelement | Wo gespeichert | Eigentümer | Personenbezogen / Sensibel? | Wer hat Zugriff | Backup-Status | Aufbewahrung |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Ausgefülltes Beispiel

| Datenelement | Wo gespeichert | Eigentümer | Personenbezogen / Sensibel? | Wer hat Zugriff | Backup-Status | Aufbewahrung |
|---|---|---|---|---|---|---|
| Kunden-Kontaktliste | CRM (Cloud) | Verkaufsleiter | Personenbezogen (Namen, E-Mails, Telefon) | Vertriebsteam (bearbeiten), Finanzen (lesen) | Täglich, extern | Während der Aktivität + 3 Jahre |
| Gehaltsdatei | Gemeinsames Laufwerk, Ordner „HR" | HR-Leitung | Sensibel (Gehalt, Ausweis, Bank) | Nur HR | Wöchentlich, extern | 10 Jahre (gesetzlich) |
| Lieferantenverträge | Papierschrank + gescannter Ordner | Inhaber | Weder (geschäftsvertraulich) | Inhaber, Finanzen | Teilweise (nur Scans) | Laufzeit des Vertrags + 6 Jahre |

## Wo du nach Daten suchen solltest

Gehe jeden dieser Punkte durch. Daten verstecken sich offen sichtbar:

- [ ] Gemeinsame E-Mail-Postfächer und persönliche Mailfächer.
- [ ] Gemeinsame Laufwerke und Netzwerkordner.
- [ ] Cloud-Werkzeuge: CRM, Buchhaltung, HR, Projekt-Tools.
- [ ] Tabellenkalkulationen und Anhänge (oft das Chaotischste).
- [ ] Papierakten, Schränke und gescannte Kopien.
- [ ] Backups und alte Exporte.
- [ ] Chat-Werkzeuge und Nachrichtenhistorie.
- [ ] Handys und Laptops der Mitarbeiter.
- [ ] Drittanbieter-Tools, die Mitarbeiter selbst installiert haben (Schattenkopien).

## Was gilt als „sensibel"

Nach der DSGVO brauchen diese besonderen Kategorien besondere Sorgfalt. Markiere sie klar:

- Gesundheitsdaten
- Rassische oder ethnische Herkunft
- Politische Meinungen
- Religiöse oder weltanschauliche Überzeugungen
- Gewerkschaftszugehörigkeit
- Genetische und biometrische Daten (zur Identifizierung)
- Sexualleben oder sexuelle Orientierung

Behandle auch Folgendes als sensibel, auch wenn es keine „besondere Kategorie" ist: Bankdaten, Ausweisnummern, Passwörter, Daten von Kindern und alles, was einer Person schaden könnte, wenn es durchsickert.

## Spaltenanleitung

- **Datenelement** — Ein einfacher Name für die Sache (nicht der Dateiname).
- **Wo gespeichert** — System und Ort: Cloud-Werkzeug, Laufwerkpfad, Papierschrank.
- **Eigentümer** — Eine Person, die dafür verantwortlich ist.
- **Personenbezogen / Sensibel?** — Personenbezogen, Sensibel oder Weder.
- **Wer hat Zugriff** — Rollen oder Personen, und ob sie lesen oder bearbeiten können.
- **Backup-Status** — Wie oft es gesichert wird und wo. Vermerke, wenn es **kein** Backup gibt.
- **Aufbewahrung** — Wie lange du es aufbewahrst und warum (gesetzliche Regel oder geschäftliches Bedürfnis).

## Warnsignale, die du jetzt beheben solltest

- [ ] Sensible Daten ohne Eigentümer.
- [ ] Sensible Daten, die jeder in der Firma öffnen kann.
- [ ] Wichtige Daten ohne Backup.
- [ ] Daten, die „für immer" ohne Grund aufbewahrt werden.
- [ ] Personenbezogene Daten in einem Werkzeug, das du nicht kontrollierst (Shadow AI, private E-Mail).
- [ ] Dieselben Daten an vielen Orten ohne Masterkopie.

## Faustregeln zur Aufbewahrung

- Hebe Daten nur so lange auf, wie du sie brauchst. Länger ist nicht sicherer — es ist mehr Risiko.
- Prüfe die gesetzlichen Mindestfristen: Steuer- und Gehaltsunterlagen haben oft feste Jahre. Frage deinen Steuerberater.
- Bei Kundendaten: hebe sie, solange die Beziehung aktiv ist, dann einen kurzen, festgelegten Zeitraum.
- Lösche oder anonymisiere Daten, die du nicht mehr brauchst. Lass sie sich nicht ansammeln.
- Schreibe den Grund für jede Aufbewahrungsfrist auf, damit später niemand raten muss.

## Das Inventar aktuell halten

- Prüfe es alle 6 Monate und vor jedem neuen KI-Projekt.
- Füge am Tag, an dem ein neues Werkzeug oder eine neue Datenquelle auftaucht, eine Zeile hinzu.
- Benenne pro Element einen Eigentümer; Eigentümer halten es ehrlich.
- Behandle es als lebendiges Dokument, nicht als einmalige Pflichtübung.

## Regel für KI-Projekte

Bevor Daten in ein KI-Werkzeug gehen, prüfe dieses Inventar. Wenn ein Element **sensibel** ist, brauchst du einen klaren Grund, ein sicheres Werkzeug und oft eine DSFA. Im Zweifel lass es weg.
