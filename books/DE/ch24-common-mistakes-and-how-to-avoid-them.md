# Kapitel 24 — Häufige Fehler und wie du sie vermeidest

## In einfachen Worten

Die meisten KI-Projekte scheitern aus denselben wenigen Gründen. Nicht weil die Technik schwach ist, sondern wegen vorhersehbarer Fehler, die Menschen immer wieder machen. Die gute Nachricht: Wenn du die Fehler kennst, kannst du fast alle vermeiden. Dieses Kapitel ist ein geführter Rundgang durch die großen Fehler, mit der Behebung für jeden.

Sieh es als eine Liste von Landminen. Jede ist leicht zu betreten, wenn du nicht weißt, dass sie da ist, und leicht zu umgehen, wenn du es weißt. Das Ziel ist nicht, dich von der KI abzuschrecken. Es ist, dich zu der Art Unternehmer zu machen, der das eigene Projekt nicht aus Versehen in die Luft jagt.

Die sechs großen Fehler sind: den falschen Prozess automatisieren, Daten und Menschen unterschätzen, der KI zu sehr vertrauen, zu groß anfangen, Vorschriften und Sicherheit ignorieren und Ergebnisse nicht messen. Jeder ist häufig, jeder ist kostspielig, und jeder hat einen klaren Weg zur Vermeidung. Wir nehmen sie einzeln, erklären, warum er passiert und was er kostet, und verweisen auf das Kapitel, das die Behebung vollständig behandelt.

Ein einfaches Bild zum Mitnehmen: KI einzuführen ist wie ein langer Fußweg durchs offene Land. Die meisten scheitern nicht, weil der Weg unmöglich ist. Sie scheitern, weil sie das falsche Ziel gewählt, zu wenig Wasser eingepackt, einer fehlerhaften Karte vertraut, am ersten Tag zu weit gehen wollten, das Wetter ignoriert und nie geprüft haben, ob sie in die richtige Richtung laufen. Die Fehler sind alltäglich und vermeidbar. Dieses Kapitel ist die Sicherheitsunterweisung vor dem Aufbruch.

Lies es als Checkliste gegen deine eigenen Pläne. Wenn du dich dabei ertappst, etwas davon zu tun, halt an und behebe es, bevor du mehr Geld ausgibst oder mehr Vertrauen verbrennst.

## Ein wenig Geschichte

**1980er: Der Zusammenbruch der Expertensysteme lehrte die Lehre vom falschen Prozess.** Während des Expertensystem-Booms pumpten Unternehmen Geld in die Kodierung der Regeln menschlicher Experten. Viele Projekte scheiterten, weil sie versuchten, Aufgaben zu automatisieren, die zu chaotisch, zu selten oder zu sehr vom Urteil abhängig waren, um sie zu kodieren. Die Systeme waren spröde und teuer zu aktualisieren, und der Markt brach zusammen. Die Lehre: Das Falsche zu automatisieren, vernichtet ein Vermögen, egal wie gut die Technik ist.

**1990er: „Müll rein, Müll raus" wurde ein Mantra.** Als Unternehmen computergestützt arbeiteten, lernten sie, dass ein System, das mit schlechten Daten gefüttert wird, schlechte Ergebnisse liefert, egal wie klug die Software ist. Diese alte Rechner-Weisheit wurde zum Kern jedes Datenprojekts. Sie ist die Vorfahrin des heutigen Fehlers „Daten unterschätzen".

**1990er–2000er: das Big-Bang-Scheitermuster.** Enterprise-Softwareprojekte der 1990er und 2000er waren berühmt dafür, „Big Bang" zu gehen — alles auf einmal ersetzen, nach einem großen Plan, über Jahre. Viele liefen über Budget, über Zeit und scheitern offen. Das Muster war so häufig, dass „Big-Bang-Einführung" ein warnender Begriff wurde. Die daraus entstandene Behebung: klein anfangen, Wert beweisen, dann wachsen. Das ist die Vorfahrin von „zu groß anfangen".

