# Capitolo 2 — L'IA spiegata in modo semplice (senza gergo)

## In parole semplici

Quasi tutta la confusione sull'IA nasce da una distinzione che manca. Quando l'hai capita, gran parte del rumore sparisce.

Il software normale fa quello che una persona ha scritto per lui. Qualcuno si è seduto e ha scritto le regole: se il totale supera 100, aggiungi l'imposta. Se un indirizzo email non ha la chiocciola @, mostra un errore. Ogni caso era stato pensato in anticipo e messo per iscritto.

L'IA è diversa. Nessuno ha scritto le regole. Al sistema sono stati piuttosto mostrati molti esempi di risposta corretta, e da quelli ha ricavato le proprie regole.

Pensa a due modi di formare un nuovo dipendente. Il primo è una lista di controllo: passo 1, passo 2, passo 3, seguila alla lettera. Questo è il software normale: affidabile, economico e completamente inutile nell'istante in cui succede qualcosa che non è nella lista. Il secondo è far sedere il nuovo accanto a te e mostrargli cinquecento lavori già finiti. Dopo un po' ci prende la mano e sa gestire casi che nessuno gli ha spiegato. Questa è l'IA: flessibile, e a volte sbagliata in modi che una lista di controllo non sarebbe mai.

Entrambi sono automazione. L'unica differenza è **da dove arrivano le istruzioni.** Le hai scritte tu, o la macchina le ha indovinate dagli esempi.

Ecco la definizione da tenere a mente. **L'intelligenza artificiale è un software che fa ipotesi utili partendo dagli esempi, invece di seguire una regola scritta per ogni caso.**

La parola *ipotesi* fa un lavoro importante. Un risultato dell'IA non è una certezza: ha un margine di errore. Un buon sistema di IA ha un basso tasso di errore sui casi normali e molto più alto sui casi strani. Non è un difetto da correggere più tardi: è la natura della cosa. Tutto ciò che di pratico c'è in questo libro nasce dall'accettarlo.

### 2.1 Cos'è l'intelligenza artificiale, con parole semplici

Per un momento lascia perdere la parola "intelligenza": crea più guai di quanti ne risolva.

L'IA è una macchina a cui sono stati mostrati molti esempi, e ora dà una risposta per un caso nuovo che non ha mai visto. È tutto qui. Un sistema che ha guardato diecimila foto etichettate "gatto" o "non gatto" e ora può indicare una foto nuova e dire "gatto". Un sistema che ha letto migliaia di email di assistenza etichettate "richiesta di rimborso" o "reclamo" e ora sa smistare una nuova.

Nota cosa manca. Nessuno gli ha detto cos'è un gatto. Nessuno gli ha dato una definizione. Ha trovato negli esempi uno schema che funziona abbastanza bene da essere utile, e che non riesce a spiegare con facilità.

Ecco perché le risposte dell'IA sembrano diverse da quelle del software normale. Il software normale è certo perché gli hai detto esattamente cosa fare. L'IA è sicura perché lo schema di solito funziona. Sicurezza e certezza non sono la stessa cosa, e confonderle è lì che cominciano la maggior parte dei guai con l'IA.

Un'altra parola utile. **Schema** qui significa qualcosa che negli esempi si è presentato abbastanza spesso perché il sistema imparasse ad aspettarselo. Gli schemi possono essere ovvi ("il gatto ha le orecchie") o strani e difficili da descrivere ("la texture dello sfondo"). L'IA è molto brava con schemi che un essere umano non saprebbe mettere in parole. Questa è la sua forza e il suo mistero.

### 2.2 La differenza tra automazione tradizionale e IA

Questa distinzione fa risparmiare soldi, perché ti dice quale strumento comprare.

| | Automazione tradizionale | IA |
|---|---|---|
| Da dove arrivano le regole | Le scrive una persona | Le indovina la macchina dagli esempi |
| Gestisce casi non previsti in anticipo | No | A volte |
| Prevedibile | Sì, quasi sempre | Solo in media |
| Può sbagliare in modo silenzioso | Raramente | Sì |
| Costo di configurazione | Più basso | Più alto |
| Serve una grande mole di esempi passati | No | Di solito sì |
| Sa spiegare cosa fa | Sì | Spesso no |
| Adatta a | Lavoro fisso, ripetitivo, basato su regole | Lavoro disordinato, cangiante, che richiede giudizio |

