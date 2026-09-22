# Capitolo 24 — Errori comuni e come evitarli

## In parole semplici

La maggior parte dei progetti IA fallisce per lo stesso pugno di ragioni. Non perché la tecnologia è debole, ma per errori prevedibili che le persone commettono ripetutamente. La buona notizia è che una volta conosciuti gli errori, puoi evitarne quasi tutti. Questo capitolo è una visita guidata dei più grandi, con la soluzione per ciascuno.

Pensala come una lista di mine. Ognuna è facile su cui mettere il piede se non sai che è lì, e facile da aggirare se lo sai. L'obiettivo non è spaventarti lontano dall'IA. È farti diventare il tipo di titolare che non fa saltare in aria il proprio progetto per incidente.

I sei grandi errori sono: automatizzare il processo sbagliato, sottovalutare dati e persone, fidarsi troppo dell'IA, iniziare troppo in grande, ignorare regolamenti e sicurezza, e non misurare i risultati. Ognuno è comune, ognuno è costoso, e ognuno ha un modo chiaro per evitarlo. Li prendiamo uno alla volta, spieghiamo perché accade e cosa costa, e ti indichiamo il capitolo che copre la soluzione per intero.

Una semplice immagine da portare con sé: adottare l'IA è come mettersi in cammino per una lunga passeggiata in campagna. La maggior parte delle persone non fallisce perché la strada è impossibile. Fallisce perché ha scelto la destinazione sbagliata, ha messo troppa poca acqua, si è fidata di una mappa difettosa, ha provato a camminare troppo lontano il primo giorno, ha ignorato il meteo, e non ha mai controllato se stava andando nella direzione giusta. Gli errori sono ordinari ed evitabili. Questo capitolo è il briefing di sicurezza prima della partenza.

Leggilo come una checklist contro i tuoi piani. Se ti ritrovi a fare uno di questi, fermati e correggilo prima di spendere più denaro o bruciare più fiducia.

## Un po' di storia

**Anni '80: il collasso dei sistemi esperti insegnò la lezione del processo sbagliato.** Durante il boom dei sistemi esperti, le aziende versarono denaro per codificare le regole degli esperti umani. Molti progetti fallirono perché provarono ad automatizzare compiti troppo disordinati, troppo rari, o troppo dipendenti dal giudizio per essere codificati. I sistemi erano fragili e costosi da aggiornare, e il mercato collassò. La lezione: automatizzare la cosa sbagliata spreca una fortuna, non importa quanto buona è la tecnologia.

**Anni '90: "spazzatura dentro, spazzatura fuori" divenne un mantra.** Mentre le aziende si computerizzavano, impararono che un sistema nutrito di dati cattivi produce risultati cattivi, non importa quanto ingegnoso è il software. Questo vecchio detto informatico divenne centrale in ogni progetto dati. È l'antenato dell'errore odierno di "sottovalutare i dati".

**Anni '90-2000: il modello di fallimento del big-bang.** I progetti di software aziendale degli anni '90 e 2000 erano famosi per andare "big bang" — sostituire tutto in una volta, su un grande piano, nell'arco di anni. Molti sforarono il budget, i tempi, e fallirono del tutto. Il modello era così comune che "implementazione big-bang" divenne un termine di ammonimento. La soluzione che emerse: iniziare piccolo, provare il valore, poi crescere. Questo è l'antenato di "iniziare troppo in grande".

**Anni 2000: compiacimento dell'automazione.** I ricercatori che studiavano sistemi automatizzati — autopiloti, monitoraggio automatico — trovarono un fallimento sorprendente: quando un sistema funziona bene la maggior parte del tempo, gli umani smettono di prestare attenzione e si fidano troppo. Poi fallisce su un caso raro e nessuno lo coglie. Questo si chiama **compiacimento dell'automazione** o **bias dell'automazione**, ed è esattamente l'errore di "fidarsi troppo dell'IA". Fu documentato molto prima delle chatbot ed è ora più rilevante che mai.