**2000er: Automations-Nachsichtigkeit.** Forscher, die automatisierte Systeme untersuchten — Autopiloten, automatische Überwachung —, fanden einen überraschenden Fehler: Wenn ein System meist gut funktioniert, hören Menschen auf, Acht zu geben, und vertrauen ihm zu sehr. Dann versagt es bei einem seltenen Fall, und niemand fängt es auf. Das heißt **Automations-Nachsichtigkeit** oder **Automations-Bias**, und es ist genau der Fehler „der KI zu sehr vertrauen". Er wurde lange vor Chatbots dokumentiert und ist heute relevanter denn je.

**2010er: Die Regulierung holt auf.** Als Datenlecks und Missbrauch Schlagzeilen machten, begannen Regierungen, strenge Regeln zu schreiben — die DSGVO in Europa die größte. Unternehmen, die lax mit Daten umgegangen waren, sahen sich mit hohen Bußgeldern und Rechtsrisiko konfrontiert. Die Lehre: Die Regeln zu ignorieren ist keine Abkürzung; es ist eine Belastung, die nur darauf wartet, ausgelöst zu werden.

**2020er: dieselben alten Fehler, neue Technik.** Die aktuelle KI-Welle wiederholt jeden einzelnen dieser Fehler in rasendem Tempo. Billige, beeindruckende Tools machen es leicht, groß zu starten, zu sehr zu vertrauen, die Datenarbeit auszulassen, die Regeln zu ignorieren und das Messen zu überspringen. Die Technik ist neu; die Fehlermuster sind alt und gut dokumentiert. Die Geschichte zu kennen ist die billigste Verteidigung, die es gibt.

Der Bogen: Jede Generation von Geschäftstechnik hat dieselben wenigen Fehler gemacht. Keiner davon ist neu. Alle sind vermeidbar, wenn du sie schon einmal gesehen hast.

## Neugier

### 24.7 Der Eliza-Effekt: warum wir Maschinen mehr vertrauen, als sie verdienen

Ein Grund, warum Menschen KI zu sehr vertrauen, geht auf ein Chat-Programm von 1966 namens ELIZA zurück und die nach ihm benannte menschliche Gewohnheit — den **Eliza-Effekt**: Wir gewähren einer Maschine bereitwillig Verständnis und Gefühle, die sie nur nachahmt, und vertrauen ihrer Ausgabe mehr, als sie verdient.

Die ganze Geschichte von ELIZA und warum sie für die Art, wie du jedes KI-Tool gestaltest und beaufsichtigst, wichtig ist, wird in [Kapitel 1 — Eine kurze Geschichte der KI](ch01-a-short-history-of-ai.md) erzählt, der eigentlichen Heimat des Eliza-Effekts. Der Einzeiler-Verweis hier: Eine flüssige, höfliche Maschine lässt uns sie übermäßig vertrauen, und diese Gewohnheit ist die Wurzel von Fehler 24.3 unten.

## Ein echtes Geschäftsbeispiel

*Das Folgende ist eine veranschaulichende Zusammenstellung häufiger realer Muster, kein einzelnes namentlich genanntes Unternehmen.*

Ein Einzelhandelsunternehmen wollte „KI nutzen", also machte es fast alles auf dieser Liste falsch — und dann fast alles richtig.

Die falsche Version: Der Inhaber las über KI, geriet in Begeisterung und beschloss, „den Kundenservice zu transformieren". Ohne ein bestimmtes Problem zu wählen, kaufte er einen Chatbot und rollte ihn auf den ganzen Kundenstamm auf einmal aus. Er fütterte ihn mit einem Haufen alter, chaotischer Dokumente und hoffte das Beste. Er schaltete die menschliche Prüfung aus, weil „die KI schneller ist". Er prüfte nie, ob sie richtige Antworten gab. Innerhalb von Wochen teilte der Chatbot Kunden selbstbewusst falsche Rückgaberegeln und falsche Preise mit. Kunden beschwerten sich. Das Unternehmen merkte nichts, bis sich die Beschwerden auftürmten. Das Projekt war ein Chaos, und der Inhaber schloss: „KI funktioniert nicht."

