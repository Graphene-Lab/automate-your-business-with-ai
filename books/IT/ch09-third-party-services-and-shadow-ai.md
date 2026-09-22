# Capitolo 9 — Servizi di terze parti e shadow AI

## In parole semplici

Un servizio di AI di terze parti è qualsiasi AI che usi e che funziona sui computer di qualcun altro. Tu digiti una domanda o carichi un file. Questo viaggia su internet fino ai loro computer. Il loro software fa il lavoro. La risposta torna indietro. Tu non vedi mai cosa c'è dentro.

È il modo in cui quasi tutte le aziende usano l'AI oggi. È facile, costa poco iniziare ed è potente. Per questo la usano praticamente tutti.

Ma ha anche un costo nascosto. Nel momento in cui il tuo testo esce dal tuo edificio, ne perdi il controllo diretto. Ora dipendi da un'azienda che non hai progettato tu, da regole che non hai scritto tu, da un server che non puoi ispezionare.

La "shadow AI" è la seconda metà di questa storia. Shadow AI significa che i dipendenti usano strumenti di AI senza che l'azienda lo sappia, lo approvi o lo controlli. Un assistente del marketing incolla un elenco di clienti in una chatbot gratuita. Un contabile carica una fattura in un'app web per riassumerla. Chi comanda non sa che sta succedendo. I dati sono partiti, e non c'è traccia, né contratto, né controllo.

Pensa alla fotocopiatrice d'ufficio di vent'anni fa. La usavano tutti. Nessuno sapeva che conservava una copia di ogni pagina. La shadow AI è la stessa sorpresa, solo che le pagine sono i tuoi elenchi clienti, i tuoi contratti e i tuoi prezzi.

Questo capitolo parla di due cose: cosa succede davvero ai tuoi dati quando usi un servizio di terze parti, e come impedire che il tuo stesso personale crei rischi in silenzio. Il modello opposto — far funzionare l'AI sui tuoi computer — è trattato nel [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md). Il lato legale dei dati personali è l'argomento centrale del [Capitolo 10](ch10-privacy-and-gdpr.md). La domanda più ampia sul controllo dei propri strumenti è nel [Capitolo 11](ch11-digital-sovereignty.md).

## Un po' di storia

**Anni '90 e 2000: il software esce dallo scaffale.** Prima compravi un programma su un CD e lo facevi girare sul tuo computer. Poi la posta, i calendari e l'archiviazione dei file si sono spostati su internet. Hai smesso di possedere il software e hai iniziato ad affittarne l'accesso.

**Anni 2000–2015: il SaaS diventa la normalità.** "Software as a Service" significava pagare una quota mensile per usare il software di qualcun altro via web. Salesforce, Google Workspace e Microsoft 365 lo hanno reso ordinario. La comodità ha vinto. La maggior parte delle piccole imprese ha smesso di gestire i propri server.

**2016–2022: i dati seguono il software.** Una volta che i tuoi archivi clienti, i documenti e i messaggi hanno vissuto nel cloud di un fornitore, i dati della tua azienda sono stati fuori dalle tue mura in modo permanente. Quasi tutti lo hanno accettato perché gli strumenti erano validi e il prezzo basso.

**Novembre 2022: ChatGPT apre la porta a tutti.** Un'AI potente è diventata disponibile in una scatola web gratuita. Non serviva più un contratto con un fornitore per usare l'AI. Serviva solo un indirizzo email. È il momento in cui la shadow AI è cominciata, perché un singolo dipendente poteva ormai inviare dati aziendali a un modello all'avanguardia senza chiedere a nessuno.

**2023: i primi allarmi in azienda.** Le aziende hanno scoperto che il personale incollava materiale riservato nelle chatbot pubbliche. Il caso Samsung, nella sezione Curiosità, è il più noto. Diverse banche e studi professionali quell'anno hanno vietato o limitato gli strumenti di AI pubblici.

**2023–2026: i fornitori aggiungono i piani "enterprise".** In risposta, i fornitori di AI hanno venduto piani business che promettevano di non addestrarsi sui tuoi dati, di tenerli separati e di aggiungere controlli amministrativi. La comodità è rimasta; le promesse sono migliorate. Ma una promessa non è la stessa cosa che avere il controllo, ed è per questo che questo capitolo conta.