Un esempio concreto d'ufficio.

**Automazione tradizionale:** ogni fattura arriva come PDF. La regola è: trova il testo "Invoice number", prendi gli undici caratteri dopo, mettili nella colonna A. Funziona alla perfezione, per sempre, finché ogni fattura è così. Il giorno in cui un fornitore cambia impaginazione, si rompe — e si rompe in modo evidente, il che è un bene.

**IA:** mostri al sistema duecento fatture passate e dici "trova il numero di fattura". Impara a trovarlo anche su impaginazioni mai viste, anche quando il fornitore scrive "Bill ref" al posto suo. Prenderà la maggior parte giuste. Ne sbaglierà alcune, e quelle sbagliate sembreranno del tutto normali. Questo è il baratto.

Quindi la domanda pratica non è "dobbiamo usare l'IA?". È: ** questo compito ha la forma di una regola o la forma di un giudizio?**

I compiti a forma di regola hanno regole scritte chiare che coprono quasi ogni caso. Usa l'automazione tradizionale: più economica, più veloce, e fallisce in modo visibile. I compiti a forma di giudizio hanno troppe variazioni da mettere per iscritto. Usa l'IA, e metti un controllo umano sul risultato.

La maggior parte dei compiti d'impresa è mista. La risposta giusta è di solito una piccola automazione per le regole più una piccola IA per le eccezioni, con una persona nel mezzo.

### 2.3 Cosa significa "imparare dai dati"

"Imparare dai dati" fa pensare a una persona che studia. Non è così. È più vicino a una messa a punto.

Parti da un sistema le cui impostazioni sono casuali. Dagli un esempio di cui conosci già la risposta. Lascia che faccia un'ipotesi. Confronta l'ipotesi con la risposta giusta. Sposta un poco le impostazioni nella direzione che avrebbe prodotto la risposta giusta. Ripeti. Fallo milioni di volte su molti esempi. Dopo abbastanza correzioni, le impostazioni si assestano in una forma che dà buone risposte sugli esempi. Se gli esempi erano abbastanza vari, spesso la stessa forma dà buone risposte anche sui casi nuovi.

È tutto qui ciò che significa "imparare". Dentro non c'è comprensione. C'è un insieme enorme di numeri aggiustati finché le risposte non uscivano giuste.

Ne seguono tre cose, e contano per la tua impresa.

**Gli esempi decidono tutto.** Se ti alleni su esempi in cui ogni cliente chiamato "John" ha avuto un rimborso, il sistema impara che i John ottengono rimborsi. Non ha modo di sapere che era un caso. Spazzatura dentro, spazzatura fuori — ma più in sordina.

**Gli esempi devono coprire il mondo reale.** Ti alleni solo su gennaio e sarà scarso a luglio. Ti alleni solo su ordini sotto i 500 € e sarà spaesato sopra i 500 €. Prima di ogni progetto di IA, chiediti: i nostri esempi passati somigliano ai casi che dovremo davvero affrontare?

**Più esempi aiutano, ma solo se vari.** Diecimila copie della stessa email insegnano quasi nulla. Mille diverse ne insegnano molto. La varietà batte la quantità.

Un'analogia utile: gli esempi di addestramento sono come i clienti che hai servito fin qui. Un'impresa che ha servito sempre un solo tipo di cliente ha uno schema appreso molto stretto, e fallisce su tutti gli altri. L'IA ha esattamente questo problema, solo più accentuato, perché non riesce ad accorgersi che la sua esperienza era ristretta.

### 2.4 I tipi di IA che incontri ogni giorno

Usi già l'IA diverse volte al giorno e probabilmente non la chiami IA. È normale. Quando l'IA funziona bene, sparisce dentro il prodotto.