Die richtige Version: Nach dem Chaos startete der Inhaber mit Disziplin neu. Er wählte ein kleines, klares Problem — die zehn häufigsten „Wo ist meine Bestellung?"-Fragen beantworten, die Arbeitszeit fraßen. Er prüfte zuerst die Daten und fand heraus, dass er saubere Sendungsverfolgungs-Daten hatte, die diese Fragen zuverlässig beantworten konnten. Er begann mit einem winzigen Pilot nur auf diesen Fragen, mit einem Menschen, der jede Antwort prüfte. Er maß das Ergebnis: Die Antwortzeit sank, die Zufriedenheit hielt, und die Antworten waren richtig, weil die Daten gut und der Umfang eng waren. Erst dann weitete er sich aus, Schritt für Schritt, und behielt die menschliche Prüfung bei den schwereren Fällen.

Die Technik war dieselbe. Der erste Versuch scheiterte an sechs Fehlern. Der zweite funktionierte, weil jeder Fehler vermieden wurde. Die Lehre ist nicht „KI ist riskant". Die Lehre ist „die Fehler sind das Risiko, und sie sind vermeidbar".

## So machst du es

### 24.1 Den falschen Prozess automatisieren

Der teuerste Fehler ist, Geld auszugeben, um etwas zu automatisieren, das nie das Automatisieren wert war. Ein schneller falscher Prozess ist immer noch falsch, und jetzt ist er falsch im großen Maßstab.

**Warum er passiert.** Begeisterung. Du hast ein Tool und willst es benutzen, also richtest du es auf irgendetwas vor dir, statt sorgfältig zu wählen. Oder du automatisierst einen Prozess, der schon in Ordnung ist, und sparst Zeit, die niemand sparen musste, während der echte Engpass unangetastet bleibt.

**Was er kostet.** Geld für ein Tool, das wenig liefert, plus die Opportunitätskosten des echten Problems, das du nicht gelöst hast. Schlimmer noch: Eine schlecht gewählte Automatisierung kann die Dinge verschlimmern — einen kaputten Prozess zu automatisieren erzeugt nur schneller kaputte Ausgabe und verbirgt den Bruch.

**Die Behebung: wählen, bevor du kaufst.** Wähle vor jedem Tool den Prozess nach zwei Tests. Erstens *Wirkung*: Ist dieser Prozess wirklich wichtig? Kostet er echte Zeit, echtes Geld oder echte Kundenzufriedenheit? Zweitens *Eignung*: Ist der Prozess für Automatisierung geeignet — wiederholend, regel- oder beispielbasiert, mit verfügbaren Daten? Die Wirkung-gegen-Mühelosigkeit-Matrix in [Kapitel 12 — Wo KI deinem Unternehmen helfen kann](ch12-where-ai-can-help-your-business.md) ist das Werkzeug dafür. Benutz es. Wähle das Ziel mit hoher Wirkung und hoher Eignung, nicht das Erste, was dir einfällt.

**Behebe den Prozess, bevor du ihn automatisierst.** Wenn ein Prozess kaputt ist, repariere ihn zuerst und automatisiere dann die reparierte Version. Ein Chaos zu automatisieren gibt dir ein automatisiertes Chaos. Manchmal ist der beste erste Schritt, einen Schritt zu vereinfachen oder ganz zu entfernen, statt ihn zu automatisieren.

### 24.2 Daten und Menschen unterschätzen

KI läuft auf zwei Dingen: Daten und Menschen. Beide sind meist schwieriger und wichtiger als das Modell selbst, und beide werden routinemäßig unterschätzt.

**Der Daten-Fehler.** KI ist nur so gut wie die Daten, mit denen du sie fütterst. Chaotische, unvollständige, veraltete oder voreingenommene Daten erzeugen chaotische, unvollständige, veraltete oder voreingenommene Ausgabe — egal wie gut das Tool. Menschen stellen sich vor, die KI werde es aus dem, was sie haben, „schon herausfinden". Kann sie nicht. Wenn deine Unterlagen ein Chaos sind, erbt die KI das Chaos. Die vollständige Behandlung der Datenqualität ist in [Kapitel 14 — Daten: Der Rohstoff](ch14-data-the-raw-material.md). Die Kurzfassung: Prüfe deine Daten, bevor du gute Ausgabe erwartest, und behebe die Daten, bevor du die KI beschuldigst.

