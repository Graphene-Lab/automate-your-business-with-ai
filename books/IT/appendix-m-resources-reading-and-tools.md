# Appendice M — Risorse, letture e strumenti consigliati

Un elenco breve e onesto di strumenti e letture. **Non** sono pubblicità. Sono progetti reali e nominati che puoi verificare da solo. La maggior parte è open-source, il che significa che puoi vedere come funzionano e non sei bloccato a una sola azienda.

**Una nota sul livello di competenza:** alcuni strumenti qui richiedono una persona tecnica (un partner IT, uno sviluppatore o un assunto esperto di tecnologia). Non devi farli girare tu stesso. Leggili per sapere cosa è possibile e per parlare in modo consapevole con chi li configura.

**Verificato:** ogni strumento e libro qui sotto è stato controllato rispetto al proprio sito web o al proprio repository di codice nel **settembre 2026**. Gli strumenti cambiano in fretta — ricontrolla prima di adottarli.

## Far girare l'IA in locale (sui tuoi macchinari)

Far girare i modelli in locale significa che l'IA lavora sul tuo computer o server. I tuoi dati non lasciano la tua macchina. È l'opzione più privata.

- **Ollama** — `ollama.com`. Uno strumento gratuito e open-source per far girare modelli IA aperti sul tuo computer. I modelli locali non costano nulla e tengono i dati sulla tua macchina. È il punto di partenza più facile per l'IA locale e viene spesso usato come motore dietro altri strumenti.
- **Thunderbolt** — `thunderbolt.io` (codice: `github.com/Thunderbird/thunderbolt`). Un **client IA** open-source e auto-ospitabile di MZLA Technologies, la sussidiaria di Mozilla che produce anche Thunderbird. Annunciato nell'aprile 2026 e con licenza Mozilla Public License 2.0. La sua promessa è "AI You Control: scegli i tuoi modelli, possiedi i tuoi dati, elimina il lock-in del fornitore". Funziona su web, Windows, macOS, Linux, iOS e Android, e opera con modelli locali, in sede o cloud. Per l'uso locale si appoggia a Ollama o llama.cpp. **Stato:** nelle prime fasi e sotto una verifica di sicurezza — consideralo promettente, non finito.
- **llama.cpp** — un noto motore open-source che fa girare grandi modelli su hardware informatico ordinario, incluso il tuo portatile. È il motore tecnico su cui altri costruiscono. Lo citiamo qui perché Thunderbolt lo raccomanda per l'inferenza locale gratuita.

**Quando scegliere il locale:** tratti dati sensibili, vuoi evitare le tariffe per messaggio, o hai bisogno che l'IA funzioni senza inviare dati all'esterno. Il compromesso: paghi hardware e configurazione, e i modelli locali di solito sono più piccoli dei più grandi modelli cloud.

## Costruire automazioni (collegare l'IA al tuo lavoro)

Questi strumenti ti permettono di integrare l'IA in compiti reali — leggere documenti, rispondere a ticket, spostare dati tra app.

- **Haystack** — `haystack.deepset.ai` (codice: `github.com/deepset-ai/haystack`). Un framework open-source di **deepset** (Germania) per costruire applicazioni IA, in particolare pipeline **RAG**. RAG ("retrieval-augmented generation", generazione aumentata dal recupero) significa che l'IA consulta i tuoi documenti prima di rispondere, così risponde dai tuoi fatti, non da ipotesi. Gratuito da installare (`pip install haystack-ai`); il supporto enterprise a pagamento è opzionale. Ideale per un team con uno sviluppatore.
- **n8n** — `n8n.io`. Una piattaforma di automazione **fair-code** (il sorgente è pubblico su GitHub) che ti permette di costruire flussi di lavoro su una tela visuale e collegarti a oltre 500 app. Costruisce anche agenti IA e sistemi RAG, con approvazioni umane nel ciclo. Puoi auto-ospitarla o usare il loro cloud. "Fair-code" significa che il codice è aperto da leggere e auto-ospitare, ma non è una licenza open-source standard — controlla i termini se prevedi di rivenderlo.

**Quando scegliere questi:** vuoi che l'IA agisca sui tuoi dati attraverso più app, non solo in chat. Haystack serve a costruire pipeline IA su misura; n8n serve a collegare app e automatizzare passi con l'IA dentro di esse.

## Approfondire (letture)

- **Headcount Zero: How to Build an AI-Run Company with Paperclip** — di **Anthony David Adams**. Un libro open-source (su GitHub, licenza CC BY-NC-SA 4.0) su come gestire un'azienda dove gli agenti IA fanno la maggior parte del lavoro e un piccolo numero di umani giudica l'output. Copre l'idea della "azienda di una sola persona", come funzionano gli agenti IA, l'economia di pochi dipendenti e come governare l'IA con interruttori di arresto. Leggilo per la visione audace — poi applicalo con la cautela che questo libro insegna: tieni gli umani al comando di ciò che conta.
- **I capitoli di questo stesso libro** — la migliore "ulteriore lettura" sono spesso i capitoli che hai sfoltito. Rileggi il capitolo sui rischi prima di ogni lancio, e il capitolo sui dati prima di collegare qualsiasi strumento a dati reali dei clienti.
- **Documentazione di fornitori e progetti** — per qualsiasi strumento qui sopra, leggi la documentazione e la licenza del progetto prima di adottarlo. Ti dice cosa è gratuito, cosa è a pagamento e a cosa stai acconsentendo.

## Come scegliere, in tre domande

1. **Dove devono restare i dati?** Se non devono lasciare le tue macchine, guarda gli strumenti locali (Ollama, Thunderbolt, llama.cpp).
2. **Hai aiuto tecnico?** Se sì, Haystack e n8n aprono più porte. Se no, inizia con uno strumento ospitato semplice e un piccolo pilota.
3. **Puoi andartene più tardi?** Preferisci strumenti che ti permettono di esportare i dati e cambiare modello. Evita tutto ciò che blocca i tuoi dati dentro.

## Un avvertimento sugli elenchi come questo

Gli strumenti salgono e cadono. Un nome qui può cambiare, fondersi o sparire entro un anno. È normale nell'IA. I **principi** di questo libro — tieni i dati privati, tieni un umano nel ciclo, misura i risultati, evita il lock-in — sopravvivono a qualsiasi singolo strumento. Usa questo elenco come una mappa, non come una promessa.
