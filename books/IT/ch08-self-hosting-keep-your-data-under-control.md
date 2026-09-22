# Capitolo 8 — Self-hosting: tieni i tuoi dati sotto controllo

## In parole semplici

Self-hosting significa far girare un software su computer che possiedi o controlli tu, invece di affittarlo dai computer di qualcun altro.

Conosci già entrambe le situazioni. Affittare una camera d'albergo è il cloud: qualcun altro pulisce, ripara e tiene una copia delle chiavi. Avere una casa di proprietà è il self-hosting: la caldaia la ripari tu, ma nessun altro ha le chiavi.

Applicato all'AI, il self-hosting significa che il modello — il software che fa il ragionamento — gira su una macchina del tuo ufficio o su un server che controlli tu. Le tue domande entrano lì. Le risposte escono da lì. Niente viaggia su internet verso un'azienda che non hai scelto tu.

Fino a poco tempo fa questo non era possibile per una piccola impresa. Fino al 2022 i migliori modelli linguistici vivevano solo dentro enormi centri di dati, e si potevano raggiungere solo attraverso una porta affittata chiamata API — un'interfaccia standard che un'azienda apre per permettere ad altri software di fare domande ai suoi sistemi. Ogni domanda che scrivevi passava da quella porta e finiva sulle loro macchine.

Poi due cose sono cambiate. Primo, sono comparsi i modelli aperti: modelli i cui file già addestrati chiunque può scaricare e far girare. Secondo, le tecniche di compressione sono diventate abbastanza buone da far girare un modello compresso su un normale computer desktop potente, con solo una piccola perdita di qualità.

Lo scambio è un triangolo, e non puoi avere tutti e tre gli angoli insieme.

- **Controllo.** Decidi tu cosa succede ai tuoi dati, quale modello usi, quando cambia e chi può vederlo.
- **Capacità.** Quanto è davvero bravo l'AI nei compiti difficili.
- **Costo.** Cosa paghi, in denaro, tempo e attenzione.

L'AI su cloud offre alta capacità con poco sforzo e poco controllo. Il self-hosting offre alto controllo, capacità media, e un costo che paghi in anticipo nell'hardware e poi di nuovo nel tempo continuo. La risposta giusta dipende da cosa stai facendo.

Due frasi oneste prima di andare oltre. Il self-hosting non è automaticamente più sicuro — un server locale configurato male è peggio di un servizio cloud ben gestito. E il self-hosting non è automaticamente più economico — su piccola scala, affittare di solito vince. Ciò che il self-hosting ti fa guadagnare è una cosa specifica e preziosa: i tuoi dati non escono, e nessuno può cambiare il tuo sistema senza che tu lo sappia.

Argomenti correlati altrove: il [Capitolo 11](ch11-digital-sovereignty.md) tratta l'idea più ampia di controllare i propri strumenti digitali, il [Capitolo 9](ch09-third-party-services-and-shadow-ai.md) tratta il modello opposto dei servizi di terze parti non gestiti, e il [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md) tratta le basi della sicurezza che valgono ancora per una macchina nel tuo stesso ufficio.

## Un po' di storia

**Anni '90 e 2000: tutto in casa.** Una piccola impresa aveva un server in un armadio. Email, file e account stavano tutti in sede. La macchina era tua, e così tutti i suoi problemi.

**Anni 2000–2018: la migrazione verso l'esterno.** La banda larga è diventata veloce, e affittare è diventato più facile che possedere. Prima è andata l'email, poi i file, poi la contabilità e i record dei clienti. "Il cloud" è diventato la risposta di default. La battuta tra gli ingegneri era esatta: non esiste il cloud, è solo il computer di qualcun altro.

**2013: i container.** È arrivato Docker e ha impacchettato il software in modo che girasse allo stesso modo ovunque. Questo, in silenzio, ha reso di nuovo facile il self-hosting, perché non serviva più uno specialista per ricostruire un'applicazione su ogni nuova macchina.