**Der Menschen-Fehler.** Wie Kapitel 15 zeigt, kann ein Tool, das in einem Test funktioniert, ungenutzt herumliegen, weil niemand wusste, warum es existiert, niemand geschult wurde und niemand sich sicher fühlte. Menschen sind kein Nebensatz; sie sind der Grund, warum Projekte leben oder sterben. Die menschliche Seite zu unterschätzen — die Schulung, die Angst, das Vertrauen, das Änderungsmanagement — ist eine der häufigsten Ursachen für Scheitern. Die Fähigkeiten zum Änderungsmanagement sind in [Kapitel 21](ch21-managing-change-in-your-company.md). Plane für die menschliche Arbeit so ernsthaft Budget ein wie für die Software.

**Warum er passiert.** Sowohl Daten- als auch Menschenarbeit sind langsam, unglamourös und langweilig im Vergleich zum aufregenden Tool. Es ist verlockend, sie auszulassen und zur Demo zu kommen. Aber sie auszulassen heißt, das Fundament auszulassen. Das Gebäude stürzt ein.

**Die Behebung.** Behandle Daten und Menschen als das Hauptprojekt, mit dem Tool als einem Teil davon, nicht umgekehrt. Verwende echte Zeit aufs Reinigen und Prüfen der Daten. Verwende echte Zeit fürs Schulen, Kommunizieren und Unterstützen der Menschen. Das ist nicht Überkopf; das ist die Arbeit.

### 24.3 Der KI zu sehr vertrauen

Moderne KI erzeugt flüssige, selbstbewusste, gut geschriebene Ausgabe. Diese Flüssigkeit bringt uns dazu, ihr mehr zu vertrauen, als sie verdient. Das ist Automations-Bias, und er ist der gefährlichste Fehler in der Liste, weil er ein Tool in einen unbeaufsichtigten Entscheider verwandelt.

**Warum er passiert.** Eine selbstbewusste, gut geschriebene Antwort *fühlt* sich richtig an. Unser Gehirn verwechselt „klingt gut" mit „ist wahr". Kommt der Eliza-Effekt dazu — unsere Gewohnheit, einer höflichen Maschine Verständnis zuzugestehen —, ist es leicht, das Prüfen einzustellen. Wenn das Tool zu 95 % recht hat, rutschen die 5 %, in denen es falsch liegt, durch, weil niemand zusieht.

**Was er kostet.** Falsche Antworten, die Kunden erreichen. Falsche Zahlen in Berichten. Falsche Entscheidungen auf selbstbewusster, aber falscher Ausgabe. Der Schaden ist gerade deshalb größer, weil die Ausgabe vertrauenswürdig aussah, sodass niemand sie hinterfragte, bis es zu spät war. Erinnere dich an die Lehre aus Kapitel 1: Flüssigkeit ist nicht Wahrheit.

**Die Behebung: behalte den Menschen im Loop.** Lass niemals KI-Ausgabe ungeprüft hinausgehen, besonders nicht zu Kunden oder in wichtige Entscheidungen. Setze eine feste Regel: Die KI entwirft, ein Mensch prüft und sendet. Bring den Menschen *bei, wie* man prüft — worauf zu achten ist, wie eine falsche Antwort aussieht —, nicht nur, einen Knopf zu drücken. Die Prüffähigkeit ist wichtiger als das Tool.

**Hüte dich vor selbstbewusstem Unsinn.** KI kann selbstbewusst falsch liegen. Je selbstbewusster und flüssiger die Ausgabe, desto sorgfältiger solltest du sie prüfen, nicht weniger. Schulde deinen Instinkt, bei wichtigen Dingen glatten Antworten misstrauisch zu begegnen. Die misstrauische Denkweise in [Kapitel 7 — Trustless: Vertrauen ohne zu vertrauen](ch07-trustless-trust-without-trusting.md) ist der richtige Rahmen: verifizieren, nicht standardmäßig vertrauen.

**Setze Eskalationsregeln.** Entscheide, was die KI allein darf und was zu einem Menschen muss. Riskante, ungewöhnliche oder mehrdeutige Fälle gehen an eine Person. Die KI erledigt das Routine; der Mensch das Wichtige und das Seltsame.