## Curiosità

### 9.7 L'azienda di semiconduttori che incollò i suoi segreti in ChatGPT

All'inizio del 2023, Samsung Electronics — una delle più grandi aziende tecnologiche al mondo — scoprì che i suoi stessi ingegneri avevano inserito materiale riservato in una chatbot AI pubblica.

Le segnalazioni, pubblicate per la prima volta dal quotidiano finanziario coreano *Korea Economic Daily* nell'aprile 2023 e poi riprese ampiamente, descrivevano tre distinti incidenti all'interno della divisione semiconduttori. Nel primo, un ingegnere incollò del codice sorgente difettoso di un programma usato per scaricare i dati di misura da una fabbrica di chip, sperando che la chatbot trovasse il bug. Nel secondo, il personale caricò codice legato alle apparecchiature per semiconduttori e al rilevamento dei difetti. Nel terzo, i dipendenti inserirono trascrizioni registrate di riunioni nello strumento per ottenerne riassunti. Tutto questo avvenne nell'arco di circa tre settimane da quando la divisione aveva iniziato a consentire l'accesso allo strumento.

Una volta che i dati erano dentro la chatbot, si trovavano su computer che Samsung non possedeva. L'azienda non poteva recuperarli facilmente, e non poteva essere certa che non venissero usati o visti da altri.

La risposta di Samsung fu netta. Vietò gli strumenti di AI generativa, ChatGPT compreso, sui computer, i tablet, i telefoni aziendali e sulla rete interna. Violare la regola poteva portare a provvedimenti disciplinari fino al licenziamento. Ai dipendenti che usavano tali strumenti su dispositivi personali fu detto di non inserire mai informazioni aziendali o dati personali che potessero rivelare la proprietà intellettuale di Samsung. Un'indagine interna rilevò che il 65% degli intervistati riteneva che i servizi di AI rappresentassero un rischio per la sicurezza. Al tempo stesso, Samsung dichiarò di stare costruendo strumenti di AI interni per la traduzione, il riassunto di documenti e lo sviluppo software, e di lavorare a modi per bloccare il caricamento di informazioni sensibili su servizi esterni.

La lezione non è che Samsung sia stata sconsiderata. È che se un'azienda con un budget di sicurezza di miliardi si è fatta sorprendere da una chatbot gratuita, una piccola impresa senza un team di sicurezza è ancora meno protetta. La comodità è reale, e reale è anche la perdita di dati.

## Un esempio di business reale

### L'agenzia che perse il suo elenco clienti due volte

Pensa a una piccola agenzia di marketing, venti persone, nessun reparto IT. È una storia composita, ma ogni sua parte accade ogni settimana in aziende vere.

Prima perdita: una senior account manager vuole riscrivere in fretta una proposta. Apre una chatbot AI gratuita sul portatile e incolla la bozza, che include il nome di un prodotto non ancora lanciato di un cliente, cifre di budget e recapiti. Ottiene un paragrafo più curato. Non pensa mai a dove sia finito il testo.

Seconda perdita: la stessa manager, un mese dopo, si iscrive a un "assistente di scrittura AI" a pagamento che promette risultati migliori. Per configurarlo, lo collega alla posta e all'unità condivisa dell'agenzia così che possa "imparare il tono dell'azienda". Ora il fornitore può leggere tutto: ogni cliente, ogni contratto, ogni battuta interna che diventa una nota strategica.

Poi arriva il problema dell'evoluzione. Un anno dopo il fornitore cambia piano. Le funzioni per cui pagava passano a un livello superiore. Il prezzo raddoppia. Il modello dietro lo strumento viene sostituito con uno più recente, e lo stile di scrittura su cui aveva formata il suo team cambia silenziosamente. Lei vuole andarsene, ma tutto è cablato in quello strumento. Cambiare significa ricollegare tutta l'agenzia da un'altra parte e riaddestrare tutti. Questa è la lock-in, ed è avvenuta senza una sola decisione sbagliata — solo una serie di scelte comode.

Nulla di tutto questo richiedeva cattiveria. Richiedeva comodità e l'assenza di una regola. La soluzione non è temere l'AI. È decidere, in anticipo, quali dati possono andare dove, e dare alle persone un buon strumento così che non ricorrano a uno rischioso.