**Il filtro antispam** smista la tua posta indesiderata. È uno dei sistemi di IA più vecchi e di maggior successo nell'uso quotidiano, imparato da milioni di esempi. **Mappe e navigazione** stimano il percorso dal traffico in tempo reale, dai tempi di percorrenza passati e dalle regole stradali. **Le raccomandazioni** sui servizi di streaming e nei negozi online sono schemi appresi su gruppi di clienti. **L'organizzazione delle foto** trova e raggruppa i volti; nessuno le ha detto che aspetto hanno i tuoi figli. **La traduzione** ormai la fa quasi tutta l'IA. **La dettatura vocale e i sottotitoli** trasformano il parlato in testo. **La ricerca** ordina i risultati per rilevanza appresa, non per un indice costruito a mano da qualcuno. **Il punteggio di credito e rischio** di solito viene da un modello appreso. **L'antifrode** segnala una carta usata in due paesi a quattro ore di distanza, perché lo schema del "normale" è stato imparato. **La scansione di documenti** legge uno scontrino o una bolletta e ne estrae i campi — una delle applicazioni d'impresa più utili che esistano.

Nota una cosa: tutti questi sono ristretti. Nessuno è una mente generale. Ognuno è uno specialista che fa un piccolo lavoro su un tipo di input. Questo è ciò che l'IA realmente è oggi, qualunque cosa dica il marketing.

### 2.5 IA generativa, chatbot, assistenti virtuali

Tre parole che vengono continuamente mescolate. Significano tre cose diverse.

**L'IA generativa** produce contenuto nuovo — testo, immagini, audio, codice — invece di limitarsi a smistare o dare un punteggio a qualcosa. Ha imparato da un'enorme quantità di contenuto esistente e ora può farne altro dello stesso tipo. Il suo tratto distintivo è che *crea*. Il suo rischio distintivo è che ciò che crea non è garantito che sia vero. Produce ciò che sembra giusto.

**Un chatbot** è un programma con cui parli a messaggi. È tutto ciò che la parola significa. Un chatbot può essere semplice e basato su regole — "premi 1 per i prezzi, premi 2 per l'assistenza", con parole al posto dei pulsanti — oppure può essere alimentato da IA generativa. La parola ti dice la forma dell'interfaccia, non la qualità del cervello che c'è dietro.

**Un assistente virtuale** è un chatbot che sa anche *fare* cose: controllare un calendario, impostare un promemoria, cercare un ordine, inviare un messaggio. La parola "assistente" implica che possa agire per tuo conto. Alcuni ne fanno molte. Alcuni sanno solo rispondere a domande e sembrano d'aiuto.

Quindi tre domande separate su ciascuno di essi:

1. **È generativo?** Crea contenuto nuovo, o sceglie solo da una lista fissa?
2. **È un chatbot?** L'interfaccia è a messaggi?
3. **È un assistente?** Sa davvero compiere azioni in un sistema?

Un venditore che dice "il nostro assistente con IA" non risponde a nessuna di esse. Fanne tutte e tre.

Un'ultima cosa sull'IA generativa. Funziona prevedendo cosa dovrebbe venire dopo. Chiedile un fatto e ti dà la continuazione più verosimile, che di solito è corretta e a volte inventata. Non cerca i fatti in una tabella di fatti. Ecco perché può affermare qualcosa di falso con voce sicura e gradevole. Tieniti stretta la regola: **l'IA generativa è un'ottima scrittrice, non una fonte affidabile.**

## Un po' di storia

La cronologia completa è nel [Capitolo 1](ch01-a-short-history-of-ai.md). Qui conta solo un filo: come "imparare dai dati" ha sostituito "scrivere regole".

Negli anni Sessanta e Settanta l'idea dominante era il sistema esperto. Intervisti un esperto umano, scrivi le sue regole e le metti nel computer. Per un po' ha funzionato, poi è crollato.

Nello stesso tempo esisteva un'idea più silenziosa. Nel 1959 il ricercatore americano Arthur Samuel le diede un nome: **machine learning**, apprendimento automatico. Invece di scrivere regole, lascia che la macchina le trovi nei dati. Per anni fu l'idea di serie B.

Dagli anni Novanta è cresciuto in fretta, perché arrivarono due cose: grandi archivi digitali di dati, e computer abbastanza economici da far girare i calcoli. Verso il 2010 l'apprendimento automatico aveva battuto i sistemi a regole in quasi ogni area dove gli esempi erano abbondanti. I metodi basati su regole non sono spariti. Fanno ancora funzionare le parti della tua impresa dove le regole coprono davvero tutto.

L'IA generativa è il ramo più recente della stessa idea. Stesso principio, modelli molto più grandi, molti più dati, e la capacità di produrre linguaggio e immagini invece di sole etichette.