**Anni 2010: il regolamento recupera il ritardo.** Mentre violazioni di dati e abusi finivano sui titoli, i governi iniziarono a scrivere regole severe — il GDPR in Europa il più grande. Aziende che avevano trattato i dati con leggerezza si ritrovarono davanti a multe pesanti e rischio legale. La lezione: ignorare le regole non è una scorciatoia; è una passività in attesa di essere attivata.

**Anni 2020: gli stessi vecchi errori, nuova tecnologia.** L'attuale ondata di IA ripete ognuno di questi errori a velocità. Strumenti economici e impressionanti rendono facile iniziare in grande, fidarsi troppo, saltare il lavoro sui dati, ignorare le regole e saltare la misurazione. La tecnologia è nuova; le modalità di fallimento sono vecchie e ben documentate. Conoscere la storia è la difesa più economica che esista.

L'arco: ogni generazione di tecnologia aziendale ha commesso lo stesso pugno di errori. Nessuno di essi è nuovo. Tutti sono evitabili se li hai già visti.

## Curiosità

### 24.7 L'effetto Eliza: perché ci fidiamo delle macchine più di quanto meritino

Una ragione per cui le persone si fidano troppo dell'IA risale a un programma di chat del 1966 chiamato ELIZA e all'abitudine umana che da esso prende il nome — l'**effetto Eliza**: concediamo volentieri comprensione e sentimenti a una macchina che si limita a imitarli, e ci fidiamo del suo output più di quanto meriti.

La storia completa di ELIZA, e perché conta per come progetti e supervisioni qualsiasi strumento IA, è raccontata nel [Capitolo 1 — Una breve storia dell'IA](ch01-a-short-history-of-ai.md), la casa canonica dell'effetto Eliza. Il richiamo in una riga qui: una macchina fluente ed educata ci fa fidare troppo di essa, e quell'abitudine è la radice dell'errore 24.3 qui sotto.

## Un esempio aziendale reale

*Il seguente è un composito illustrativo di comuni schemi del mondo reale, non una singola azienda con un nome.*

Un'azienda di vendita al dettaglio voleva "usare l'IA", così fece quasi tutto in questa lista nel modo sbagliato, e poi quasi tutto nel modo giusto.

La versione sbagliata: il titolare lesse dell'IA, si entusiasmò, e decise di "trasformare il servizio clienti". Senza scegliere un problema specifico, comprarono una chatbot e la distribuirono a tutta la base clienti in una volta. Le diedero in pasto un mucchio di documenti vecchi e disordinati e sperarono per il meglio. Disattivarono la revisione umana perché "l'IA è più veloce". Non controllarono mai se stesse dando risposte corrette. Nel giro di settimane, la chatbot stava dicendo con sicurezza ai clienti politiche di reso sbagliate e prezzi sbagliati. I clienti si lamentarono. L'azienda non ne aveva idea finché le lamentele non si accumularono. Il progetto fu un disastro, e il titolare concluse: "L'IA non funziona."

La versione giusta: dopo il disastro, il titolare ripartì con disciplina. Scelsero un piccolo problema chiaro — rispondere alle dieci domande "dov'è il mio ordine?" più comuni, che stavano mangiando tempo al personale. Controllarono prima i dati e trovarono che avevano dati di tracciamento ordini puliti che potevano rispondere a quelle domande in modo affidabile. Iniziarono con un minuscolo pilota solo su quelle domande, con un umano che revisionava ogni risposta. Misurarono il risultato: il tempo di risposta scese, la soddisfazione tenne, e le risposte erano corrette perché i dati erano buoni e l'ambito era ristretto. Solo allora si espansero, passo dopo passo, mantenendo la revisione umana sui casi più difficili.

La tecnologia era la stessa. Il primo tentativo fallì per sei errori. Il secondo funzionò perché ogni errore fu evitato. La lezione non è "l'IA è rischiosa". La lezione è "gli errori sono il rischio, e sono evitabili".

## Come si fa

### 24.1 Automatizzare il processo sbagliato

L'errore più costoso è spendere denaro per automatizzare qualcosa che non è mai valsa la pena automatizzare. Un processo sbagliato veloce è comunque sbagliato, e ora è sbagliato su scala.

**Perché accade.** Entusiasmo. Hai uno strumento e vuoi usarlo, così lo punti su qualunque cosa hai davanti invece di scegliere con cura. Oppure automatizzi un processo che va già bene, risparmiando tempo che nessuno doveva risparmiare, mentre il vero collo di bottiglia resta intatto.

**Cosa costa.** Denaro speso per uno strumento che consegna poco, più il costo opportunità del vero problema che non hai risolto. Peggio, un'automazione scelta male può peggiorare le cose — automatizzare un processo rotto produce solo output rotto più velocemente e nasconde la rottura.

**La soluzione: scegli prima di comprare.** Prima di qualsiasi strumento, scegli il processo con due test. Primo, *impatto*: questo processo conta davvero? Costa tempo reale, denaro reale o felicità reale dei clienti? Secondo, *adattamento*: il processo è adatto all'automazione — ripetitivo, a regole o a esempi, con dati disponibili? La matrice impatto-verso-facilità nel [Capitolo 12 — Dove l'IA può aiutare il tuo business](ch12-where-ai-can-help-your-business.md) è lo strumento per questo. Usala. Scegli l'obiettivo ad alto impatto e alto adattamento, non la prima cosa a cui hai pensato.

