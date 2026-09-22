# Anhang M — Ressourcen, Lektüre und empfohlene Werkzeuge

Eine kurze, ehrliche Liste von Werkzeugen und Lektüre. Das sind **keine** Anzeigen. Es sind echte, namentlich genannte Projekte, die du selbst nachschlagen kannst. Die meisten sind Open Source, das heißt, du kannst sehen, wie sie funktionieren, und bist an keine Firma gebunden.

**Hinweis zum Können:** Manche Werkzeuge hier brauchen eine technische Person (einen IT-Partner, einen Entwickler oder eine technisch versierte Einstellung). Du musst sie nicht selbst betreiben. Lies sie, um zu wissen, was möglich ist, und um mit wem auch immer sie einrichtet, klug zu sprechen.

**Geprüft:** Jedes Werkzeug und jedes Buch unten wurde im **September 2026** gegen die jeweilige Website oder das Code-Repository geprüft. Werkzeuge ändern sich schnell — prüfe vor der Übernahme neu.

## KI lokal betreiben (auf deinen eigenen Maschinen)

Modelle lokal auszuführen bedeutet, die KI arbeitet auf deinem eigenen Computer oder Server. Deine Daten verlassen deinen Rechner nicht. Das ist die privatste Option.

- **Ollama** — `ollama.com`. Ein freies, Open-Source-Werkzeug, um offene KI-Modelle auf deinem eigenen Computer auszuführen. Lokale Modelle kosten nichts und halten die Daten auf deinem Rechner. Es ist der einfachste Einstieg in lokale KI und wird oft als Motor hinter anderen Werkzeugen genutzt.
- **Thunderbolt** — `thunderbolt.io` (Code: `github.com/Thunderbird/thunderbolt`). Ein Open-Source, selbst hostbarer **KI-Client** von MZLA Technologies, der Mozilla-Tochter, die auch Thunderbird macht. Angekündigt April 2026 und lizenziert unter der Mozilla Public License 2.0. Sein Versprechen ist „AI You Control: choose your models, own your data, eliminate vendor lock-in." Er läuft auf Web, Windows, macOS, Linux, iOS und Android, und funktioniert mit lokalen, On-Premise- oder Cloud-Modellen. Für lokale Nutzung verweist er auf Ollama oder llama.cpp. **Status:** früh in der Entwicklung und unter einem Sicherheits-Audit — sieh ihn als vielversprechend, nicht fertig.
- **llama.cpp** — eine bekannte Open-Source-Engine, die große Modelle auf gewöhnlicher Computer-Hardware ausführt, auch auf deinem eigenen Laptop. Sie ist der technische Motor, auf dem andere aufbauen. Hier erwähnt, weil Thunderbolt sie für kostenlose lokale Inferenz empfiehlt.

**Wann lokal wählen:** du handhabst sensible Daten, willst Gebühren pro Nachricht vermeiden, oder brauchst, dass die KI arbeitet, ohne Daten hinauszusenden. Der Kompromiss: du zahlst für Hardware und Einrichtung, und lokale Modelle sind meist kleiner als die größten Cloud-Modelle.

## Automationen bauen (KI mit deiner Arbeit verbinden)

Diese Werkzeuge lassen du KI in echte Aufgaben einbinden — Dokumente lesen, Tickets beantworten, Daten zwischen Apps verschieben.

- **Haystack** — `haystack.deepset.ai` (Code: `github.com/deepset-ai/haystack`). Ein Open-Source-Framework von **deepset** (Deutschland) zum Bauen von KI-Anwendungen, besonders **RAG**-Pipelines. RAG („retrieval-augmented generation", abrufverstärkte Generierung) bedeutet, die KI schlägt vor dem Antworten in deinen eigenen Dokumenten nach, sodass sie aus deinen Fakten antwortet, nicht aus Vermutungen. Kostenlos zu installieren (`pip install haystack-ai`); bezahlter Enterprise-Support ist optional. Am besten für ein Team mit einem Entwickler.
- **n8n** — `n8n.io`. Eine **Fair-Code**-Automatisierungsplattform (der Quellcode ist öffentlich auf GitHub), mit der du Workflows auf einer visuellen Oberfläche baust und dich mit über 500 Apps verbindest. Sie baut auch KI-Agenten und RAG-Systeme, mit Freigaben durch Menschen (human-in-the-loop). Du kannst sie selbst hosten oder ihre Cloud nutzen. „Fair-code" bedeutet, der Code ist offen zum Lesen und Selbst-Hosten, aber keine Standard-Open-Source-Lizenz — prüfe die Bedingungen, wenn du sie weiterverkaufen willst.

**Wann diese wählen:** du willst, dass KI auf deinen Daten über mehrere Apps hinweg handelt, nicht nur chattet. Haystack ist zum Bauen maßgeschneiderter KI-Pipelines; n8n ist zum Verbinden von Apps und Automatisieren von Schritten mit KI darin.

## Mehr erfahren (Lektüre)

- **Headcount Zero: How to Build an AI-Run Company with Paperclip** — von **Anthony David Adams**. Ein Open-Source-Buch (auf GitHub, Lizenz CC BY-NC-SA 4.0) darüber, eine Firma zu führen, in der KI-Agenten den Großteil der Arbeit machen und eine kleine Zahl von Menschen die Ausgabe beurteilt. Es behandelt die Idee der „Ein-Personen-Firma", wie KI-Agenten arbeiten, die Ökonomie weniger Mitarbeiter und wie man KI mit Not-Ausschaltern (Kill-Switches) steuert. Lies es wegen der mutigen Vision — dann wende es mit der Vorsicht an, die dieses Buch lehrt: lass Menschen das Wichtige kontrollieren.
- **Die eigenen Kapitel dieses Buchs** — die stärkste „weiterführende Lektüre" sind oft die Kapitel, die du überflogen hast. Lies das Risiko-Kapitel vor jedem Start neu, und das Daten-Kapitel, bevor du ein Werkzeug mit echten Kundendaten verbindest.
- **Anbieter- und Projekt-Dokumentation** — lies für jedes Werkzeug oben die eigene Doku und Lizenz des Projekts vor der Übernahme. Sie sagt dir, was frei ist, was bezahlt, und worauf du dich einlässt.

## So wählst du, in drei Fragen

1. **Wo müssen die Daten bleiben?** Wenn sie deine Maschinen nicht verlassen dürfen, schau dir die lokalen Werkzeuge an (Ollama, Thunderbolt, llama.cpp).
2. **Hast du technische Hilfe?** Wenn ja, öffnen Haystack und n8n die meisten Türen. Wenn nein, starte mit einem einfachen gehosteten Werkzeug und einem kleinen Piloten.
3. **Kannst du später wieder weg?** Gib Werkzeugen den Vorzug, die dir erlauben, deine Daten zu exportieren und Modelle zu wechseln. Vermeide alles, was deine Daten einschließt.

## Eine Warnung zu Listen wie dieser

Werkzeuge steigen und fallen. Ein Name hier kann sich innerhalb eines Jahres ändern, fusionieren oder verblassen. Das ist normal bei KI. Die **Prinzipien** in diesem Buch — halte Daten privat, halte einen Menschen im Prozess, mess die Ergebnisse, vermeide Lock-in — überdauern jedes einzelne Werkzeug. Nutze diese Liste als Karte, nicht als Versprechen.