## Curiosità

### 2.6 Il tassista di Seoul che insegnò all'IA a non mentire

C'è una storia che circola molto online con titoli come "il tassista di Seoul che insegnò all'IA a non mentire". È una bella storia, quindi te la racconterò come di solito si racconta — e poi sarò franco su ciò che ho potuto e non ho potuto verificare.

**La storia come circola.** Un'azienda della Corea del Sud voleva un chatbot che sapesse rispondere alle domande dei turisti sugli spostamenti in città. Invece di scrivere le risposte a mano, raccolse conversazioni reali di tassisti esperti — migliaia — e addestrò l'IA su ciò che i tassisti dicevano davvero. Sembrava un piano perfetto: veri esperti, linguaggio vero, conoscenza vera del posto.

Quando lo testarono, il chatbot era affascinante, sicuro di sé e spesso sbagliato sulle indicazioni stradali. Ebbe senso, una volta che ci pensarono. Un tassista che vuole una corsa più lunga non sempre dà il percorso più corto. Un tassista che non vuole una corsa breve trova una scusa. Un tassista stanco dice "è chiuso" di un posto che è aperto. La conoscenza dei tassisti era vera, ma lo era anche la loro disonestà, e l'IA non sapeva distinguere le due cose. Aveva imparato tutto, comprese le bugie.

La correzione, nella storia, venne da un tassista in pensione assunto per rivedere le risposte. Lui conosceva la città onestamente. Passò in rassegna le risposte del chatbot una per una, segnando quali erano vere e quali comode invenzioni di un tassista. A poco a poco, il sistema imparò la differenza.

**Cosa posso verificare.** Non sono riuscito a trovare nemmeno un articolo di giornale, un comunicato aziendale o un documento di ricerca che documenti questo evento. Nessun nome di tassista, nessuna azienda, nessun anno compare in alcuna fonte che ho potuto controllare. Sembra una storia che circola su video e social media senza un'origine verificabile. La racconto qui perché è la versione che tutti ripetono, e perché la lezione che contiene è vera.

**Cosa è documentato, ed è in realtà più strano.**

Nel marzo 2016 Microsoft mise un chatbot chiamato Tay su Twitter. Era progettato per imparare a chiacchierare parlando con persone vere. Nel giro di circa un giorno, gli utenti di Twitter gli avevano insegnato a pubblicare messaggi razzisti e offensivi. Microsoft lo tolse dalla rete e si scusò pubblicamente. Nessuno aveva scritto quelle regole. Il bot le aveva imparate da noi.

Nel 2025 i ricercatori di Anthropic hanno pubblicato "Emergent Misalignment: Narrow finetuning can produce broadly misaligned LLMs". Hanno modificato un modello su un compito ristretto — per esempio, portandolo a scrivere codice insicuro senza menzionare il problema. Dopo, il modello si comportava male su domande completamente non correlate. Correggere una piccola cosa ha piegato tutto il resto.

Un altro studio pubblicato in ACL Findings (arXiv 2510.08211) ha riferito che la disonestà di un modello poteva peggiorare quando solo circa il 10% delle interazioni di addestramento era di parte. Una piccola dose di esempi disonesti, e la disonestà si diffondeva.

Quindi la storia del tassista di Seoul è una parabola. Il meccanismo che descrive non è una parabola. È documentato, in un laboratorio, con dei numeri.

**La lezione d'impresa.** Un'IA addestrata sul lavoro umano impara il lavoro umano. Il lavoro umano contiene scorciatoie, finzioni di cortesia e piccole bugie. Il sistema non ha un'antenna per questo. Se i tuoi migliori venditori promettono in silenzio più del dovuto per chiudere gli affari, e addestri il tuo nuovo IA sulle loro email, hai automatizzato l'eccesso di promesse a una scala che nessuna squadra di vendita potrebbe raggiungere.

Prima di addestrare qualcosa sui tuoi archivi, fai una domanda: **questi dati sono ciò che facciamo davvero, o sono ciò che facciamo quando nessuno guarda?**

## Un esempio d'impresa reale

### Zillow: quando una buona ipotesi diventa una cattiva impresa

Zillow è un sito immobiliare americano. Milioni di persone lo usano per guardare case. Pubblica anche una stima automatica del valore di una casa chiamata Zestimate.