**Sistema il processo prima di automatizzarlo.** Se un processo è rotto, sistemalo prima, poi automatizza la versione sistemata. Automatizzare un disastro ti dà un disastro automatizzato. A volte il miglior primo passo è semplificare o rimuovere un passo del tutto, non automatizzarlo.

### 24.2 Sottovalutare dati e persone

L'IA gira su due cose: dati e persone. Entrambe sono di solito più difficili e più importanti del modello stesso, ed entrambe sono di routine sottovalutate.

**L'errore dei dati.** L'IA è buona solo quanto i dati che le dai. Dati disordinati, incompleti, obsoleti o di parte producono output disordinato, incompleto, obsoleto o di parte — non importa quanto buono è lo strumento. Le persone immaginano che l'IA "capirà" da qualunque cosa abbiano. Non può. Se i tuoi archivi sono un disastro, l'IA eredita il disastro. Il trattamento completo della qualità dei dati è nel [Capitolo 14 — Dati: la materia prima](ch14-data-the-raw-material.md). La versione breve: controlla i tuoi dati prima di aspettarti un buon output, e sistema i dati prima di dare la colpa all'IA.

**L'errore delle persone.** Come mostra il Capitolo 15, uno strumento che funziona in un test può restare inutilizzato perché nessuno è stato detto perché esiste, nessuno è stato formato, e nessuno si sentiva al sicuro. Le persone non sono una nota a margine; sono la ragione per cui i progetti vivono o muoiono. Sottovalutare il lato delle persone — la formazione, la paura, la fiducia, la gestione del cambiamento — è una delle cause più comuni di fallimento. Le competenze di gestione del cambiamento sono nel [Capitolo 21](ch21-managing-change-in-your-company.md). Metti a budget il lavoro sulle persone con la stessa serietà con cui metti a budget il software.

**Perché accade.** Sia il lavoro sui dati che quello sulle persone sono lenti, poco glamour e noiosi rispetto all'entusiasmante strumento. È tentatore saltarli e arrivare alla demo. Ma saltarli significa saltare le fondamenta. L'edificio cade.

**La soluzione.** Tratta dati e persone come il progetto principale, con lo strumento come una parte di esso, non il contrario. Dedica tempo reale a pulire e controllare i dati. Dedica tempo reale a formare, comunicare e sostenere le persone. Questi non sono costi generali; sono il lavoro.