### 24.4 Zu groß anfangen

Der Big-Bang-Rollout — alles auf einmal ändern nach einem großen Plan — ist ein klassisches Scheitern. Er ist verlockend, weil er sich ambitioniert anfühlt, aber er ist der sicherste Weg, die Kontrolle zu verlieren.

**Warum er passiert.** Ehrgeiz und Ungeduld. Du willst die große Transformation jetzt, also gehst du breit und schnell vor. Oder du willst beeindrucken, also wählst du den großartigsten möglichen Umfang. Groß fühlt sich kühn an; in der Praxis ist es fragil.

**Was er kostet.** Große Projekte sind schwer zu kontrollieren, teuer zu beheben, wenn sie schiefgehen, und langsam darin, Wert zu zeigen. Ein Mangel, der im Pilot klein wäre, wird zur Krise, wenn er über die ganze Firma multipliziert wird, bevor du ihn siehst. Big-Bang-Projekte laufen oft über Budget und über Zeit, und viele scheitern offen.

**Die Behebung: klein anfangen und Wert beweisen.** Wähle eine enge Aufgabe, ein Team, ein klares Ziel. Fahre einen Pilot. Miss ihn. Wenn er funktioniert, skaliere in Schritten (Kapitel 23). Klein ist nicht ängstlich; klein ist, wie du billig lernst und die Kontrolle behältst. Jeder kleine Erfolg baut die Fähigkeit und den Beleg für den nächsten Schritt auf. Der Weg der engen Siege ist derselbe, den Kapitel 1 aus der Geschichte empfiehlt: KI gewinnt ein bestimmtes Ding nach dem anderen, und du auch.

**Ehrgeiz ist gut; Reihenfolge ist die Disziplin.** Du kannst eine große Vision haben. Erreiche sie nur über eine Kette kleiner, bewiesener Schritte, nicht über einen einzigen Riesensprung. Das Ziel kann groß sein; der erste Schritt muss klein sein.

### 24.5 Vorschriften und Sicherheit ignorieren

KI berührt deine Daten, die Daten deiner Kunden und deine Entscheidungen. Das heißt, sie berührt das Gesetz und deine Sicherheit. Beides zu ignorieren ist keine Abkürzung; es ist eine geladene Belastung.

**Warum er passiert.** Vorschriften und Sicherheit fühlen sich langsam, komplex und weit weg an — bis sie es nicht mehr sind. Es ist verlockend, schnell voranzugehen und Compliance „später" zu erledigen. Später kommt oft als Bußgeld, Leck oder Rechtsstreit.

**Was er kostet.** Hohe Bußgelder für Verstöße gegen Datenschutzregeln. Ein Datenleck, das Kundeninformationen freilegt und Vertrauen zerstört. Rechtliche Haftung für Entscheidungen, die die KI traf und die eine Regel brachen. Die Kosten des Ignorierens sind weit größer als die Kosten der ordentlichen Behandlung, und sie treffen auf einmal ein.

**Die Behebung: kenne die Regeln, die für dich gelten.** Wenn du personenbezogene Daten in oder über Europa verarbeitest, gilt die DSGVO — behandelt in [Kapitel 10 — Privatsphäre und DSGVO](ch10-privacy-and-gdpr.md). Fällt deine KI-Nutzung unter den EU AI Act, gelten dessen Pflichten — behandelt in [Kapitel 5 — Regeln und rechtliche Verantwortung](ch05-rules-and-legal-responsibility.md). Du musst kein Anwalt sein, aber du musst wissen, welche Regeln dich betreffen, und sie befolgen. Hole dir Rat, wo es zählt.

**Nimm Sicherheit vom ersten Tag an ernst.** KI-Tools verarbeiten oft sensible Daten. Behandle diese Daten mit derselben Sorgfalt, die du Bargeld im Safe entgegenbringst. Die Sicherheitsbedrohungen, die spezifisch für das KI-Zeitalter sind — Datenlecks, Prompt-Injection, Anbieter-Exposition —, sind in [Kapitel 6 — Cybersicherheit im KI-Zeitalter](ch06-cybersecurity-in-the-ai-era.md) behandelt. Schraube Sicherheit nicht später an; bau sie von Anfang an ein.