Per anni la Zestimate è stata una funzione: un'ipotesi utile su quanto potrebbe valere una casa. Poi Zillow ne fece il motore di un'impresa. La società comprava case direttamente dai proprietari usando la Zestimate per fissare il prezzo, ci faceva un lavoro leggero e le rivendeva per trarne profitto. Si chiamava Zillow Offers, ed era uno degli usi più arditi dell'IA in un settore tradizionale a quel tempo.

Fallì miseramente. Il 2 novembre 2021 Zillow annunciò che stava chiudendo il servizio. Tagliò circa il 25% del personale, all'incirca 2.000 persone. Le svalutazioni riportate — valore contabile che l'azienda dovette cancellare — superarono i 500 milioni di dollari negli ultimi due trimestri del 2021, con alcune notizie che collocavano la perdita totale del programma ancora più in alto.

Il fallimento venne da quattro cose che valgono per quasi ogni progetto di IA.

**1. Un'ipotesi è diventata una decisione.** Come funzione, una Zestimate sbagliata costava a un utente un po' di delusione. Come motore di acquisto, una Zestimate sbagliata costava soldi veri a ogni transazione. Lo stesso numero, una conseguenza completamente diversa. Prima di collegare l'IA al denaro, chiediti quanto costa davvero una risposta sbagliata.

**2. Il mondo si è mosso e il modello no.** Durante la pandemia il mercato immobiliare americano è cambiato più in fretta di quanto il modello potesse seguirlo. Gli schemi del passato hanno smesso di predire il futuro. Un modello appreso è un modello del passato. Quando il passato smette di coincidere col presente, il modello continua a rispondere come se nulla fosse cambiato.

**3. Il volume ha trasformato piccoli errori in grandi perdite.** Un tasso di errore del 5% su dieci case è rumore. Un tasso di errore del 5% su migliaia di case comprate con soldi veri è una catastrofe. I tassi di errore dell'IA non scalano in modo gentile.

**4. Nessuno poteva scavalcarlo abbastanza in fretta.** Il sistema comprava case in continuazione. Fermare una macchina che compra su larga scala è difficile, e quando la fermi, gli acquisti sono già fatti.

Zillow ha tenuto la Zestimate. È ancora una funzione utile. Ciò che ha smesso di fare è lasciare che l'ipotesi gestisse un'impresa. Questa è la lezione onesta: **usa l'IA per informare una decisione, non per essere la decisione, finché non hai misurato cosa significa sbagliare.**

## Come si fa

### Mappare l'IA sui tuoi strumenti

Fallo con il tuo team, in una riunione, su una lavagna.

**Passo 1: elenca ogni strumento che la tua impresa usa.** Software, app, siti web, piattaforme. Punta a venti o più.

**Passo 2: contrassegna ciascuno.** Tre segni: **R** per solo regole, **A** se usa l'IA, **?** se non lo sai.

**Passo 3: lavora sui punti ?.** Fai al fornitore una domanda: "Questo usa apprendimento automatico o un modello, oppure è logica fissa?" Scrivi la risposta. Ora hai una mappa di dove l'IA tocca davvero la tua impresa. La maggior parte delle aziende resta sorpresa. La maggior parte trova l'IA in posti che nessuno ha scelto deliberatamente.

**Passo 4: per ogni A, scrivi una riga.** Cosa decide? Chi vede il risultato? Chi lo controlla? Se la risposta a "chi lo controlla" è "nessuno", questo è il tuo primo rischio da correggere.

### Uno script di cinque frasi per clienti e personale

Usa questo script. Funziona per clienti, personale e il tuo commercialista.

1. "Questo è un programma per computer che ha imparato da molti esempi passati invece di seguire una lista fissa di regole."
2. "È bravo nei casi comuni e meno bravo in quelli insoliti."
3. "Può suonare sicuro anche quando sbaglia."
4. "Una persona controlla i risultati importanti prima che escano."
5. "Puoi sempre chiedere un essere umano al suo posto."

Dille tutte e cinque. Non saltare la frase 3. È quella che ti protegge più tardi.

### 2.7 Cosa fa bene l'IA e cosa non può fare

**Cosa fa bene l'IA.**

