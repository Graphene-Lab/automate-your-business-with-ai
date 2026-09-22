# Capitolo 26 — Vendite e marketing

## In parole semplici

Le vendite e il marketing sono dove l'IA può aiutarti a trovare più clienti, parlare con loro meglio, e spendere meno tempo a indovinare. Il lavoro qui è pieno di piccoli compiti ripetuti: smistare quali contatti vale la pena chiamare, scrivere email, rispondere alle stesse domande sul tuo sito web, e cercare di capire cosa vogliono i tuoi clienti. L'IA è brava in tutti.

L'idea centrale è la *personalizzazione su larga scala*. Un buon venditore ricorda ogni cliente, adatta il messaggio, e fa seguito al momento giusto. Un piccolo team non può farlo per migliaia di persone. L'IA sì. Può guardare ogni contatto e indovinare quanto è probabile che compri, scrivere un'email che sembra scritta per quella persona, rispondere alla domanda di un visitatore alle 2 di notte, e individuare quali clienti stanno per andarsene.

Questo capitolo copre quattro lavori: punteggiare i contatti (indovinare chi è più probabile che compri), scrivere email e contenuti, gestire chatbot e assistenti, e analizzare i clienti per capire cosa vogliono e chi è a rischio di andarsene.

Un avviso onesto prima di iniziare: l'IA è un potente amplificatore. Farà arrivare un buon messaggio a più persone, e farà arrivare un cattivo messaggio a più persone. Può anche spingerti verso lo spam — mandare troppo, troppo spesso, a persone che non l'hanno chiesto. L'obiettivo non è bombardare tutti; è raggiungere la persona giusta con il messaggio giusto al momento giusto. Il metodo per giudicare se tutto questo ripaga vive nel [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md); questo capitolo ti mostra cosa automatizzare e come.

## Un po' di storia

**Anni '90: marketing di massa e la mailing list.** L'automazione del marketing iniziò con semplici liste email. Un'azienda poteva mandare un messaggio a migliaia di persone in una volta. Era economico e ampio, ma grossolano — tutti ricevevano lo stesso messaggio, che stesse loro bene o no. Questa era l'era dello "spruzza e prega".

**Anni 2000: il CRM e il funnel.** Il software di Customer Relationship Management (CRM) — una banca dati di ogni cliente e ogni interazione — arrivò. I marketer cominciarono a pensare in un "funnel": molte persone entrano in cima, meno ne arrivano a un acquisto in fondo. Il CRM permetteva di tracciare dove ogni persona era nel funnel e fare seguito. I dati entrarono nel quadro.

**Anni 2010: segmentazione e personalizzazione.** Con più dati, i marketer impararono a dividere il loro pubblico in gruppi (segmenti) e mandare a ogni gruppo un messaggio diverso. "Le persone che hanno comprato X hanno anche comprato Y." La personalizzazione rese i messaggi più rilevanti ed efficaci. Ma era ancora per lo più basata su regole: se un cliente faceva questo, manda quello.