**2022: l'AI era solo a noleggio.** I migliori modelli linguistici esistevano solo dentro una manciata di grandi aziende. Se volevi l'AI, mandavi il tuo testo a loro. Non c'era un'alternativa che valesse la pena usare.

**2023: l'anno dei modelli aperti.** Meta ha rilasciato Llama come modello di ricerca a febbraio, poi Llama 2 con pesi aperti a luglio. Mistral AI ha rilasciato un forte modello da sette miliardi di parametri ad agosto. "Pesi aperti" significa che i file addestrati sono pubblicati, quindi chiunque può scaricarli e farli girare. Lo stesso anno, la quantizzazione — comprimere un modello così che richieda molta meno memoria — è diventata abbastanza buona per l'uso quotidiano. All'improvviso un'AI capace non stava più solo in un centro di dati.

**8 luglio 2023: Ollama.** È stato rilasciato un tool chiamato Ollama, open source con licenza MIT, scritto principalmente in Go con un po' di C e TypeScript, da Jeffrey Morgan e Michael Chiang. Il suo compito era eliminare ogni attrito. Un solo comando scarica un modello e lo fa girare in locale, con un'interfaccia semplice e un servizio locale a cui altri programmi possono parlare. Usava il motore llama.cpp per il lavoro vero sulla tua hardware.

**2024: "sovrano" diventa un criterio d'acquisto.** Aziende di settori regolamentati, e diversi governi europei, hanno iniziato a chiedere un'AI che resti dentro un Paese e dentro i propri confini. I fornitori cloud hanno risposto con opzioni di cloud sovrano, e un mercato per l'AI on-premise è cresciuto rapidamente.

**2026: un client enterprise open source.** Ad aprile 2026 MZLA Technologies, una sussidiaria di Mozilla, ha annunciato Thunderbolt, un client AI open source progettato per essere self-hostato. La sezione Curiosità ne parla.

La forma di questa storia è un cerchio. Abbiamo iniziato col self-hosting, ci siamo spostati fuori per comodità, e ora stiamo tornando indietro per avere controllo — con strumenti molto migliori della prima volta.

## Curiosità

### 8.7 Il client AI open source di Mozilla per "un'AI che controlli tu"

Ad aprile 2026, MZLA Technologies Corporation — una sussidiaria al 100% di Mozilla, il non-profit dietro Firefox — ha annunciato **Thunderbolt**. È un client AI open source, multipiattaforma, costruito per organizzazioni che vogliono far girare l'AI alle proprie condizioni.

I dettagli che contano per questo capitolo:

- **Self-hostabile.** Gira sull'infrastruttura del cliente stesso. Il progetto descrive il supporto per configurazioni on-premise, cloud sovrano e air-gapped — cioè una rete fisicamente scollegata da internet.
- **Agnostico sul modello.** Funziona con qualsiasi agente che parli l'Agent Client Protocol, e con qualsiasi modello che offra un'API compatibile con OpenAI. In pratica significa che puoi puntarlo su un modello locale, sul tuo server, o su un fornitore commerciale, e cambiare senza modificare i tuoi strumenti.
- **Ovunque.** Web, Windows, macOS, Linux, iOS e Android.
- **Connesso ai tuoi sistemi.** Si integra con i sistemi aziendali attraverso il Model Context Protocol — un modo standard per far raggiungere a un tool AI i tuoi dati e le tue azioni interne — e supporta automazioni riutilizzabili e un'API estensibile.
- **Verificabile.** Poiché il codice è aperto, tu o un terzo potete leggerlo e controllare cosa fa davvero. Il progetto ha dichiarato di essere in fase di audit di sicurezza.
- **Un partner per la sovranità europea.** Si abbina a Haystack di deepset, una piattaforma di orchestrazione open source, per distribuzioni sovrane in Europa.
- **Supporto incluso.** Sono offerti supporto enterprise e ingegneria dedicata sul campo, che è la parte che la maggior parte dei progetti open source ti lascia risolvere da solo.