**Compliance ist nicht optional und keine Ziellinie.** Regeln ändern sich, und deine Nutzung von KI ändert sich. Compliance ist laufend, wie Wartung. Bau sie in deine Arbeitsweise ein, nicht in eine einmalige Prüfung, die du überspringst.

### 24.6 Ergebnisse nicht messen

Wenn du nicht misst, kannst du nicht sagen, ob die KI geholfen, geschadet oder nichts getan hat. Du fährst blind, und du wirst weiter Geld für etwas ausgeben, das du nicht bewerten kannst.

**Warum er passiert.** Messen fühlt sich wie Extrarbeit an, und es kann schlechte Nachrichten zeigen. Es ist leichter anzunehmen, dass es funktioniert, als nachzuprüfen. Viele Projekte starten mit Begeisterung und schauen nie wieder auf eine Zahl.

**Was er kostet.** Du kannst keinen Wert beweisen, also kannst du keine guten Entscheidungen übers Expandieren oder Stoppen treffen. Du gibst weiter Geld für Dinge aus, die vielleicht nicht funktionieren. Du verpasst die Lehre, die das nächste Projekt besser machen würde. Ein Projekt, das du nie gemessen hast, ist ein Projekt, dessen Ausgang zufällig war.

**Die Behebung: von Anfang an messen.** Setze einen Ausgangswert vor dem Start, verfolge ein paar ehrliche KPIs und prüfe sie regelmäßig. Die volle Methode ist in [Kapitel 16 — Ziele, Kosten und Kapitalrendite](ch16-goals-costs-and-return-on-investment.md), und die Dashboard-Praxis ist in [Kapitel 22 — Ergebnisse und ROI messen](ch22-measuring-results-and-roi.md). Lerne sie hier nicht neu; verpflichte dich einfach dazu. Miss die Wahrheit, inklusive der schlechten Wochen, und nutze sie, um Behalten, Korrigieren oder Stoppen zu entscheiden.

**Miss die Dinge, die zählen, nicht die, die schmeicheln.** Vermeide Eitelkeits-Metriken wie Nutzungszahlen. Miss Zeit, Fehler, Kosten und Zufriedenheit. Eine Zahl, die nur die gute Seite zeigt, ist eine Zahl, die dich anlügt.

## Ethik und Verantwortung

Jeder Fehler auf dieser Liste hat eine ethische Seite, weil jeder echte Menschen verletzen kann — Kunden, Mitarbeitende oder das Unternehmen selbst.

**Der KI zu sehr zu vertrauen ist ein ethisches Versagen, nicht nur ein praktisches.** Wenn ungeprüfte KI-Ausgabe einen Kunden erreicht und falsch ist, hast du jemandem geschadet. Du bleibst verantwortlich für das, was deine KI hinausschickt, egal wie selbstbewusst es klang. Den Menschen im Loop zu behalten ist eine Pflicht, keine Vorliebe.

**Vorschriften zu ignorieren ist eine Pflicht, die du Menschen schuldest, kein anzukreuzendes Kästchen.** Datenschutzregeln existieren, um echte Menscheninformationen zu schützen. Ihnen zu folgen heißt, diese Menschen zu respektieren, nicht ein Bußgeld zu vermeiden. Das Bußgeld ist das Geringste; der Schaden an der Person, deren Daten du schlecht behandelst, ist der Punkt.

**Nicht zu messen ist ein Versagen der Ehrlichkeit.** Wenn du nicht sagen kannst, ob deine KI funktioniert, kannst du deinen Kunden, deinen Mitarbeitenden oder deinen Partnern nicht ehrlich sagen, was du tust. Messen ist Teil davon, im eigenen Geschäft wahrhaftig zu sein.

**Zu groß anzufangen kann die eigenen Leute verletzen.** Ein gescheitertes Big-Bang-Projekt verschwendet das Geld der Firma und das Vertrauen und die Mühe des Teams. Ehrgeiz, der den sicheren Weg ignoriert, kann genau die Menschen beschädigen, denen du helfen willst. Schütze sie, indem du in sicheren Schritten vorgehst.