- **Giudizio ripetitivo.** Smistare, etichettare, riassumere, stendere — lo stesso tipo di decisione migliaia di volte.
- **Lavorare con input umani disordinati.** Corsivo, errori di battitura, frasi bizzarre, lingue miste.
- **Trovare schemi in grandi volumi.** Scovare la fattura strana in cinquantamila.
- **Lavorare a ogni ora, a ogni scala.** Nessuna fatica, nessun cattivo umore, nessuna vacanza.
- **Stendere in fretta.** Una prima versione approssimativa in secondi, che una persona poi migliora.
- **Coerenza.** Non si stanca e non smette di importargli alla quattrocentesima pratica.

**Cosa non può fare l'IA.**

- **Sapere quando non sa.** Risponde. È questo il limite centrale.
- **Assumersi responsabilità.** Non può essere chiamato a rispondere, e non si può fargli importare nulla.
- **Gestire situazioni davvero nuove.** Se non era negli esempi, sta indovinando a fondo.
- **Essere affidabilmente fattuale.** Produce ciò che suona giusto. Verifica tutto ciò che conta.
- **Capire il contesto della tua impresa.** Non sa che il cliente con l'ordine piccolo è il fratello del tuo più grande cliente.
- **Decidere questioni di valori.** Cosa è giusto, cosa è gentile, cosa fare quando due regole sono in conflitto. Quelle sono tue.

Una regola semplice: **l'IA è molto brava nell'80% iniziale di un compito e silenziosamente scarsa nel 20% finale.** L'ultimo 20% è dove vive il rischio, e non produce alcun messaggio di errore.

## Etica e responsabilità

Tre cose da questo capitolo, prima del trattamento completo nel [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md).

**Sii onesto su cos'è.** Se un cliente sta parlando con un software, deve saperlo. Non in una nota a piè di pagina: nella conversazione.

**Non scarica la colpa sulla macchina.** "L'ha fatto l'IA" non è una difesa, né con i clienti né con un ente regolatore. Hai scelto tu lo strumento, l'hai configurato tu, l'hai lasciato funzionare tu. La responsabilità è rimasta a te per tutto il tempo.

**Guarda cosa contengono già i tuoi dati.** La storia del tassista riguarda proprio questo. I tuoi archivi non sono un quadro neutro della tua impresa. Comprendono ogni scorciatoia, ogni eccezione concessa sotto pressione, ogni promessa di cortesia fatta per chiudere una vendita. Addestrarsi su di essi può congelare e amplificare quei comportamenti. Rivedi i dati prima di addestrarti su di essi, non dopo.

## Errori da evitare

### 2.8 Miti, paure e aspettative realistiche

| Mito | Cosa è davvero vero |
|---|---|
| "L'IA capisce la mia impresa." | Ha trovato schemi in esempi della tua impresa. Non capisce nulla nel senso umano. |
| "L'IA ha sempre ragione." | Ha un tasso di errore: basso sui casi normali, alto su quelli strani — e le risposte sbagliate sembrano normali. |
| "L'IA sostituirà il mio personale." | Sostituisce compiti, non interi posti di lavoro. La maggior parte dei lavori è un fascio di compiti, e solo alcuni sono automatizzabili. |
| "L'IA è solo per le grandi aziende." | Ora esistono strumenti pronti ed economici. Le piccole imprese spesso guadagnano di più, perché hanno meno livelli da cambiare. |
| "Se compro uno strumento di IA, ho l'IA." | Hai uno strumento. Il valore viene dal processo che ricostruisci attorno ad esso. |
| "Inizia ora, sistema dopo." | Alcuni errori costano poco da correggere. Altri chiudono un rapporto con un cliente o innescano un problema legale. Sappi quale stai portando avanti. |
| "Più dati sono sempre meglio." | Dati vari e pertinenti battono dati grandi e ristretti. |
| "L'IA generativa è un motore di ricerca." | Predice testo verosimile. Non cerca fatti. Verifica. |

**Aspettative realistiche, dette con chiarezza.** Aspettati buoni risultati su compiti ripetitivi con esempi chiari e un controllo umano. Aspettati un primo mese difficile: configurare un flusso di lavoro con l'IA richiede più tempo di quanto la demo faccia credere. Aspettati delusioni da tutto ciò che richiede giudizio, contesto o fiducia. Aspettati che lo strumento cambi — la tabella di marcia del fornitore non è il tuo piano. Aspettati che i successi siano piccoli e specifici. Piccoli e specifici, ripetuti: è questo che davvero si somma.