### 24.3 Fidarsi troppo dell'IA

L'IA moderna produce output fluente, sicuro e ben scritto. Quella fluidità ci inganna facendoci fidare più di quanto meriti. Questo è il bias dell'automazione, ed è il singolo errore più pericoloso nella lista, perché trasforma uno strumento in un decisore non sorvegliato.

**Perché accade.** Una risposta sicura e ben scritta *sembra* corretta. I nostri cervelli confondono "suona bene" con "è vero". Aggiungi l'effetto Eliza — la nostra abitudine di concedere comprensione a una macchina educata — ed è facile smettere di controllare. Se lo strumento ha ragione il 95% delle volte, il 5% in cui ha ragione scivola via perché nessuno sta guardando.

**Cosa costa.** Risposte sbagliate che raggiungono i clienti. Cifre sbagliate nei report. Decisioni sbagliate prese su output sicuro-ma-falso. Il danno è peggiore proprio perché l'output sembrava affidabile, così nessuno l'ha messo in discussione finché non era troppo tardi. Ricorda la lezione dal Capitolo 1: la fluidità non è verità.

**La soluzione: mantieni l'umano nel ciclo.** Non lasciare mai che l'output dell'IA esca non revisionato, specialmente verso i clienti o in decisioni che contano. Metti una regola ferrea: l'IA prepara bozze, un umano controlla e invia. Insegna alle persone *come* controllare — cosa cercare, che aspetto ha una risposta sbagliata — non solo a premere un pulsante. La competenza di revisione è più importante dello strumento.

**Fai attenzione alla sciocchezza sicura.** L'IA può essere sicura nel sbagliare. Più l'output è sicuro e fluente, più dovresti controllarlo con attenzione, non meno. Allena il tuo istinto a diffidare delle risposte lisce sulle cose che contano. La mentalità trustless nel [Capitolo 7 — Trustless: fidarsi senza fidare](ch07-trustless-trust-without-trusting.md) è la cornice giusta: verifica, non fidarti per default.

**Metti regole di escalation.** Decidi cosa l'IA può fare da sola e cosa deve andare a un umano. Casi ad alto rischio, insoliti o ambigui vanno a una persona. L'IA gestisce la routine; l'umano gestisce l'importante e lo strano.

### 24.4 Iniziare troppo in grande

La distribuzione big-bang — cambiare tutto in una volta su un grande piano — è un fallimento classico. È tentatore perché sembra ambizioso, ma è il modo più sicuro di perdere il controllo.

**Perché accade.** Ambizione e impazienza. Vuoi la grande trasformazione ora, così vai largo e veloce. O vuoi impressionare, così scegli l'ambito più grandioso possibile. Il grande sembra audace; in pratica è fragile.

**Cosa costa.** I progetti grandi sono difficili da controllare, costosi da correggere quando vanno male, e lenti a mostrare valore. Un difetto che sarebbe piccolo in un pilota diventa una crisi quando è moltiplicato per tutta l'azienda prima che tu lo veda. I progetti big-bang spesso sforano il budget e i tempi, e molti falliscono del tutto.

**La soluzione: inizia piccolo e prova il valore.** Scegli un singolo compito ristretto, un team, un obiettivo chiaro. Fai un pilota. Misuralo. Se funziona, scala a passi (Capitolo 23). Piccolo non è timido; piccolo è come impari a basso costo e mantieni il controllo. Ogni piccola vittoria costruisce la competenza e l'evidenza per il passo successivo. L'approccio delle vittorie ristrette è lo stesso che il Capitolo 1 raccomanda dalla storia: l'IA vince una cosa specifica alla volta, e così dovresti fare tu.

**L'ambizione va bene; la sequenziazione è la disciplina.** Puoi avere una grande visione. Raggiungila solo attraverso una catena di piccoli passi provati, non un singolo salto gigante. La destinazione può essere grande; il primo passo deve essere piccolo.