**Der gemeinsame Faden: wach bleib und verantwortlich bleib.** Jeder Fehler hier ist eine Form des Schlafwandeln — das Leichte tun statt das Sorgfältige. Die ethische Haltung ist die wache Haltung: wähle den Prozess bewusst, respektiere die Daten und die Menschen, verifiziere die Ausgabe, geh in sicheren Schritten, folge den Regeln und miss die Wahrheit.

## Zu vermeidende Fehler

Dieses Kapitel *ist* die Fehlerliste, also hier statt sie zu wiederholen der Meta-Fehler, der alle anderen verbirgt:

**Der Meta-Fehler: KI als ein Produkt behandeln, das man kauft, statt als eine Veränderung, die man managt.** Alle sechs Fehler stammen aus derselben Wurzel — KI wie einen Kauf zu behandeln, der von allein funktioniert, statt wie eine Veränderung, die Auswählen, Vorbereiten, Beaufsichtigen und Messen braucht. Wenn du ein Tool kaufst und erwartest, dass es von sich aus liefert, rutschst du in jede Falle auf einmal: falscher Prozess, schlechte Daten, blindes Vertrauen, zu groß, keine Regeln, kein Messen.

**Die Behebung des Meta-Fehlers: Behandle KI als eine gemanagte Veränderung.** Wähle das Ziel absichtlich. Bereite die Daten und die Menschen vor. Beaufsichtige die Ausgabe. Fang klein an und skaliere mit Plan. Folge den Regeln. Miss das Ergebnis. Das ist das ganze Buch in einem Satz, und es ist das Gegenteil des Schlafwandels, der jedes Scheitern hier verursacht.

Ein zweiter Meta-Fehler, den es zu benennen lohnt: **aus einem gescheiterten Projekt schließen, „KI funktioniert nicht".** Wenn ein Projekt scheitert, war die Ursache fast immer einer der sechs Fehler, nicht die Technik. Wirf die Chance nicht weg, weil du auf eine Landmine getreten bist. Lerne, welche Landmine es war, vermeide sie beim nächsten Mal und versuch es mit Disziplin erneut. Die Tools funktionieren, wenn du die Fehler vermeidest.

## Praktische Übung

### 24.8 Übung: Prüfe deinen Plan gegen die sechs Fehler

Nimm ein KI-Projekt, das du planst oder führst, und prüfe es gegen die sechs Fehler. Antworte auf jeden ehrlich mit Ja/Nein und einer Zeile Beleg.

**1. Falscher Prozess?** „Habe ich dieses Ziel nach Wirkung und Eignung gewählt, nicht nur nach Begeisterung?" Wenn nein, geh zurück und benutz den Wirkung-gegen-Mühelosigkeit-Test (Kapitel 12).

**2. Daten und Menschen unterschätzt?** „Sind meine Daten sauber genug, und habe ich echte Zeit für Schulung und Wandel eingeplant?" Wenn nein, behebe die Daten und plane die Menschenarbeit, bevor du weitergehst.

**3. Der KI zu sehr vertraut?** „Gibt es bei allem, was zählt, eine menschliche Prüfung, und wissen die Leute, wie eine falsche Antwort aussieht?" Wenn nein, füge die Prüfregel jetzt hinzu, bevor weitere Ausgabe hinausgeht.

**4. Zu groß angefangen?** „Fange ich mit einer engen Aufgabe und einem Team an oder gehe ich breit?" Wenn breit, schrumpfe auf einen Pilot und beweise zuerst Wert.

**5. Vorschriften und Sicherheit ignoriert?** „Weiß ich, welche Regeln für mich gelten, und sind die Daten geschützt?" Wenn unsicher, finde es heraus und behebe es, bevor du sensiblere Daten verarbeitest.

**6. Nicht gemessen?** „Habe ich einen Ausgangswert und ein paar ehrliche KPIs, die ich tatsächlich beobachte?" Wenn nein, richte sie jetzt ein, selbst wenn du den Ausgangswert rekonstruieren musst.