## Come si fa

### 9.1 La comodità dei servizi cloud: perché li usano tutti

L'AI di terze parti è popolare per ragioni oneste, e dovresti nominarle prima di metterla in discussione.

Non c'è configurazione. Non compri hardware, non assumi un ingegnere, non installi nulla. Apri una pagina web e cominci. Per una piccola impresa senza personale tecnico, è tutto qui il suo fascino.

Non c'è costo iniziale. La maggior parte degli strumenti ha un livello gratuito o una bassa quota mensile. Puoi provare un'idea al prezzo di un caffè invece che con un acquisto di capitale.

La qualità è alta. I migliori modelli al mondo sono dietro questi servizi. Una ditta di due persone può usare la stessa capacità di una grande corporation.

Scala all'istante. Ti serve dieci volte tanto lavoro oggi? Le macchine del fornitore lo assorbono. Tu non fai nulla.

È per questo che l'AI cloud si è diffusa più velocemente di qualsiasi tecnologia prima di essa. Lo scopo di questo capitolo non è togliertela. È farti usarla a occhi aperti, perché ognuna di queste comodità si paga con un pezzo di controllo che non ti sei accorto di star vendendo.

### 9.2 Cosa succede ai tuoi dati quando lasciano l'azienda

Quando incolli testo in un'AI di terze parti, possono succedere diverse cose, e di solito non vedi quali.

I tuoi dati attraversano internet fino ai server del fornitore, spesso in un altro paese. Una volta lì, vengono archiviati, almeno per un po', su hardware che non controlli e non puoi ispezionare.

Potrebbero essere letti da sistemi automatici per il filtraggio di sicurezza. Potrebbero essere registrati per il debug. Personale di assistenza in un altro paese potrebbe vederli. Nulla di tutto questo è insolito; è così che operano i grandi servizi.

La cosa più importante: potrebbero essere usati per addestrare il modello del fornitore. "Addestrare" significa che l'azienda inserisce il tuo testo nel suo sistema così che il modello impari da esso. Se accade, un frammento del tuo testo riservato può influenzare le risposte date ad altri clienti. È la ragione numero uno per fare attenzione.

Alcuni piani business promettono di non addestrarsi sui tuoi dati. Quella promessa vale qualcosa, ma è una clausola contrattuale, non un muro. Ti fidi che il fornitore la rispetti in ogni prodotto e in ogni paese. La regola sicura è semplice: tratta qualsiasi AI di terze parti come se tutto ciò che invii potesse diventare pubblico. Se questo pensiero è inaccettabile per un certo file, non mandare quel file.

### 9.3 Il problema della trasparenza: non sai mai davvero come vengono usati i tuoi dati

Non puoi vedere dentro un servizio di AI di terze parti. È il problema centrale, e non sta sparendo.

Non sai quale modello ti ha risposto. I fornitori scambiano i modelli senza dirtelo. Non sai dove sono stati archiviati i tuoi dati, chi poteva accedervi, o per quanto tempo sono stati conservati. Non sai se un subappaltatore in un altro paese li ha elaborati. Non sai se sono stati usati per l'addestramento, anche quando credi di no.

L'informativa sulla privacy del fornitore è scritta da avvocati, non da ingegneri, e descrive cosa possono fare, non cosa faranno nel tuo caso specifico. Leggerla raramente dà una risposta chiara.

Per questo il test pratico è così utile. Invece di cercare di capire il sistema, fai una sola domanda sui dati: *sarebbe accettabile se questo diventasse pubblico domani?* Per un post pubblico sul blog, sì. Per il file degli stipendi di un cliente, no. Quel singolo test sostituisce mille domande a cui non puoi rispondere.

Se ti serve vera trasparenza, l'unica fonte onesta è un sistema che puoi ispezionare — il tuo computer, o un software aperto che qualcuno può verificare. È l'argomento del [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md) e del [Capitolo 11](ch11-digital-sovereignty.md).

### 9.4 Il problema dell'evoluzione: i modelli cambiano, i contratti cambiano, i prezzi cambiano

Un servizio di terze parti non è una cosa che compri; è una relazione che continua a cambiare sotto i tuoi piedi.