### 24.5 Ignorare regolamenti e sicurezza

L'IA tocca i tuoi dati, i dati dei tuoi clienti e le tue decisioni. Questo significa che tocca la legge e la tua sicurezza. Ignorare entrambi non è una scorciatoia; è una passività armata.

**Perché accade.** Regolamenti e sicurezza sembrano lenti, complessi e lontani — finché non lo sono. È tentatore muoversi veloci e occuparsi della conformità "più tardi". Il "più tardi" spesso arriva come una multa, una violazione o una causa legale.

**Cosa costa.** Multe pesanti per violare le regole sulla privacy. Una violazione di dati che espone le informazioni dei clienti e distrugge la fiducia. Responsabilità legale per decisioni prese dall'IA che hanno violato una regola. Il costo di ignorare queste cose è di gran lunga più grande del costo di gestirle come si deve, e arriva tutto in una volta.

**La soluzione: conosci le regole che si applicano a te.** Se gestisci dati personali in o sull'Europa, il GDPR si applica — trattato nel [Capitolo 10 — Privacy e GDPR](ch10-privacy-and-gdpr.md). Se il tuo uso di IA ricade sotto l'AI Act europeo, si applicano i suoi doveri — trattati nel [Capitolo 5 — Regole e responsabilità legale](ch05-rules-and-legal-responsibility.md). Non devi essere un avvocato, ma devi sapere quali regole ti toccano e seguirle. Chiedi consulenza dove conta.

**Prendi la sul serio la sicurezza dal primo giorno.** Gli strumenti IA spesso gestiscono dati sensibili. Tratta quei dati con la stessa cura che useresti per contanti in una cassaforte. Le minacce alla sicurezza specifiche dell'era IA — perdite di dati, prompt injection, esposizione del fornitore — sono trattate nel [Capitolo 6 — La cybersecurity nell'era dell'IA](ch06-cybersecurity-in-the-ai-era.md). Non aggiungere la sicurezza dopo; costruiscila dentro dall'inizio.

**La conformità non è opzionale e non è un traguardo.** Le regole cambiano, e il tuo uso di IA cambia. La conformità è continua, come la manutenzione. Costruiscila nel modo in cui operi, non in un controllo una tantum che salti.

### 24.6 Non misurare i risultati

Se non misuri, non puoi dire se l'IA ha aiutato, danneggiato, o non ha fatto nulla. Stai guidando al buio, e continuerai a spendere denaro su qualcosa che non puoi valutare.

**Perché accade.** Misurare sembra lavoro extra, e può mostrare cattive notizie. È più facile dare per scontato che stia funzionando che controllarlo. Molti progetti partono con entusiasmo e non guardano più un numero.

**Cosa costa.** Non puoi provare il valore, così non puoi prendere buone decisioni sull'espandere o fermarti. Continui a spendere su cose che potrebbero non funzionare. Perdi la lezione che renderebbe migliore il progetto successivo. Un progetto che non hai mai misurato è un progetto il cui esito era casuale.

**La soluzione: misura dall'inizio.** Metti una linea di base prima di lanciare, traccia alcuni KPI onesti, e rivedili regolarmente. Il metodo completo è nel [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md) e la pratica della dashboard è nel [Capitolo 22 — Misurare risultati e ROI](ch22-measuring-results-and-roi.md). Non reimpararla qui; impegnati solo a farla. Misura la verità, incluse le settimane cattive, e usala per decidere tenere, correggere o fermare.

**Misura le cose che contano, non quelle che lusingano.** Evita metriche di vanità come i conteggi di utilizzo. Misura tempo, errori, costo e soddisfazione. Un numero che mostra solo il lato buono è un numero che ti sta mentendo.

## Etica e responsabilità

Ogni errore in questa lista ha un bordo etico, perché ognuno può ferire persone reali — clienti, dipendenti, o l'azienda stessa.