Schreibe für jedes „Nein" eine konkrete Maßnahme zur Behebung, mit einem Datum. Geh im Projekt nicht weiter, bis die „Nein"-Antworten behoben sind. Dieses Zehn-Minuten-Audit fängt die meisten teuren Fehler ein, bevor sie dich etwas kosten. Behalte die Antworten und prüfe sie am Prüfungstermin erneut.

## Checkliste

### 24.9 Anti-Fehler-Checkliste

Lauf diese vor und während jedem KI-Projekt durch.

- [ ] **Du hast das Ziel nach Wirkung und Eignung gewählt**, nicht nach Begeisterung oder Gewohnheit.
- [ ] **Du hast den Prozess vor dem Automatisieren behoben oder vereinfacht.**
- [ ] **Du hast die Datenqualität geprüft** und die Daten behoben, bevor du gute Ausgabe erwartet hast.
- [ ] **Du hast echte Zeit und Geld für die menschliche Seite eingeplant** — Schulung, Kommunikation, Wandel.
- [ ] **Du behältst bei allem, was zählt, eine menschliche Prüfung** — die KI entwirft, ein Mensch sendet.
- [ ] **Du hast die Leute angeleitet, falsche Ausgabe zu erkennen**, nicht nur Knöpfe zu drücken.
- [ ] **Du behandelst selbstbewusste, flüssige Ausgabe misstrauisch** und verifizierst, was zählt.
- [ ] **Du hast Eskalationsregeln gesetzt** — Routine an die KI, Wichtiges und Seltsames an einen Menschen.
- [ ] **Du bist klein angefangen** — eine enge Aufgabe, ein Team, ein klares Ziel.
- [ ] **Du skalierst in Schritten** mit Plan, nicht in einem Big-Bang-Rollout.
- [ ] **Du weißt, welche Vorschriften für dich gelten** (DSGVO, EU AI Act), und du befolgst sie.
- [ ] **Du schützt sensible Daten** mit echter Sicherheit vom ersten Tag an, nicht später angeschraubt.
- [ ] **Du behandelst Compliance als laufend**, nicht als einmalige Prüfung.
- [ ] **Du hast vor dem Start einen Ausgangswert gemessen.**
- [ ] **Du verfolgst ehrliche KPIs** (Zeit, Fehler, Kosten, Zufriedenheit), keine Eitelkeits-Metriken.
- [ ] **Du prüfst die Zahlen regelmäßig** und nutzt sie, um Behalten / Korrigieren / Stoppen zu entscheiden.
- [ ] **Du behandelst KI als eine gemanagte Veränderung**, nicht als ein Produkt, das von allein liefert.
- [ ] **Du hast nicht „KI funktioniert nicht" geschlossen** aus einem Fehler, der deiner zu vermeiden war.

Wenn ein Kästchen leer ist, stehst du auf einer Landmine. Geh um sie herum, bevor du mehr Geld oder Vertrauen ausgibst. Jeder Fehler auf dieser Liste ist alt, häufig und vermeidbar — sobald du weißt, dass er da ist.

## Das Wichtigste

- Die meisten KI-Scheitern stammen von sechs alten, vorhersehbaren Fehlern — falscher Prozess, schwache Daten und Menschen, zu viel Vertrauen, zu groß, ignorierte Regeln und Sicherheit, kein Messen — und alle sind vermeidbar, sobald du sie kennst.
- Der gefährlichste einzelne Fehler ist, flüssiger KI-Ausgabe zu sehr zu vertrauen; behalte bei allem, was zählt, eine menschliche Prüfung, denn Flüssigkeit ist nicht Wahrheit.
- Die Wurzel jedes Fehlers ist, KI als ein Produkt zu behandeln, das man kauft, statt als eine Veränderung, die man managt — wählen, vorbereiten, beaufsichtigen, in Schritten skalieren, den Regeln folgen und messen.
- Fang klein an und beweise Wert, bevor du breit gehst; ein enger Sieg, den du kontrollieren kannst, schlägt einen großen Rollout, den du nicht kannst.
- Schließe nicht „KI funktioniert nicht" aus einem gescheiterten Projekt — benenne, welcher Fehler es verursachte, behebe ihn und versuch es mit Disziplin erneut.