Il modello cambia. Lo strumento di oggi potrebbe girare su un modello diverso il trimestre prossimo. Le risposte cambiano. Lo stile cambia. Una cosa che funzionava bene nel tuo flusso di lavoro può peggiorare, o semplicemente diventare diversa, senza preavviso e senza modo di restare alla versione vecchia.

Il contratto cambia. Le condizioni a cui hai acconsentito all'iscrizione possono essere aggiornate. Le funzioni su cui contavi possono passare dietro un piano superiore. La promessa sui dati di addestramento può essere riformulata.

Il prezzo cambia. Uno strumento economico che ormai hai cablato nella tua azienda può alzare il prezzo, e ti trovi davanti a una scelta dolorosa: pagare di più, o strappare via tutto.

Questo è il rischio nascosto della comodità. Costruisci su un terreno che qualcun altro controlla, e loro possono muoverlo quando vogliono. La difesa è mantenere portabili i tuoi dati importanti e i tuoi flussi di lavoro essenziali, e non lasciare mai che un singolo fornitore diventi l'unico posto in cui il tuo lavoro può avvenire.

### 9.5 Lock-in: quanto è difficile cambiare fornitore dopo

La lock-in significa che lasciare un fornitore è così costoso, in tempo, denaro o disagi, che non puoi realisticamente farlo. Sei "bloccato".

Succede in tre modi. **Lock-in dei dati:** i tuoi dati sono archiviati in un formato che solo quel fornitore legge bene, o non riesci a esportarli in modo pulito. **Lock-in del flusso di lavoro:** il tuo processo quotidiano è costruito attorno a quello strumento, quindi cambiare significa riaddestrare tutti e ricostruire i modelli. **Lock-in dell'integrazione:** lo strumento è collegato alla tua posta, al tuo CRM, ai tuoi file, e tirarlo fuori rompe tutti quei collegamenti.

La lock-in dà al fornitore potere su di te. Loro sanno che andarsene è difficile, il che indebolisce la tua posizione quando alzano i prezzi o cambiano le condizioni.

Per restare libero, imponi tre cose fin dall'inizio. Primo, i tuoi dati devono essere esportabili in un formato semplice e comune. Secondo, tieni i tuoi dati principali da qualche parte che controlli tu, e lascia che il fornitore lavori su una copia. Terzo, progetta il tuo flusso di lavoro in modo che l'AI sia un passaggio, non l'intera macchina, così puoi sostituire il passaggio. L'obiettivo non è evitare i fornitori. È essere in grado di lasciarne uno in una settimana, non in un anno.

### 9.6 Shadow AI: quando i dipendenti usano strumenti non autorizzati

La shadow AI è il rischio che non puoi vedere, perché lo creano i tuoi stessi personale di fiducia.

Succede perché i buoni strumenti ufficiali sono lenti da approvare, mentre gli strumenti gratuiti rischiosi sono istantanei. Un dipendente sotto pressione temporale incolla l'email di un cliente in una chatbot gratuita per scrivere una risposta. Nessuno lo ferma, perché nessuno lo sa.

Perché è pericoloso: i dati partono senza contratto, senza verifica e senza traccia. Non puoi dirlo al cliente, non puoi ritrovare i dati dopo, e non puoi provare cosa è successo. Se lo strumento si addestra su quei dati, le tue informazioni riservate possono finire per influenzare un modello pubblico.

Come riconoscerla: addebiti insoliti sulle carte aziendali per abbonamenti di AI; personale che si lamenta che gli strumenti approvati sono troppo lenti; miglioramenti "magici" improvvisi nei risultati che nessuno strumento approvato spiega.

Come fermarla: non limitarti a vietare. Un divieto senza una buona alternativa spinge solo il comportamento in superficie... sotto terra. Dai alle persone uno strumento approvato che sia veloce e abbastanza buono, e lo useranno. Poi rendi la regola chiara, forma su di essa e monitora leggermente. Il lato completo delle policy è nella sezione 9.8 e nei modelli di policy AI aziendale nelle appendici del libro.

### 9.8 Come mitigare i rischi: due diligence, contratti, policy interna

Riduci il rischio con tre livelli. Falli tutti e tre.