**Fidarsi troppo dell'IA è un fallimento etico, non solo pratico.** Quando output IA non revisionato raggiunge un cliente ed è sbagliato, hai danneggiato qualcuno. Resti responsabile di ciò che la tua IA invia, non importa quanto sicuro suonasse. Mantenere l'umano nel ciclo è un dovere, non una preferenza.

**Ignorare i regolamenti è un dovere che devi alle persone, non una casella da spuntare.** Le regole sulla privacy esistono per proteggere le informazioni di persone reali. Seguirle è rispettare quelle persone, non evitare una multa. La multa è la minima parte; il danno alla persona di cui hai malgestito i dati è il punto.

**Non misurare è un fallimento di onestà.** Se non puoi dire se la tua IA funziona, non puoi dire onestamente ai tuoi clienti, al tuo personale o ai tuoi partner cosa stai facendo. La misurazione è parte dell'essere veritieri sul proprio business.

**Iniziare troppo in grande può ferire la tua stessa gente.** Un progetto big-bang fallito spreca il denaro dell'azienda e la fiducia e lo sforzo del team. Un'ambizione che ignora il percorso sicuro può danneggiare le stesse persone che stai cercando di aiutare. Proteggile andando in passi sicuri.

**Il filo comune: resta sveglio e resta responsabile.** Ogni errore qui è una forma di sonnambulismo — fare la cosa facile invece di quella attenta. La posizione etica è la posizione sveglia: scegli il processo deliberatamente, rispetta i dati e le persone, verifica l'output, vai in passi sicuri, segui le regole, e misura la verità.

## Errori da evitare

Questo capitolo *è* la lista degli errori, quindi invece di ripeterla, ecco il meta-errore che nasconde tutti gli altri:

**Il meta-errore: trattare l'IA come un prodotto che compri invece che come un cambiamento che gestisci.** Tutti i sei errori derivano dalla stessa radice — trattare l'IA come un acquisto che funziona da solo, piuttosto che un cambiamento che ha bisogno di essere scelto, preparato, supervisionato e misurato. Quando compri uno strumento e ti aspetti che consegni da sé, scivoli in ogni trappola insieme: processo sbagliato, dati cattivi, fiducia cieca, troppo grande, nessuna regola, nessuna misurazione.

**La soluzione al meta-errore: tratta l'IA come un cambiamento gestito.** Scegli l'obiettivo di proposito. Prepara i dati e le persone. Supervisiona l'output. Inizia piccolo e scala con un piano. Segui le regole. Misura il risultato. Questo è tutto il libro in una frase, ed è l'opposto del sonnambulismo che causa ogni fallimento qui.

Un secondo meta-errore che vale la pena nominare: **concludere "l'IA non funziona" da un progetto fallito.** Quando un progetto fallisce, la causa era quasi sempre uno dei sei errori, non la tecnologia. Non gettare via l'opportunità perché hai messo il piede su una mina. Impara quale mina era, evitala la prossima volta, e riprova con disciplina. Gli strumenti funzionano quando eviti gli errori.

## Esercizio pratico

### 24.8 Esercizio: audita il tuo piano contro i sei errori

Prendi un qualsiasi progetto IA che stai pianificando o gestendo, e auditalo contro i sei errori. Per ciascuno, rispondi onestamente con un sì/no e una riga di evidenza.

**1. Processo sbagliato?** "Ho scelto questo obiettivo per impatto e adattamento, non solo per entusiasmo?" Se no, torna indietro e usa il test impatto-verso-facilità (Capitolo 12).

**2. Dati e persone sottovalutati?** "I miei dati sono abbastanza puliti, e ho messo a budget tempo reale per formazione e cambiamento?" Se no, sistema i dati e pianifica il lavoro sulle persone prima di andare oltre.

**3. Ti sei fidato troppo dell'IA?** "C'è una revisione umana su tutto ciò che conta, e le persone sanno che aspetto ha una risposta sbagliata?" Se no, aggiungi la regola di revisione ora, prima che esca altro output.