Vale la pena notare il posizionamento. La cornice è "un'AI che controlli tu", e l'argomento è che l'AI è troppo importante per esternalizzarla del tutto. È lo stesso argomento che fa un piccolo imprenditore quando decide di tenere i file delle paghe sulla propria macchina invece che in un servizio che non ha mai ispezionato.

Un esempio più piccolo e più vecchio della stessa idea si trova in un'app di email che molte persone usano già. Il componente aggiuntivo ThunderAI per Thunderbird ha aggiunto il supporto per modelli locali tramite Ollama nella versione 2.1.1, rilasciata ad agosto 2024. Con quella configurazione il modello gira sul tuo computer, così il testo delle email non lascia mai la macchina, e non serve alcun account cloud o chiave API. È una piccola funzione, e il punto lo rende chiaramente: l'AI locale non è più un progetto di ricerca. È un'opzione dentro un client email gratuito.

## Un esempio di business reale

### Anche Apple si è costruita il proprio cloud

Apple è un'azienda che potrebbe affittare quasi qualsiasi cosa. Nel giugno 2024 ha annunciato un sistema chiamato Private Cloud Compute, costruito per le funzioni AI dei suoi dispositivi quando un compito è troppo grande per il telefono stesso. Ciò che ha scelto di fare con quel sistema è la lezione.

Apple ha costruito i propri server attorno ai propri chip con un sistema operativo irrobustito. Ha progettato il sistema per un'inferenza stateless — elabora la richiesta, restituisci la risposta, non tenere nulla. E ha fatto una promessa insolita: avrebbe pubblicato l'immagine software di ogni build di produzione così che ricercatori di sicurezza esterni potessero ispezionare esattamente cosa sta girando, e verificare che la macchina con cui stanno parlando sia davvero ciò che dice di essere. Nell'ottobre 2024 Apple ha pubblicato una guida di sicurezza e ha invitato i ricercatori ad attaccare il sistema.

Per una piccola impresa ne seguono tre cose.

Primo, nota il ragionamento. Apple non ha costruito un cloud perché non riusciva ad affittarne uno. L'ha costruito perché affittarlo avrebbe significato tenere i dati degli utenti alle condizioni di qualcun altro, e tutto il suo marchio sta nel fatto che non lo fa. Il controllo della macchina per loro valeva soldi veri.

Secondo, nota l'idea di verifica. Pubblicare il software perché gli esterni possano controllarlo è lo stesso istinto dell'audit open source. La fiducia si riduce rendendo il sistema ispezionabile, non promettendo di essere bravi.

Terzo, nota la dimensione del divario. Apple ha speso una fortuna per arrivare a "non teniamo nulla". La maggior parte delle piccole imprese non può copiarlo. Ma puoi copiare la domanda: *chi gestisce la macchina dove finiscono i miei dati, cosa tengono, e qualcuno può verificarlo?* Se non riesci a rispondere a queste tre domande su un tool, non dovresti metterci dati sensibili. E se la risposta onesta è "non possiamo verificare", un modello che gira sulla tua macchina diventa un'opzione seria.

## Come si fa

### 8.5 Come iniziare: da tool open source come Ollama ai modelli locali

**Passo 1: scegli un compito e una persona.**
Non comprare prima l'hardware. Scegli un compito ripetitivo che coinvolge dati sensibili — riassumere contratti, scrivere risposte a richieste standard, trasformare appunti di riunioni in liste di azioni. Dalo a una persona curiosa con un buon computer.

**Passo 2: installa Ollama.**
Ollama gira su Windows, macOS e Linux. Dopo l'installazione, un solo comando scarica un modello e avvia una chat nel tuo terminale. Sotto la cappuccetta avvia un piccolo servizio sulla tua macchina, sulla porta 11434, a cui altri programmi possono parlare. È quel servizio locale che ti permette di collegare il modello ai tuoi strumenti più avanti.