**Livello 1: Due diligence — verifica prima di comprare.**
Prima di adottare un fornitore di AI, fai le domande difficili. Dove sono archiviati i dati, e in quali paesi? Vi addestrate sui dati dei clienti, e potete garantire per iscritto di non farlo? Chi può accedervi, subappaltatori inclusi? Per quanto tempo sono conservati, e come vengono cancellati? Sono cifrati in transito e a riposo? Quali certificazioni avete? Ottieni le risposte per iscritto, non in una call di vendita. Un fornitore che non sa rispondere chiaramente ti sta dicendo qualcosa. Una versione a punteggio di queste domande è nella scorecard di due diligence dei fornitori nelle appendici.

**Livello 2: Contratti — metti le promesse sulla carta.**
Una rassicurazione verbale non vale nulla. Nel contratto, richiedi: nessun addestramento sui tuoi dati; residenza dei dati in un paese che accetti; il diritto di esportare tutti i tuoi dati in un formato utilizzabile; il diritto alla cancellazione; il dovere di avvisarti in caso di violazioni e di grandi cambi di modello o di condizioni; e limiti sui subappaltatori. Se il fornitore non firma queste cose, quella è la tua risposta.

**Livello 3: Policy interna — di' alle tue persone le regole.**
Scrivi una policy AI breve e semplice. Dichiara quali strumenti sono approvati. Dichiara quali dati non devono mai entrare in un'AI esterna — dati personali dei clienti, registri finanziari, contratti, codice sorgente, password. Dai al personale uno strumento approvato e veloce così che non ricorra a uno rischioso. Forma tutti sulla regola in una breve sessione. Rivedi l'elenco degli strumenti approvati ogni trimestre. Un modello è nelle appendici.

L'ordine conta. Verifica prima, contratto secondo, policy terza. La maggior parte delle aziende salta i primi due e si chiede perché si è ritrovata esposta.

## Etica e responsabilità

L'AI di terze parti solleva un dovere che devi a due gruppi: le persone di cui detieni i dati, e il tuo stesso personale.

**Ai tuoi clienti e dipendenti.** Quando un cliente ti dà dati personali, si fida di te per proteggerli. Inviare quei dati a un'AI di terze parti che non hai verificato può rompere quella fiducia, anche se non succede nulla di male. Sei responsabile di dove finiscono i loro dati. I doveri legali sono esposti nel [Capitolo 10](ch10-privacy-and-gdpr.md); il principio etico è semplice — non mettere le informazioni private di qualcuno in un posto dove non metteresti le tue.

**Al tuo personale, sulla shadow AI.** Attenzione a non trasformare la protezione in sorveglianza. Se monitori l'uso dell'AI, di' alle persone cosa monitori e perché. Una regola chiara più un buon strumento è giusto. La sorveglianza segreta di personale di fiducia danneggia il morale e la fiducia. Punta a delle protezioni, non a uno stato di polizia.

**Sii onesto su ciò che non controlli.** Se un cliente chiede se i suoi dati addestrano un modello esterno, dovresti poter rispondere con verità. Se non lo sai, dillo, e correggi. Vantarsi di una sicurezza che non c'è è peggio che ammettere una lacuna.

## Errori da evitare

1. **Guardare la demo, non il flusso dei dati.** Una demo curata non ti dice nulla su dove vanno i tuoi dati. Fai prima le domande su archiviazione e addestramento.
2. **Fidarsi di un "non ci addestriamo sui tuoi dati" verbale.** Se non è nel contratto, non esiste.
3. **Collegare uno strumento a tutta la tua unità.** "Impara il nostro tono" spesso significa "leggi tutto". Dai allo strumento il minimo indispensabile.
4. **Vietare la shadow AI senza alternativa.** Un divieto senza un buon strumento approvato nasconde soltanto il comportamento.
5. **Nessuna policy scritta.** Se la regola non è scritta e insegnata, non è una regola.
6. **Ignorare la questione del paese.** Dati archiviati sotto un sistema legale diverso possono essere accessi in modo diverso. Sappi dove si trovano.
7. **Dare per scontato che un piano a pagamento equivalga a sicurezza.** Un piano consumer a pagamento non è la stessa cosa di un piano enterprise contrattuale con le giuste condizioni.
8. **Nessun piano di esportazione.** Se non riesci a far uscire i tuoi dati, sei bloccato dal primo giorno.
9. **Trattare l'informativa sulla privacy come una garanzia.** Elenca cosa possono fare, non cosa faranno per te.
10. **Dimenticare l'elemento umano.** La perdita quasi sempre comincia con una persona sotto pressione temporale. Elimina la pressione e offri un percorso sicuro.