**4. Iniziato troppo in grande?** "Sto iniziando con un singolo compito ristretto e un team, o vado largo?" Se largo, restringi a un pilota e prova il valore prima.

**5. Regolamenti e sicurezza ignorati?** "So quali regole si applicano a me, e i dati sono protetti?" Se incerto, informati e correggi prima di gestire altri dati sensibili.

**6. Non misurare?** "Ho una linea di base e alcuni KPI onesti che guardo davvero?" Se no, impostali ora, anche se devi ricostruire la linea di base.

Per ogni "no", scrivi una concreta azione per correggerlo, con una data. Non andare avanti sul progetto finché le risposte "no" non sono corrette. Questa audizione di dieci minuti prende la maggior parte degli errori costosi prima che ti costino. Conserva le risposte e ricontrollale alla tua data di revisione.

## Checklist

### 24.9 Checklist anti-errore

Esegui questa contro qualsiasi progetto IA prima e durante.

- [ ] **Hai scelto l'obiettivo per impatto e adattamento**, non per entusiasmo o abitudine.
- [ ] **Hai sistemato o semplificato il processo prima di automatizzarlo.**
- [ ] **Hai controllato la qualità dei dati** e sistemato i dati prima di aspettarti un buon output.
- [ ] **Hai messo a budget tempo e denaro reali per il lato delle persone** — formazione, comunicazione, cambiamento.
- [ ] **Mantieni una revisione umana su tutto ciò che conta** — l'IA prepara bozze, un umano invia.
- [ ] **Hai formato le persone a riconoscere output sbagliato**, non solo a premere pulsanti.
- [ ] **Tratti l'output sicuro e fluente con diffidenza** e verifichi ciò che conta.
- [ ] **Hai impostato regole di escalation** — routine all'IA, importante e strano a un umano.
- [ ] **Hai iniziato piccolo** — un singolo compito ristretto, un team, un obiettivo chiaro.
- [ ] **Scali a passi** con un piano, non una distribuzione big-bang.
- [ ] **Sai quali regolamenti si applicano a te** (GDPR, AI Act UE) e li segui.
- [ ] **Proteggi i dati sensibili** con vera sicurezza dal primo giorno, non aggiunta dopo.
- [ ] **Tratti la conformità come continua**, non un controllo una tantum.
- [ ] **Hai misurato una linea di base** prima del lancio.
- [ ] **Tracci KPI onesti** (tempo, errori, costo, soddisfazione), non metriche di vanità.
- [ ] **Rivedi i numeri regolarmente** e li usi per decidere tenere / correggere / fermare.
- [ ] **Tratti l'IA come un cambiamento gestito**, non un prodotto che consegna da sé.
- [ ] **Non hai concluso "l'IA non funziona"** da un errore che era tuo da evitare.

Se una casella è vuota, sei in piedi su una mina. Aggirala prima di spendere più denaro o fiducia. Ogni errore in questa lista è vecchio, comune ed evitabile — una volta che sai che è lì.

## Punti chiave

- La maggior parte dei fallimenti IA viene da sei errori vecchi e prevedibili — processo sbagliato, dati e persone deboli, troppa fiducia, troppo grande, regole e sicurezza ignorate, nessuna misurazione — e tutti sono evitabili una volta conosciuti.
- Il singolo errore più pericoloso è fidarsi troppo dell'output fluente dell'IA; mantieni una revisione umana su tutto ciò che conta, perché la fluidità non è verità.
- La radice di ogni errore è trattare l'IA come un prodotto che compri invece che un cambiamento che gestisci — scegli, prepara, supervisiona, scala a passi, segui le regole, e misura.
- Inizia piccolo e prova il valore prima di andare largo; una vittoria ristretta che puoi controllare batte una grande distribuzione che non puoi.
- Non concludere "l'IA non funziona" da un progetto fallito — nomina quale errore l'ha causato, correggilo, e riprova con disciplina.