**Passo 3: scegli il modello dalla dimensione, non dal nome.**
Le dimensioni dei modello si contano in parametri, una misura approssimativa di quanto il modello è grande e capace. Come regola pratica:

- **Da 1 a 3 miliardi** — veloce e leggero, gira su un normale portatile. Buono per riassunti brevi e bozze semplici.
- **Da 7 a 9 miliardi** — la via di mezzo pratica. Buona qualità generale, richiede una macchina decente con abbastanza memoria.
- **70 miliardi e oltre** — molto più forte, ma richiede hardware serio e molta memoria. Di solito non è un punto di partenza per una piccola impresa.

Cerca le versioni **quantizzate**. La quantizzazione comprime i numeri dentro il modello così richiede molta meno memoria e gira più veloce, al prezzo di un piccolo calo di qualità. Per la maggior parte dei compiti d'ufficio quel calo è accettabile.

**Passo 4: aggiungi un'interfaccia amichevole.**
Il terminale va bene per i test. Per l'uso quotidiano, aggiungi un'interfaccia chat che gira localmente, oppure collega il modello a un'app che la gente usa già — il componente aggiuntivo per Thunderbird menzionato sopra è un esempio. L'obiettivo è che un collega non tecnico possa usarlo senza aiuto. Se solo una persona sa pilotarlo, non verrà mai adottato.

**Passo 5: fallo restare davvero locale.**
È qui che le persone falliscono. Il servizio locale deve ascoltare solo sulla tua macchina, non su tutta la rete. I ricercatori di sicurezza hanno trovato molti server Ollama esposti a internet perché impostati per accettare connessioni da qualsiasi indirizzo. Quindi: tieni il binding locale di default, metti un firewall davanti, non aprire mai la porta 11434 su internet, e non farlo girare con diritti di amministratore. Un tool locale non è automaticamente un tool sicuro.

**Passo 6: fallo leggere i tuoi file.**
Il passo successivo più utile è il retrieval, spesso chiamato RAG. In parole povere: invece di riaddestrare il modello, metti i tuoi documenti in un indice ricercabile. Quando qualcuno fa una domanda, il sistema trova i passaggi rilevanti e li passa al modello insieme alla domanda. Il modello risponde dai tuoi documenti. Nulla viene addestrato sui tuoi dati, e tutto può girare sulla tua macchina. È così che ottieni "chiedi al nostro manuale" senza mandare il manuale da nessuna parte.

**Passo 7: scala solo quando il test ha funzionato.**
Se il pilota è utile, allora compra l'hardware. Una workstation con una scheda grafica potente è la risposta usual, perché è la memoria grafica a limitare quanto grande può essere un modello che puoi far girare. Le macchine Apple con memoria unificata sono una scelta comune per la stessa ragione. Un piccolo server ha senso quando più persone lo servono allo stesso tempo.

**Passo 8: decidi la divisione.**
La maggior parte delle aziende finisce ibrida. Dati sensibili e compiti ad alto volume di routine girano localmente. Ragionamento difficile, documenti molto lunghi e funzioni specialistiche usano un servizio cloud con un contratto adeguato. Scrivi la regola: quali dati vanno dove, e chi decide.

### 8.6 Casi d'uso ideali

**Dati personali sensibili.** Cartelle cliniche, fascicoli del personale, paghe, CV dei candidati, dettagli finanziari dei clienti. Se i dati non devono uscire, l'elaborazione locale elimina del tutto la domanda.

**Informazioni proprietarie.** Progetti, disegni, codice sorgente, documenti di gara e offerta, modelli di prezzo, piani strategici. Sono i file che farebbero più male se un fornitore li tenesse o li perdesse.

**Settori regolamentati.** Sanità, studi legali, banche e assicurazioni, governo e difesa, e qualsiasi azienda soggetta a regole di residenza dei dati che richiedono che i dati restino dentro un Paese o una regione. Il self-hosting trasforma una conversazione di compliance difficile in una semplice.