## Esercizio pratico

### 9.9 Analizza i tuoi attuali fornitori di AI

Prendi un'ora e fallo per ogni strumento di AI che la tua azienda usa oggi, inclusi quelli che il personale usa in silenzio.

Fai una tabella. Una riga per strumento. Colonne:

- **Nome dello strumento** e chi lo ha attivato.
- **Quali dati entrano.** Sii specifico: email dei clienti, fatture, contratti, codice, testo pubblico.
- **Dove sono archiviati,** se lo sai. Se è ignoto, scrivi "ignoto".
- **Si addestrano sui nostri dati?** Sì / No / Non so.
- **C'è un contratto,** o solo un click di accettazione?
- **Possiamo esportare i nostri dati?** Sì / No / Non so.
- **Livello di rischio** per i dati che effettivamente ci metti: Basso / Medio / Alto.

Ora leggi le righe a rischio Alto. Per ciascuna, chiediti: sarebbe accettabile se questi dati diventassero pubblici? Se no, hai tre scelte — smettere di metterci quei dati, passare a un fornitore che firma le giuste condizioni, o spostare quel compito su uno strumento che controlli tu (vedi [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md)).

Infine, chiedi in giro. Manda un messaggio onesto al tuo team: "Quali strumenti di AI usate per lavoro di cui non abbiamo parlato?" Le risposte sono la tua vera lista di shadow AI. Non punire l'onestà; correggi le lacune che rivela.

## Checklist

### 9.10 Domande da fare a ogni fornitore di AI

Prima di mettere dati reali in un servizio di AI di terze parti, ottieni una risposta scritta a ognuna di queste.

- [ ] **Dove sono fisicamente archiviati i nostri dati,** e in quali paesi?
- [ ] **Vi addestrate i modelli sui nostri dati?** Puoi impegnarti al "no" nel contratto?
- [ ] **Chi può accedere ai nostri dati,** dipendenti e subappaltatori inclusi, e da dove?
- [ ] **Per quanto tempo conservate i nostri dati,** e come facciamo a farli cancellare?
- [ ] **I nostri dati sono cifrati** sia in transito che durante l'archiviazione?
- [ ] **Possiamo esportare tutti i nostri dati** in qualsiasi momento, in un formato comune e utilizzabile?
- [ ] **Ci avviserete** in caso di violazione dei dati, e entro quanto tempo?
- [ ] **Ci avviserete** prima di cambiare il modello, il prezzo o le condizioni?
- [ ] **Quali certificazioni di sicurezza** avete, e potete mostrarcele?
- [ ] **Ci sono subappaltatori,** e sono vincolati dalle stesse condizioni?
- [ ] **Qual è il nostro ricorso legale** se fate un uso improprio dei nostri dati?
- [ ] **C'è una console di amministrazione** così che possiamo vedere e controllare gli utilizzi?

Se un fornitore non sa rispondere a queste domande in modo chiaro e per iscritto, tratta lo strumento come ad alto rischio e tieni fuori i dati sensibili.

## Punti chiave

- Un servizio di AI di terze parti funziona sui computer di qualcun altro, quindi nel momento in cui i tuoi dati partono, scambi il controllo per comodità.
- Il rischio più grande è che i tuoi dati riservati possano essere usati per addestrare un modello che serve altri, e spesso non puoi vederlo né fermarlo.
- I fornitori cambiano modelli, contratti e prezzi sotto i tuoi piedi, e la lock-in rende costoso andarsene — quindi tieni i tuoi dati esportabili e il tuo flusso di lavoro sostituibile.
- La shadow AI è il tuo stesso personale che usa strumenti non approvati; fermala con un buon strumento approvato più una regola scritta chiara, non solo con divieti.
- Proteggiti su tre livelli: verifica prima il fornitore, metti le promesse in un contratto secondo, e definisci una policy interna terzo.