**Fine anni 2010: il machine learning punteggia i contatti.** Il machine learning — software che impara modelli da molti esempi — cominciò a punteggiare i contatti. Invece di una persona che indovinava chi chiamare per prima, il modello guardava centinaia di segnali (dimensione dell'azienda, quali pagine hanno visitato, come ti hanno trovato) e classificava i contatti per quanto erano probabili da comprare. I team di vendita smisero di sprecare tempo su contatti freddi.

**Anni 2020: l'IA generativa scrive e chatta.** I grandi modelli linguistici — IA addestrate su enormi quantità di testo — possono ora scrivere email, testi pubblicitari e descrizioni di prodotti che suonano umane. Chatbot costruiti sulla stessa tecnologia possono tenere una vera conversazione, rispondere a domande e guidare un cliente attraverso un acquisto. Il chatbot passò da una frustrante menu di pulsanti a qualcosa che capisce davvero cosa hai digitato.

**Ora: agenti che lavorano l'intero percorso.** Il passo più recente è l'agente — IA che porta a termine un compito attraverso vari passi. Un agente rivolto ai clienti può rispondere a una domanda, controllare lo stock e guidare un acquisto. Un agente interno può prendere una richiesta di supporto e creare il ticket. L'esempio di mobilezone qui sotto usa esattamente questo: due agenti, uno per i clienti e uno per il team interno.

L'arco: da un messaggio a tutti, a funnel tracciati, a segmenti, a contatti punteggiati, a IA che scrive e chatta. Ogni passo rese il marketing più personale e meno un gioco d'indovinello.

## Curiosità

### 26.5 Il chatbot che divenne due agenti

Quando mobilezone, un rivenditore svizzero di telecomunicazioni, sostituì il suo vecchio chatbot, non costruì un bot migliore. Costruì due agenti diversi per due lavori diversi: uno rivolto ai clienti, uno rivolto al proprio personale. Quella divisione è l'idea interessante. La stessa tecnologia di IA servì due pubblici in due modi molto diversi — una guida amichevole per lo shopping sul sito web, e un aiutante per scrivere ticket dentro l'azienda. La storia, con i numeri reali, è qui sotto.

## Un esempio reale di business

**mobilezone: due agenti Copilot, uno per i clienti e uno per l'IT.**

mobilezone è un rivenditore svizzero di telecomunicazioni con più di 125 negozi fisici, che vende telefoni, piani e dispositivi connessi. Aveva due problemi separati. Lato clienti, il suo vecchio chatbot del sito web era rigido e frustrante — poteva solo seguire una menu fissa e spesso falliva nel rispondere a domande reali. Dentro l'azienda, il personale doveva compilare moduli scomodi per segnalare problemi IT, il che rallentava tutti.

Secondo uno studio di caso cliente Microsoft pubblicato, mobilezone ricostruì entrambi i lati usando Microsoft Copilot Studio — uno strumento per costruire agenti di IA conversazionali — insieme a Dynamics 365 (il suo CRM) e la Power Platform (gli strumenti di automazione low-code di Microsoft). Costruì due agenti:

- **Mia — l'agente rivolto ai clienti.** Mia è un'assistente multilingue sul sito web. Risponde alle domande ad alto volume dei clienti, aiuta i visitatori a trovare il prodotto o il piano giusto, e li guida attraverso un acquisto. Perché capisce il linguaggio naturale, gestisce le domande che il vecchio bot a menu non poteva.
- **Supporto — l'agente IT interno.** Supporto è un aiutante per il personale di mobilezone stesso. Invece di compilare un modulo rigido, un dipendente dice a Supporto cosa è rotto in parole semplici, e l'agente crea il ticket IT automaticamente.

I risultati riportati: gli agenti ora gestiscono **più di 1.600 chat al mese**, e l'agente IT interno ha **tagliato il tempo di risoluzione IT di circa il 50%**. Importante altrettanto, gli agenti hanno ridotto il carico sul contact center esterno di mobilezone (il supporto telefonico in appalto), e l'agente clienti ha migliorato la conversione online guidando gli acquirenti nella scoperta dei prodotti.

Due lezioni spiccano. Primo, la stessa tecnologia servì due lavori molto diversi — vendite esterne e supporto interno — il che mostra quanto flessibili siano questi agenti. Secondo, mobilezone non sostituì gli umani; spostò le conversazioni facili e ripetitive all'agente così la sua gente poteva concentrarsi su quelle più difficili. Questa è la promessa realistica: l'IA gestisce il volume, gli umani gestiscono il valore.

Una nota sulla fonte: le cifre sopra provengono dalla storia cliente Microsoft pubblicata su mobilezone. Trattale come i risultati riportati da mobilezone; i tuoi numeri dipenderanno dal tuo volume e configurazione.

## Come si fa

### 26.1 Punteggiatura dei contatti

Un *contatto* è una persona o azienda che ha mostrato un po' di interesse — ha compilato un modulo, scaricato qualcosa, o fatto una domanda. Non hai tempo di chiamare ogni contatto con lo stesso impegno. Punteggiare i contatti significa classificarli per quanto sono probabili da comprare, così il tuo team chiama i più caldi per primi.

**Come l'IA punteggia un contatto.** Un modello di machine learning guarda molti segnali insieme: la dimensione dell'azienda del contatto, il titolo di lavoro della persona, quali pagine hanno visitato, quante volte sono tornati, se hanno aperto le tue email, e come ti hanno trovato. Dagli affari passati che si sono chiusi, il modello impara quali segnali vanno insieme a una vendita, e punteggia ogni nuovo contatto di conseguenza.

**Perché batte l'indovinare.** Una persona che punteggia i contatti a intuito è lenta e di parte — tende a favorire i contatti che "sembrano" amichevoli, non quelli che davvero convertono. L'IA punteggia in modo coerente e veloce, e può ponderare centinaia di segnali che una persona non può tenere in testa.

**Inizia semplice.** Non ti serve un modello perfetto il primo giorno. Inizia con pochi segnali chiari — dimensione dell'azienda, ruolo, e cosa hanno scaricato — e punteggia i contatti a mano nel tuo CRM. Man mano che raccogli più affari chiusi, un vero modello può imparare da essi e migliorare.

**Alimenta il ciclo.** Il modello migliora quando gli dici quali contatti sono davvero diventati clienti. Assicurati che il tuo CRM registri l'esito di ogni affare, così la punteggiatura impara da risultati reali, non da indovinelli.

**Non fidarti troppo del punteggio.** Un punteggio è un indizio, non un verdetto. Un punteggio alto significa "chiama presto", non "vendita garantita". Un punteggio basso potrebbe comunque essere un buon cliente che il modello non ha ancora imparato. Usa il punteggio per impostare la priorità, non per ignorare le persone.

### 26.2 Email e contenuti

Scrivere email, testi pubblicitari e descrizioni di prodotti richiede ore. L'IA generativa — IA che produce testo — può redigerle velocemente, e una persona può modificarle per farle suonare bene.

**Redigi, non spedire.** Usa l'IA per produrre una prima bozza, poi modificala. L'IA è eccellente nel mettere parole sulla pagina velocemente e terribile nel conoscere la tua voce esatta, il tuo marchio e i sentimenti del tuo cliente senza guida. La bozza è al 70%; la tua modifica è l'ultimo 30% che la rende tua.

**Personalizza su larga scala.** L'IA può prendere un modello e adattarlo per molte persone: inserire il nome del destinatario, riferirsi a ciò che hanno guardato, adattare l'offerta al loro segmento. Questa è l'idea di personalizzazione su larga scala di prima — un messaggio che sembra scritto per una persona, mandato a migliaia.

**Abbina il canale.** Un'email, un post social e una pagina prodotto hanno bisogno di lunghezze e toni diversi. Dì all'IA il canale e l'obiettivo, e modifica di conseguenza. Una email lunga non funziona come tweet; un tweet non funziona come landing page.

**Mantieni la voce umana.** Il testo dell'IA può suonare piatto, generico o troppo zelante. Leggi ogni bozza ad alta voce. Se non suona come qualcosa che diresti, riscrivilo. I tuoi clienti capiscono quando un messaggio è generico.

**Non lasciare mai che l'IA mandi senza revisione.** Un'email IA non revisionata può contenere un prezzo sbagliato, un nome sbagliato, o una riga inappropriata. Fai sempre leggere a un umano prima che esca. Questa è la stessa regola della finanza: l'IA redige, l'umano approva.

**Vigila sul volume.** L'IA rende facile mandare più email di quante dovresti. Di più non è meglio. Mandare troppo a persone che non l'hanno chiesto è spam, e brucia la tua lista e la tua reputazione. Mandane meno, ma fai contare ogni una.

### 26.3 Chatbot e assistenti

Un chatbot è un programma che parla con un cliente sul tuo sito web o app. I chatbot moderni, costruiti su grandi modelli linguistici, capiscono cosa una persona digita e rispondono in linguaggio semplice — un enorme passo avanti rispetto alle vecchie menu "premi 1 per le vendite".

**Cosa fa un buon chatbot.** Risponde istantaneamente alle domande comuni (prezzo, orari, spedizione, resi), guida un visitatore al prodotto giusto, cattura i dettagli di contatto per un follow-up, e passa a un umano quando non può aiutare. Il passaggio è critico: un chatbot che non passa mai frustra le persone e perde vendite.

**Progetta prima il passaggio.** Prima di costruire il bot, decidi quando dovrebbe passare la conversazione a una persona. Quando il bot è incerto, quando il cliente chiede un umano, quando l'argomento è sensibile — passa. Un bot che conosce i propri limiti è fidato; uno che bluffa no.

**Formalo sulle tue vere domande.** Dai al bot le domande che i clienti davvero fanno, con le risposte che vuoi. Più conosce i tuoi prodotti e le tue politiche specifiche, più è utile. Un bot generico dà risposte generiche che frustrano.

**Lascialo parlare molte lingue.** Uno dei più grandi vantaggi di un chatbot moderno è il supporto multilingue. Può rispondere a un cliente nella propria lingua senza che tu assuma traduttori. Questo è esattamente ciò che fa Mia di mobilezone.

**Misura cosa gestisce e cosa fallisce.** Traccia quante conversazioni il bot risolve da solo, quante ne passa, e cosa non ha potuto rispondere. I fallimenti sono oro — ti dicono cosa insegnargli dopo. (Le stesse idee di chatbot, applicate al supporto anziché alle vendite, sono trattate nel [Capitolo 27 — Assistenza e supporto clienti](ch27-customer-care-and-support.md).)

### 26.4 Analisi dei clienti

Analisi dei clienti significa usare i dati per capire chi sono i tuoi clienti, cosa vogliono, e chi sta per andarsene. L'IA è forte qui perché può vedere modelli attraverso migliaia di clienti che nessuna persona potrebbe individuare a mano.

**Segmenta i tuoi clienti.** L'IA può raggruppare i clienti per comportamento: acquirenti frequenti, grandi spendaccioni, acquirenti stagionali, clienti a rischio. Ogni gruppo ha bisogno di un messaggio diverso. Questa è la segmentazione, e l'IA la fa più velocemente e più accuratamente delle regole manuali.

**Individua l'abbandono prima che accada.** L'*abbandono* significa che un cliente smette di comprare. L'IA può guardare segnali — meno visite, ordini più piccoli, meno coinvolgimento — e segnalare clienti che probabilmente se ne andranno presto. Questo ti dà tempo di riconquistarli con un'offerta o una chiamata personale, invece di scoprirlo dopo che sono andati.

**Trova la prossima migliore offerta.** L'IA può guardare cosa un cliente ha comprato e suggerire cosa probabilmente vorrà dopo. "Ha comprato un telefono, probabilmente gli serve una custodia e un'assicurazione." Questa è l'idea del motore di raccomandazioni, e alza il valore di ogni cliente.

**Leggi cosa dicono i clienti.** L'IA può leggere recensioni, commenti di sondaggi e chat di supporto ed estrarre i temi principali: cosa la gente ama, cosa la infastidisce, cosa chiede. Invece di leggere mille commenti uno per uno, ottieni un riassunto dei temi grandi. Questo trasforma il feedback grezzo in qualcosa su cui puoi agire.

**Non trattare le persone come punti dati.** L'analisi è uno strumento per servire meglio i clienti, non per manipolarli. Usa ciò che impari per rendere migliore la loro esperienza, non per sfruttare le loro debolezze. Il confine tra personalizzazione e manipolazione è reale, e dovresti restare dalla parte giusta.

## Etica e responsabilità

Le vendite e il marketing toccano direttamente l'attenzione e la fiducia delle persone, quindi il confine etico conta.

**Non fare spam.** L'IA rende facile mandare troppo. Mandare messaggi a persone che non l'hanno chiesto, o più di quanto hanno accettato, è spam. Rispetta il consenso e la frequenza. Una corta lista di persone che vogliono i tuoi messaggi batte un'enorme lista che bombardi.

**Sii onesto nei testi scritti dall'IA.** L'IA può scrivere un'affermazione che suona vera ma non lo è. Controlla ogni affermazione fattuale — prezzo, funzionalità, risultati — prima che esca. Non lasciare mai che l'IA inventi un beneficio che non puoi fornire.

**Divulga quando è un bot.** In molti luoghi, e come buona pratica, un cliente dovrebbe sapere che sta parlando con un chatbot e non con una persona. Rendi il passaggio a un umano facile e chiaro.

**Rispetta la privacy.** L'analisi dei clienti usa dati personali. Segui le regole per gestirli — le basi sono nel [Capitolo 10 — Privacy e GDPR](ch10-privacy-and-gdpr.md). Raccogli solo ciò che ti serve, di' alle persone cosa raccogli, e tienilo sicuro.

**Non manipolare.** La personalizzazione dovrebbe aiutare le persone a trovare ciò che vogliono, non spingerle in un acquisto di cui si pentiranno. Evita i dark pattern — trucchi che fanno pressione sulle persone. Costruisci fiducia, non una trappola.

**Tieni un umano nel ciclo.** L'IA redige l'email, la pubblicità, la risposta. Un umano la rivede prima che raggiunga un cliente. Questa singola regola previene la maggior parte dei danni.

## Errori da evitare

**Fare spam con l'IA.** Usare il potere dello strumento per mandare più di quanto le persone vogliono. Mandane meno, fallo contare.

**Spedire testi IA non revisionati.** Un prezzo sbagliato o un'affermazione falsa in un'email scritta dall'IA danneggia la fiducia. Rivedi sempre.

**Un chatbot che non passa mai.** Un bot che bluffa invece di passare a un umano frustra i clienti e perde vendite. Progetta prima il passaggio.

**Testi generici e piatti.** Testo IA che suona come quello di tutti gli altri. Modificalo per la tua voce o verrà ignorato.

**Fidarsi troppo del punteggio dei contatti.** Trattare un punteggio come un verdetto invece che come un indizio. Usalo per impostare la priorità, non per ignorare le persone.

**Spazzatura dentro, analisi spazzatura fuori.** Se i dati del tuo CRM sono disordinati, i segmenti e i segnali di abbandono sono sbagliati. Pulisci prima i tuoi dati.

**Trattare i clienti come punti dati.** Usare l'analisi per manipolare invece che servire. Resta dalla parte etica.

**Nessuna divulgazione dei bot.** Lasciare che un chatbot finga di essere umano. Sii chiaro.

**Ignorare le regole sulla privacy.** Usare dati personali senza consenso o sicurezza. Segui le basi del GDPR.

**Confondere attività con risultati.** Contare le email mandate invece degli affari chiusi. Misura i risultati, non il volume.

**Saltare la baseline.** Non misurare la conversione prima, così non puoi provare l'incremento. Misura prima (vedi Capitolo 22).

**Sostituire completamente il tocco umano.** I clienti vogliono ancora una persona per i problemi difficili. Tieni gli umani per le conversazioni di valore.

## Esercizio pratico

### 26.7 Esercizio: pianifica una campagna assistita dall'IA

Scegli una campagna — un'email a clienti passati, un chatbot sul tuo sito, o una passata di punteggiatura dei contatti — e pianificala dall'inizio alla fine.

**Passo 1 — Scegli il lavoro.** Scegline uno: punteggiatura dei contatti, una campagna email, un chatbot, o un'analisi dei clienti. Fanne uno, non tutti.

**Passo 2 — Definisci l'obiettivo e la metrica.** Cosa dovrebbe ottenere? Iscrizioni, risposte, domande risolte, clienti riconquistati? Scegli un numero da misurare.

**Passo 3 — Misura la baseline.** Qual è quel numero ora? Scrivilo. Senza di esso non puoi provare l'incremento.

**Passo 4 — Raccogli i dati.** Per la punteggiatura: i tuoi contatti passati e quali si sono chiusi. Per l'email: la tua lista con consenso. Per il chatbot: le tue vere domande e risposte dei clienti. Per l'analisi: i tuoi registri clienti. Pulisci prima i dati.

**Passo 5 — Costruisci la parte di IA.** Punteggia i contatti, redigi l'email, forma il bot, o esegui la segmentazione. Lascia che l'IA faccia il lavoro pesante.

**Passo 6 — Aggiungi la revisione umana.** Leggi ogni bozza. Controlla ogni affermazione fattuale. Decidi le regole di passaggio del chatbot. Niente esce senza una lettura umana.

**Passo 7 — Controlla consenso e privacy.** Conferma che ti è permesso mandare messaggi a queste persone e che i loro dati sono gestiti correttamente.

**Passo 8 — Lancia in piccolo e misura.** Fallo girare prima su un piccolo gruppo. Confronta la metrica con la baseline. Se funziona, scala verso l'alto. Se no, impara e aggiusta.

Fai bene una campagna. Le lezioni che impari — sul tono, sui passaggi, su cosa i tuoi clienti rispondono — si portano in ogni campagna successiva.

## Checklist

### 26.8 Checklist vendite e marketing

Prima di lanciare qualsiasi attività di vendite o marketing assistita dall'IA, controlla queste.

- [ ] **Hai misurato la baseline** per l'unica metrica a cui tieni.
- [ ] **Un umano rivede ogni messaggio scritto dall'IA** prima che raggiunga un cliente.
- [ ] **Ogni affermazione fattuale è controllata** — prezzo, funzionalità, risultati.
- [ ] **Hai il consenso** per mandare messaggi alle persone a cui li mandi.
- [ ] **Rispetti la frequenza** — niente spam, niente invii eccessivi.
- [ ] **Il chatbot ha chiare regole di passaggio** a un umano.
- [ ] **Il chatbot è formato sulle tue vere domande**, non su domande generiche.
- [ ] **Divulghi che è un bot** dove richiesto e come buona pratica.
- [ ] **Pulisci i tuoi dati** prima di punteggiare, segmentare o analizzare.
- [ ] **Restituisci gli esiti** al modello di punteggiatura dei contatti così impara.
- [ ] **Tratti il punteggio dei contatti come un indizio**, non un verdetto.
- [ ] **Usi l'analisi per servire i clienti**, non per manipolarli.
- [ ] **Segui le regole sulla privacy** (basi GDPR, vedi Capitolo 10).
- [ ] **Mantieni gli umani per le conversazioni difficili.**
- [ ] **Misuri i risultati** (affari, risposte, vittorie), non solo il volume mandato.
- [ ] **Lanci in piccolo prima** e fai scala solo a ciò che si dimostra.

Se una casella è vuota, stai rischiando la fiducia. Riempila prima di premere invia.

## Punti chiave

- L'IA aiuta vendite e marketing personalizzando su larga scala — punteggiando i contatti, adattando i messaggi, rispondendo a domande e individuando clienti a rischio.
- Il caso mobilezone (una storia cliente Microsoft) costruì due agenti Copilot Studio — Mia per i clienti, Supporto per l'IT interno — gestendo oltre 1.600 chat al mese e tagliando il tempo di risoluzione IT di circa il 50%.
- L'IA redige, un umano rivede: non spedire mai un messaggio scritto dall'IA né lasciare che un chatbot bluffi invece di passare a una persona.
- Dati puliti sono la fondazione — registri disordinati rendono punteggiature, segmenti e segnali di abbandono sbagliati.
- Usa l'IA per servire meglio i clienti, non per fare spam o manipolarli; consenso e onestà proteggono la fiducia su cui stai vendendo.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come lo stesso lavoro appare con AgentBridge. Ogni riquadro mostra il risultato finito e l'unica riga che digiti per ottenerlo.

### Trasforma un'idea in una proposta

![Un documento di proposta di progetto strutturato](../../assets/examples/project-proposal.png)
*Un documento di proposta di progetto strutturato*

**Cosa chiedi:** `Crea una proposta di progetto per un piccolo negozio online: obiettivi, cosa consegniamo, una tempistica di 8 settimane, e un prezzo di 9.500 euro.`

L'agente costruisce una proposta con l'obiettivo del cliente, la tua soluzione, i consegnabili, la tempistica e il prezzo — tutto in un layout pulito che sembra aver richiesto un intero pomeriggio. Ha richiesto un minuto.

*Suggerimento: Aggiungi il tuo logo e una frase sui risultati passati per renderlo personale.*

---

### Traccia le tue vendite

![Un tracker vendite con ricavi per canale](../../assets/examples/sales-tracker.png)
*Un tracker vendite con ricavi per canale*

**Cosa chiedi:** `Crea un tracker vendite con mese, canale e ricavi, e un grafico dei ricavi per canale.`

L'agente costruisce il tracker e il grafico. Aggiungi righe man mano, o allega la tua lista di vendite grezza e chiedigli di compilare il foglio per te.

*Suggerimento: Allega un'esportazione disordinata dal tuo negozio e di' 'pulisci questo in un tracker' — lo farà.*

---

### Una presentazione di pitch da un solo prompt

![Una slide di presentazione costruita dall'agente](../../assets/examples/pitch-deck.png)
*Una slide di presentazione costruita dall'agente*

**Cosa chiedi:** `Fai una presentazione di pitch di 6 slide per la mia startup di consegne: problema, soluzione, mercato, modello, trazione, richiesta.`

L'agente progetta le slide con un look pulito, un'idea chiara per slide, e il giusto ordine per un pitch. Nel browser premi F11 per lo schermo intero e presenta.

*Suggerimento: Ti serve un vero .pptx da mandare? Usa /tools office-files e chiedi PowerPoint.*

---

### Una presentazione di vendita per un cliente

![Una slide di presentazione di vendita rivolta al cliente](../../assets/examples/sales-presentation.png)
*Una slide di presentazione di vendita rivolta al cliente*

**Cosa chiedi:** `Crea una presentazione di vendita che riassuma il nostro lavoro con Acme e proponga la prossima fase.`

L'agente costruisce una presentazione focalizzata: risultati finora, cosa il cliente ha guadagnato, e il prossimo passo proposto. Tu ritocchi i numeri e presenti con sicurezza.

*Suggerimento: Allega il report di progetto e l'agente estrae i punti salienti nelle slide.*

---

### Un follow-up gentile

![Una bozza di email di follow-up amichevole](../../assets/examples/follow-up.png)
*Una bozza di email di follow-up amichevole*

**Cosa chiedi:** `Scrivi un breve follow-up a un cliente che non ha risposto al nostro preventivo della settimana scorsa.`

L'agente scrive un promemoria leggero e gentile che ricorda senza pressione. Tu lo mandi e tieni caldo il rapporto.

*Suggerimento: Un follow-up programmato può mandarli per te se una risposta non è arrivata.*

---

### Una newsletter per clienti

![Una bozza di newsletter pronta da mandare](../../assets/examples/newsletter.png)
*Una bozza di newsletter pronta da mandare*

**Cosa chiedi:** `Scrivi una newsletter mensile per i nostri clienti: nuovi articoli, un consiglio, e un piccolo codice sconto.`

L'agente scrive la newsletter nella tua voce con le novità, un consiglio utile e l'offerta. Mandala, o lasciala preparare una su un programma.

*Suggerimento: Un'attività programmata mensile può redigere la newsletter per la tua revisione ogni volta.*

---

### Trasforma un argomento in un podcast

![Un episodio di podcast pronto da riprodurre](../../assets/examples/podcast-episode.png)
*Un episodio di podcast pronto da riprodurre*

**Cosa chiedi:** `Crea un episodio di podcast di 5 minuti sul perché i piccoli negozi dovrebbero andare online, in uno stile amichevole a due voci.`

L'agente scrive il copione e produce un episodio audio con due voci, pronto da pubblicare. Il tuo messaggio, in forma audio, senza studio.

*Suggerimento: Dagli i tuoi punti chiave e li modella in una conversazione naturale.*

<!-- END agentbridge-examples -->