**Connettività scarsa o assente.** Cantieri, fabbriche, navi, miniere, uffici remot, risposta alle emergenze. Un modello locale funziona quando internet non funziona.

**Lavoro ripetitivo ad alto volume.** Migliaia di ticket, fatture o documenti. Un prezzo per richiesta fa male ad alto volume; una macchina fissa non cresce.

**Sperimentazione economica.** Provare idee senza un contatore che gira. Utile prima di impegnare budget.

**Dove si adatta male:** ragionamento di frontiera, documenti molto lunghi, generazione avanzata di immagini, e qualsiasi team senza alcun supporto tecnico. Se nessuno può mantenerlo, non iniziare.

## Etica e responsabilità

Il self-hosting risolve un problema etico e ne crea altri. Sia chiaro quale è quale.

**Cosa risolve.** I dati dei tuoi clienti smettono di viaggiare verso aziende che non hai scelto, e non possono essere usati per addestrare il prodotto di qualcun altro senza di te. È un vero guadagno di rispetto verso le persone di cui tieni i dati.

**Cosa non risolve.** Il modello può ancora essere sbagliato, di parte, o con sicurezza fuorviante. Far girare un modello di parte sul tuo hardware non lo rende equo. I doveri del [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md) valgono ancora, e così le regole di divulgazione del [Capitolo 5](ch05-rules-and-legal-responsibility.md).

**Cosa aggiunge.** Ora l'operatore sei tu. Patch, controllo degli accessi, logging e backup sono compito tuo. Se un server locale non patchato perde dati, è colpa tua in un modo nuovo e molto diretto.

**Monitoraggio dei dipendenti.** Se registri le domande su un sistema locale, ora tieni un record dettagliato di cosa hanno chiesto i tuoi dipendenti. Abbi una policy scritta su cosa viene tenuto, perché, chi lo legge e per quanto tempo. Mantienila proporzionata, e informa le persone.

**Non sopravvalutare la sovranità.** "Sovrano" è una parola di marketing quanto una tecnica. Se rivendichi controllo ma non puoi fare patch, backup o audit, la rivendicazione è vuota. Dì cosa hai davvero, e dì chiaramente cosa non hai.

**Energia.** Una macchina che fa girare modelli tutto il giorno consuma corrente. Il locale non è automaticamente più verde di un grande centro di dati efficiente. Se rivendichi un beneficio ambientale, verificalo prima.

## Errori da evitare

1. **Comprare hardware prima di testare un compito.** Prova prima con una configurazione affittata o prestata. L'hardware comprato sulla speranza resta inutilizzato.
2. **Esporre il servizio AI locale a internet.** È l'errore di self-hosting più comune e più grave. Tienilo locale, mettilo dietro un firewall, non aprire la porta.
3. **Dare per scontato che locale equivalga a sicuro.** Ora possiedi la sicurezza di quella macchina, incluse le parti a cui non avevi mai pensato.
4. **Nessun backup.** La macchina, i modelli, la configurazione e l'indice dei documenti hanno tutti bisogno di backup.
5. **Scegliere il modello più grande.** Più grande è più lento, più affamato, e spesso non migliore per il tuo compito reale.
6. **Ignorare le licenze dei modelli.** I modelli a pesi aperti vengono con termini diversi, incluse regole sull'uso commerciale e su come puoi descrivere il tuo uso. Leggi la licenza prima di costruirci sopra.
7. **Dipendenza da una sola persona.** Se una sola persona sa come funziona e se ne va, il sistema si ferma. Scrivi la configurazione, il riavvio e i passi di ripristino.
8. **Self-hostare il carico di lavoro sbagliato.** Se il compito richiede qualità di frontiera, il locale deluderà, e concluderai per errore che la tecnologia è inutile.
9. **Non aggiornare mai, o aggiornare senza testare.** Una nuova versione di un modello cambia le risposte. Riesegui i tuoi compiti campione dopo ogni modifica.
10. **Trattarlo come tutto o niente.** Una configurazione ibrida è di solito la risposta giusta, non uno spostamento totale in una direzione o nell'altra.