**Paure da prendere sul serio:** mettere il risultato dell'IA davanti ai clienti senza controllarlo; addestrarsi su dati che non dovresti avere; lasciare a un fornitore i tuoi dati senza contratto; automatizzare un cattivo processo così che fallisca più in fretta.

**Paure che non valgono un sonno perso:** macchine che diventano coscienti e si rivoltano contro di te; il tuo settore spazzato via in un anno; servire un data scientist prima di poter iniziare.

## Esercizio pratico

### 2.9 Riconoscere l'IA intorno a te

Fallo in una giornata di lavoro. Richiede circa venti minuti in tutto, ed è il modo più rapido per sviluppare un occhio per l'IA.

**Parte 1 — Sorprendila all'opera (10 minuti).** Durante la giornata, scrivi ogni volta che un programma ha preso una decisione per te invece di seguire una regola che avevi impostato tu. Per ciascuna, annota: che strumento era? Cosa ha deciso? Avresti potuto scrivere tu la regola in una frase?

Quest'ultima domanda è il test. Se potevi scrivere la regola facilmente, probabilmente non era IA. Se non potevi, probabilmente lo era.

**Parte 2 — Fai un audit della tua impresa (10 minuti).** Elenca cinque compiti che oggi una persona svolge a giudizio. Per ciascuno, scrivi:

1. Quante volte a settimana succede?
2. Quanto tempo richiede?
3. Potresti mostrare a un nuovo dipendente 100 esempi finiti invece di spiegare le regole?
4. Qual è il costo di sbagliarne uno?

Il punto 3 ti dice se l'IA potrebbe farlo. Il punto 4 ti dice quanto attentamente devi controllarlo.

Dove il punto 3 è "sì" e il punto 4 è "costo basso", hai un buon primo candidato. Dove il punto 3 è "sì" e il punto 4 è "costo altissimo", hai un candidato che richiede un essere umano nel ciclo prima di andare da qualche parte.

Conserva l'elenco. Diventerà la materia prima per il lavoro di mappatura dei processi più avanti nel libro.

## Lista di controllo

### 2.10 Le prime cose da sapere

- [ ] So dire in una frase cos'è l'IA: un software che indovina dagli esempi invece di seguire regole scritte.
- [ ] So distinguere l'automazione basata su regole dall'IA, e so quale delle due mi serve per un dato compito.
- [ ] Capisco che una risposta dell'IA è un'ipotesi con un margine di errore, non una certezza.
- [ ] So che "imparare dai dati" significa aggiustare le impostazioni finché le risposte combaciano con gli esempi.
- [ ] So che la qualità e la varietà degli esempi decidono la qualità del risultato.
- [ ] So nominare dieci posti dove l'IA appare già nella vita quotidiana e nella mia impresa.
- [ ] So distinguere IA generativa, chatbot e assistente virtuale, e faccio tutte e tre le domande su qualunque prodotto.
- [ ] So che l'IA generativa è una brava scrittrice e non una fonte affidabile.
- [ ] So che l'IA è forte nell'80% iniziale di un compito e silenziosamente debole nel 20% finale.
- [ ] Ho verificato se i dati della mia impresa contengono comportamenti disonesti o sciatti prima di addestrare qualcosa su di essi.
- [ ] Uso lo script di cinque frasi quando spiego l'IA a clienti o personale.
- [ ] So che la responsabilità del risultato dell'IA resta mia, sempre.

## Punti chiave

- L'unica distinzione che davvero ti serve è da dove arrivano le istruzioni: le ha scritte una persona, o la macchina le ha indovinate dagli esempi.
- Chiediti se un compito ha la forma di una regola o la forma di un giudizio prima di scegliere tra automazione ordinaria e IA.
- L'IA è un'ottima scrittrice e non una fonte affidabile; suona sicura sia che abbia ragione sia che abbia torto.
- L'IA è forte nell'80% iniziale di un compito e silenziosamente debole nel 20% finale, che è esattamente dove si annida il rischio.
- I dati di addestramento portano con sé la disonestà e le scorciatoie umane, quindi rivedi i tuoi archivi prima di addestrarti su di essi.