## Esercizio pratico

### 8.8 Valuta se il self-hosting fa per la tua azienda

Assegna a ogni riga un punteggio 0, 1 o 2. Sii onesto.

| Domanda | 0 | 1 | 2 |
|---|---|---|---|
| Quanto è sensibile il dato? | Pubblico | Interno | Riservato al cliente o regolamentato |
| Supporto tecnico disponibile | Nessuno | Help IT part-time | Qualcuno che può mantenere un server |
| Budget hardware | Nessuno | Una buona workstation | Workstation più un piccolo server |
| Complessità del compito | Riassunti e bozze | Domande su documenti | Ragionamento complesso, documenti molto lunghi |
| Connettività | Inaffidabile | Buona | Buona |
| Volume | Occasionale | Quotidiano | Alto e in crescita |

Leggi il punteggio riga per riga, perché le righe non spingono tutte nella stessa direzione.

- **Sensibilità 2** e **Volume 2** entrambi spingono verso il self-hosting.
- **Supporto tecnico 0** spinge fortemente contro, qualunque sia il punteggio delle altre righe.
- **Complessità del compito 2** spinge contro, perché i modelli locali restano indietro nel ragionamento difficile.

Ora fai un test di un giorno prima di spendere qualsiasi cosa. Prendi venti compiti reali dalla tua lista. Falli dieci con un modello locale di media dimensione e dieci con un servizio cloud. Confronta tre cose: la risposta era abbastanza buona da usarla così com'era, quanto tempo ci è voluto, e quanto sarebbe costato nell'altro modo. Scrivi i risultati.

Se la risposta locale era utilizzabile per la maggior parte dei compiti, il self-hosting vale l'investimento. Se era utilizzabile solo per pochi, tieni quelli in locale e lascia il resto sul cloud con un contratto. In ogni caso ora hai prove invece di un'opinione.

## Checklist

### 8.9 Cosa ti serve per iniziare

- [ ] **Un compito nominato** che coinvolge dati sensibili e si ripete spesso.
- [ ] **Una persona nominata** che sappia installare, riavviare, fare backup e aggiornare il sistema — o un piano per assumerne una.
- [ ] **Una macchina con abbastanza memoria**, scelta dopo un test, non prima.
- [ ] **Un modello scelto per dimensione e quantizzazione**, adattato al compito anziché al più grande disponibile.
- [ ] **Un'interfaccia locale** che un collega non tecnico possa usare senza aiuto.
- [ ] **Il servizio agganciato solo alla macchina locale**, dietro firewall, senza porte aperte su internet.
- [ ] **Un controllo scritto della licenza** per il modello che scegli, inclusi i termini di uso commerciale.
- [ ] **Un piano di backup** per la macchina, i modelli, la configurazione e l'indice dei documenti.
- [ ] **Una routine di patch** con una data fissa, e un re-test dei compiti campione dopo ogni modifica.
- [ ] **Una regola di divisione scritta** che indichi quali dati restano locali e quali possono usare un servizio cloud, e chi decide.

## Punti chiave

- Il self-hosting significa che l'AI gira su macchine che controlli tu, così i tuoi dati non le lasciano.
- È diventato pratico per le piccole imprese quando sono arrivati i modelli a pesi aperti e una buona compressione nel 2023, e tool come Ollama hanno eliminato l'attrito della configurazione.
- Scambi capacità e comodità con il controllo: il triangolo è controllo, capacità e costo, e non puoi averli tutti e tre.
- Il locale non è automaticamente sicuro o economico; un server locale configurato male è un rischio reale, e la manutenzione ora è compito tuo.
- Inizia con un compito, una persona e un test di un giorno prima di comprare qualsiasi hardware.
