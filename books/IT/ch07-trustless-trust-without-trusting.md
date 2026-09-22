# Capitolo 7 — Trustless: fidarsi senza dover credere

## In parole semplici

La parola "trustless" è scelta male. Sembra un mondo senza fiducia, dove nessuno crede a niente. Non è questo che significa, e l'idea vera è molto più utile.

Trustless significa: **non devi fidarti di una persona o di un'istituzione, perché puoi verificare tu stesso il fatto.**

Parti da un contrasto familiare. Assumi una ditta di traslochi. Consegni un acconto. Ora dipendi dal fatto che si presentino. Devi fidarti di loro, o fidarti del loro marchio, o fidarti che la legge li punisca se non lo fanno. Ora pensa a un distributore automatico. Metti le monete, la bevanda esce. Non c'è relazione, non c'è promessa, e non c'è bisogno di credere a nessuno. La macchina fa rispettare l'accordo dal modo in cui è costruita. Questa è la sensazione del trustless: l'accordo è fatto rispettare da un sistema invece che dalle buone intenzioni di una persona.

Tre strumenti rendono questo possibile.

**Verifica invece di promesse.** Invece di qualcuno che ti dice che una cosa è vera, la controlli. Una firma digitale è l'esempio comune. Prova che un file proveniva da chi detiene una particolare chiave, e che il file non è cambiato da quando è stato firmato. Non devi fidarti del mittente. Controlli la firma.

**Trasparenza invece di segretezza.** Invece di tenere un registro in un unico quaderno privato, lo tieni da qualche parte dove molti possono leggere e nessuno può riscrivere di nascosto. Se tutti possono vedere il registro, una parte non può cambiare la storia a proprio piacimento.

**Applicazione automatica invece di speranza.** Invece di concordare delle condizioni e sperare che vengano rispettate, scrivi le condizioni in modo che un software le esegua. Il denaro viene rilasciato quando la condizione è soddisfatta. Nessuno deve inseguire una fattura.

Ora l'avviso onesto, detto subito: trustless non significa senza rischi. Hai spostato la tua fiducia dalle persone ai sistemi, e i sistemi sono costruiti da persone. Il codice ha bug. I flussi di dati che dicono a un sistema cosa è successo nel mondo reale possono essere sbagliati o mentire. Le chiavi si perdono, e una chiave persa può significare denaro perso. L'obiettivo non è rimuovere la fiducia. È collocarla da qualche parte che puoi ispezionare, e ridurre quanta te ne serve.

Perché bother affatto? Perché la fiducia costa. Ogni intermediario a cui ti affidi — una banca, un agente di escrow, un mediatore, un notaio, una piattaforma che trattiene i fondi finché il lavoro non è fatto — prende una commissione e prende tempo. I sistemi trustless ne rimuovono un po', e rendono ciò che resta più economico, più veloce e visibile. Questo non è solo per banche e programmatori; ha un uso diretto in qualsiasi azienda che compra da fornitori, ingaggia freelance, e ha bisogno di registri di cui il suo contabile possa fidarsi.

La domanda più ampia di chi controlla i tuoi strumenti digitali è nel [Capitolo 11](ch11-digital-sovereignty.md). Se ripaga è una domanda del [Capitolo 16](ch16-goals-costs-and-return-on-investment.md). Il lato sicurezza della verifica è nel [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md).

## Un po' di storia

**2008.** In ottobre un paper intitolato "Bitcoin: A Peer-to-Peer Electronic Cash System" fu pubblicato sotto il nome di Satoshi Nakamoto. Il suo scopo dichiarato era il pagamento elettronico senza terze parti fidate. Il trucco era un registro condiviso e ordinato — una blockchain — mantenuto insieme da molti computer indipendenti, così che nessuno di essi da solo possa riscriverlo.

**2009.** La rete Bitcoin iniziò a funzionare a gennaio. Per la prima volta, due sconosciuti potevano scambiare valore senza una banca nel mezzo, e nessuno dei due doveva fidarsi dell'altro.

**2015.** Ethereum arrivò e aggiunse il miglioramento chiave: gli smart contract. Uno smart contract è un programma memorizzato sulla rete che funziona esattamente come scritto quando le sue condizioni sono soddisfatte. Il denaro poteva ora essere legato a una regola.

**2016.** Un progetto chiamato The DAO deteneva fondi in uno smart contract e fu svuotato a causa di un difetto in quello smart contract. Le conseguenze spaccarono la comunità. La lezione fu netta e ancora vera: l'applicazione automatica applica i bug con la stessa lealtà con cui applica le funzionalità.

**2017 al 2021.** La finanza decentralizzata crebbe fino a diventare un settore reale: prestiti, trading e compensazioni gestiti da contratti invece che da banche, con stablecoin — token pensati per mantenere un valore stabile — come suo denaro operativo. Mostrò anche gli stessi fallimenti su scala più grande: codice cattivo, flussi di prezzo sbagliati, operatori disonesti. Nel **2019** il W3C, l'organismo che stabilisce gli standard web, pubblicò le Credenziali Verificabili: un modo per un'autorità di emettere una dichiarazione digitale — un titolo di studio, una licenza, una prova dell'età — che chiunque può controllare senza telefonare all'emittente. Questa è la metà identitaria del quadro.

**2021 al 2023.** Uno standard chiamato ERC-4337, noto come astrazione di account, fu proposto nel 2021 e poi finalizzato. Permette a un account di essere un piccolo programma invece di una singola chiave privata, così l'account può contenere le proprie regole: limiti di spesa, una lista di beneficiari consentiti, una seconda firma per importi elevati, e recupero se una chiave è persa.

**Maggio 2025.** Un aggiornamento di Ethereum chiamato Pectra è andato live sulla rete principale. Ha permesso a un normale indirizzo di wallet di puntare a codice di smart contract, portando raggruppamento delle transazioni, commissioni sponsorizzate e un recupero migliore a indirizzi che prima non ne avevano. Ha anche alzato il massimo di puntata che un singolo validatore può detenere.

**Agosto 2025.** È apparso uno standard provvisorio chiamato ERC-8004, intitolato "Trustless Agents". È stato scritto per il problema di cui questo capitolo tratta davvero: agenti software che hanno a che fare con gli agenti di altre persone.

Leggi la linea del tempo come un unico lungo argomento. Ogni passo ha spostato l'applicazione dalle mani di una persona a un sistema verificabile: prima il denaro, poi gli accordi, poi l'identità, poi le autorizzazioni, e più di recente gli agenti.

## Curiosità

### 7.6 Ethereum sta costruendo la tubatura per un'economia di agenti

Nell'agosto 2025 uno standard provvisorio chiamato **ERC-8004** è stato pubblicato sul sito ufficiale degli standard di Ethereum. Il suo titolo è "Trustless Agents", e il suo scopo dichiarato è permettere agli agenti software di scoprire, scegliere e lavorare con altri agenti oltre i confini organizzativi senza alcuna fiducia preventiva.

Definisce tre registri, tutti on-chain.

**Identità.** Ogni agente ottiene un identificatore on-chain, costruito sullo standard comune di token ERC-721, che punta a un file di registrazione. Quel file contiene i metadati dell'agente, gli indirizzi con cui puoi parlare, e quali modelli di fiducia supporta. In parole povere: un agente può dire chi è, per chi agisce, e come puoi verificarlo, e tu puoi cercare queste cose invece di credergli sulla parola.

**Reputazione.** Un modo standard per pubblicare e leggere feedback su un agente, così che lo storico delle prestazioni non resti bloccato nella valutazione a stelle privata di una piattaforma. Chiunque può contribuire con segnali, e l'aggregazione può avvenire off-chain. Il punto è la portabilità: il registro di un agente lo segue, invece di essere azzerato ogni volta che cambia mercato.

**Validazione.** Ganci per ottenere un controllo indipendente del lavoro di un agente. Lo standard elenca diversi metodi: far rieseguire il lavoro a un'altra parte con denaro in gioco, usare prove di machine learning a conoscenza zero — un modo di provare che un calcolo è stato fatto correttamente senza rivelare i dati o il modello dietro di esso — usare enclaves hardware fidate, o usare un giudice umano fidato.

Perché un piccolo titolare d'azienda dovrebbe interessarsi a uno standard provvisorio? Mostra dove l'industria pensa che sia il problema difficile: non "un agente sa fare il compito" ma "come faccio a sapere se credere a questo agente" — una domanda di business, non tecnica. Se avrà successo, potrai controllare un registro pubblico invece di fidarti di una presentazione di vendita, il che cambia chi detiene il potere nella conversazione. E le stesse tre domande sono una checklist utile già oggi, senza alcuna blockchain: *Chi sei, e per chi agisci? Come ti sei comportato in passato? Il tuo lavoro può essere controllato indipendentemente?*

Due altri pezzi della stessa tubatura sono già attivi. L'astrazione di account, lo standard ERC-4337, significa che un agente può detenere un budget con regole applicate dal codice: un limite duro di spesa, una whitelist di beneficiari consentiti, una seconda firma umana sopra una soglia. E dalla distribuzione di Pectra nel maggio 2025, un normale indirizzo può puntare a tale codice. Questa combinazione — un agente che può pagare, dentro una scatola da cui non può uscire — è la forma pratica di un'economia trustless di agenti.

Tratta tutto questo come direzione, non come un prodotto da comprare questo trimestre. ERC-8004 è provvisorio. I concetti, però, sono utilizzabili ora.

## Un esempio reale di business

### Il mango che ha richiesto sette giorni per essere tracciato, poi due secondi

Nel 2017 Walmart e IBM condussero un pilota nelle catene di approvvigionamento alimentare, e i numeri che pubblicarono diventarono famosi nel settore. Tracciare l'origine di un mango acquistato in Centro o Sud America richiedeva circa sette giorni di telefonate, email e inseguimenti di carte. Con i registri tenuti su un registro condiviso, lo stesso tracciamento richiese circa 2,2 secondi. IBM lo descrisse come tracciabilità completa end-to-end. Un pilota parallelo tracciava la carne suina in Cina.

Due note oneste. La cifra proveniva da un pilota controllato, non da un lancio completo dal vivo, e i 2,2 secondi sono il tempo per interrogare il registro, non il tempo per correggere una spedizione contaminata.

Ora guarda cosa è cambiato. Prima, ogni parte teneva il proprio quaderno: la fattoria scriveva la data del raccolto, l'impacchettatore il lotto, il trasportatore il container, il negozio la consegna. Per rispondere a una domanda dovevi chiedere a quattro aziende di cercare nei loro quaderni privati e sperare che rispondessero velocemente e onestamente. Dopo, tutti scrivevano nello stesso registro man mano che procedevano. Nessuno poteva riscrivere silenziosamente la propria pagina, e "da dove viene questo" è diventato una ricerca invece che una negoziazione.

Questo è il valore trustless in una frase: **hai sostituito una catena di promesse con un unico registro condiviso che puoi leggere.**

Mostra anche il limite, che conta più della vittoria. Un registro condiviso prova cosa è stato scritto. Non prova che lo scritto fosse vero. Se un fornitore inserisce una fattoria falsa o una data falsa, il registro conserva la bugia perfettamente. L'anello debole è il momento in cui un umano o un sensore mette un fatto nel sistema. Qualsiasi progetto trustless che ignora quel momento è decorazione.

## Come si fa

### 7.3 Come funziona nella pratica: identità verificabile, reputazione, pagamenti programmabili

Non ti serve una criptovaluta per usare il pensiero trustless. Quattro blocchi costruttivi si applicano al business ordinario.

**Blocco 1: Identità verificabile.**
La domanda è: questo è davvero chi dice di essere, e posso controllare senza telefonare a nessuno? Certificati digitali e firme digitali già rispondono a questo per te ogni giorno. Quando un fornitore invia un documento firmato con una firma digitale riconosciuta, puoi verificare sia chi l'ha firmato sia che nulla è cambiato dopo. Una credenziale verificabile va oltre: il tuo contabile può provare di avere una licenza valida, o un dipendente può provare di aver superato un controllo dei precedenti, senza consegnare l'intero certificato e senza che tu chiami l'ente emittente.

**Blocco 2: Registri a prova di manomissione.**
La domanda è: qualcuno può riscrivere la storia di nascosto? Un registro condiviso è una risposta. Così è un trucco più semplice chiamato hash — una breve impronta digitale calcolata da un file. Se registri l'impronta di un documento nel momento in cui lo concordate, e il file viene cambiato dopo, l'impronta non corrisponderà. Puoi produrre quell'impronta dopo e provare lo stato del documento a quel tempo. Questo costa quasi nulla e non richiede permessi speciali.

**Blocco 3: Pagamenti programmabili.**
La domanda è: può il denaro muoversi da solo quando la condizione è soddisfatta? L'escrow è la vecchia versione: una terza parte trattiene i fondi e li rilascia a un trigger. La versione più nuova scrive il trigger nel codice, così non serve nessuna decisione umana al momento del rilascio. Il pagamento a milestone per un freelance è il caso ovvio: il pagamento viene rilasciato quando il consegnabile viene accettato, e la regola di accettazione è scritta in anticipo.

**Blocco 4: Rintracciabilità.**
La domanda è: dopo i fatti, possiamo entrambi vedere la stessa verità? Ogni azione dovrebbe lasciare un registro con timestamp, ordinato e non modificabile. Quando entrambe le parti leggono lo stesso registro, le discussioni si accorciano. Il tuo contabile, il tuo revisore e il tuo cliente possono tutti controllare la stessa cosa senza chiedere un favore a te.

**Come iniziare in piccolo, oggi:**

1. Scegli un processo in cui attualmente inseguivi una conferma.
2. Scrivi la condizione di rilascio come una singola frase verificabile. Se non riesci a scriverla come frase verificabile, il processo non è pronto.
3. Chiediti se una macchina può misurare il trigger. "Consegnato" significa una nota di consegna firmata scansionata. "Approvato" significa un clic su un pulsante di approvazione. "Completato" significa un cambio di stato nel tuo stesso sistema.
4. Metti il denaro dietro una regola che aspetta quella misurazione: un servizio di escrow, un piano di pagamenti nel tuo sistema contabile, o un flusso di lavoro che richiede il trigger prima del rilascio.
5. Registra ogni passo dove entrambe le parti possono vederlo.
6. Solo allora automatizza.

### 7.4 Agenti IA che interagiscono tra loro: il futuro del business automatizzato

La versione interessante di questo è vicina. Il tuo agente software parla con l'agente software di un fornitore, e chiudono una transazione senza un umano a ogni passo.

Perché questo funzioni in sicurezza, cinque cose devono esistere.

**Identità e autorità.** Non solo "questo è l'agente del fornitore X", ma "questo agente è autorizzato a impegnare fino a 500 unità a un prezzo inferiore a 4,20 l'una". L'autorità deve essere dimostrabile e delimitata, non data per scontata.

**Un accordo leggibile dalla macchina.** Entrambe le parti hanno bisogno dei termini in una forma strutturata — quantità, prezzo, data di consegna, penale — non un cordiale thread di email. Un umano può perdonare l'ambiguità. Un sistema automatizzato o si blocca su di essa o la sfrutta.

**Una rotaia di pagamento che può aspettare.** Il pagamento deve essere condizionale: trattenuto, poi rilasciato su prova. Un pagamento istantaneo e incondizionato rimuove ogni leva e ogni motivo per eseguire.

**Prova.** Una conferma di consegna, un record di accettazione, una ricevuta firmata, in una forma che entrambi i sistemi possono leggere e che nessuno dei due può alterare di nascosto.

**Un percorso di disputa.** Qualcosa deve gestire il caso in cui i due agenti non sono d'accordo, o in cui il mondo non è andato come la regola assumeva. Senza un percorso di escalation, una piccola disputa diventa un pagamento bloccato e un fornitore arrabbiato.

Cosa è realistico ora: gli agenti possono già cercare, confrontare, redigere preventivi e preparare ordini. Cosa non è ancora di routine è lasciarli impegnare denaro e termini legali da soli. Il percorso sensato è un umano che approva l'impegno finale mentre l'agente prepara tutto. Questo mantiene la velocità e elimina il rischio.

### 7.5 Cosa significa per la tua azienda: smart contract, pagamenti automatici, rintracciabilità

**Smart contract, in parole semplici.** Uno smart contract è un programma che detiene un accordo e lo esegue quando si verifica la condizione dichiarata. Non è furbo e non è un contratto nel senso dell'avvocato. È un distributore automatico molto letterale. Scrivi la regola con cura ed è un ottimo servitore. La scrivi in modo lasco ed è un ottimo servitore anche lui — di ciò che hai effettivamente scritto.

**Pagamenti automatici.** La forma pratica è un pagamento che aspetta. Aspetta una conferma di consegna, un clic di approvazione, una milestone accettata, una data raggiunta. Ognuno è limitato, registrato e visibile a entrambe le parti prima di muoversi.

**Rintracciabilità.** Ogni passo lascia un registro. Il tuo contabile chiude il mese più velocemente perché non c'è nulla da ricostruire. Una disputa con un cliente finisce in minuti perché entrambe le parti guardano la stessa riga. Se un regolatore chiede, produci il registro invece di una storia.

**Dove si adatta bene:** pagamenti transfrontalieri a fornitori dove l'applicazione è lenta; milestone di freelance e contraenti; mercati dove compratore e venditore sono sconosciuti; accordi di condivisione dati dove devi provare cosa hai rilasciato e quando; assicurazioni che pagano su un evento misurato, come un ritardo di un volo.

**Dove si adatta male:** tutto ciò che richiede giudizio, negoziazione o una relazione. Tutto ciò dove il trigger non può essere misurato onestamente. Tutto ciò dove un pagamento automatico sbagliato è difficile da recuperare.

## Etica e responsabilità

I sistemi trustless cambiano chi è responsabile, ed è esattamente per questo che richiedono un'attenta riflessione.

**Il codice che fa rispettare fa rispettare anche gli errori.** Se la tua regola rilascia un pagamento su una condizione facile da falsificare, hai automatizzato una perdita. Scrivi la regola per il caso disonesto, non solo per quello efficiente.

**Gli oracoli sono persone.** Un "trigger misurabile dalla macchina" spesso dipende da un umano che inserisce dati da qualche parte. L'anello più debole di una catena trustless è il momento in cui una persona digita la verità dentro di essa. Progetta pensando che quella persona sia di corsa, sbagli, o corrotta.

**L'immutabilità collide con la privacy.** Mettere dati personali su un registro permanente e immutabile può entrare in conflitto con i diritti di protezione dei dati, incluso il diritto alla cancellazione. Tieni i dati personali fuori dai registri pubblici; conserva solo riferimenti e impronte digitali. Il dettaglio legale è nel [Capitolo 10](ch10-privacy-and-gdpr.md).

**Non rimuovere l'umano da un problema umano.** I clienti infelici non vogliono una regola perfettamente applicata; vogliono che qualcuno li ascolti. Il trustless serve per la parte noiosa centrale di una transazione, non per il momento in cui qualcuno è contrariato.

**Sii trasparente, e mantieni un proprietario nominato.** Dillo alle persone il cui lavoro ora è misurato dal sistema, e spiega come una decisione può essere ribaltata; una regola che nessuno può mettere in discussione alla fine sarà sbagliata senza nessuno che possa correggerla. L'applicazione automatica non rimuove la responsabilità — qualcuno nella tua azienda deve comunque possedere il risultato, come illustrato nel [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md).

## Errori da evitare

### 7.7 Non tutto deve essere trustless

1. **Usare una blockchain dove basterebbe un foglio di calcolo.** Se le parti si fidano l'una dell'altra, il registro è piccolo, e un normale contratto funziona, un registro distribuito aggiunge costo e complessità per nulla.
2. **Confondere trustless con senza rischi.** Il codice ha bug, i flussi possono essere sbagliati, le chiavi si possono perdere, e spesso non c'è un numero di assistenza da chiamare.
3. **Automatizzare un cattivo processo.** Un sistema trustless applicherà il tuo cattivo processo più velocemente e più coerentemente di quanto abbia mai fatto una persona.
4. **Mettere dati personali su una catena pubblica.** Non può essere cancellato dopo.
5. **Nessun interruttore di arresto.** Qualsiasi sistema di pagamento automatico ha bisogno di un modo per fermarlo con un clic.
6. **Nessun limite di spesa.** Un agente con un wallet aperto è un libretto degli assegni aperto.
7. **Fidarsi troppo del trigger.** Chiediti come il trigger potrebbe essere falsificato, poi decidi se conta.
8. **Inseguire una presentazione di vendita.** "Trustless" è una utile idea di design, non una ragione per comprare un token. Se una proposta non sa spiegare il trigger, il registro e il percorso di disputa, è marketing.
9. **Eliminare ogni intermediario.** Alcuni intermediari guadagnano la loro commissione. Un notaio, un agente doganale o un assicuratore possono fare un lavoro reale che il codice non può fare.
10. **Dimenticare chi è responsabile.** Anche con l'applicazione automatica, un umano nominato deve possedere il risultato.

## Esercizio pratico

### 7.8 Pensa a un processo aziendale che potrebbe beneficiare dell'automazione trustless

Scegli un processo in cui attualmente spendi tempo a controllare, inseguire o discutere. Lavora su queste nove domande per iscritto.

1. **Chi sono le parti?** Nominalle. Nota se si fidano già l'una dell'altra.
2. **Cosa deve essere vero prima che il denaro si muova?** Una frase.
3. **Chi verifica questo oggi?** Una persona? Quanto tempo richiede? Quanto spesso sbaglia?
4. **Quanto costa quella verifica?** Tempo, commissioni, ritardi. Numeri approssimativi vanno bene; marchiali come approssimativi.
5. **Una macchina può misurare il trigger?** Se sì, qual è il segnale? Se no, il processo può essere riprogettato perché possa?
6. **Qual è la traccia di prove?** Quale registro esiste, dove, e una delle due parti può cambiarlo?
7. **Cosa succede in una disputa?** Chi decide, e quanto velocemente?
8. **Qual è il modo peggiore in cui questo potrebbe essere abusato?** Scrivi lo scenario disonesto prima di quello efficiente.
9. **Qual è il limite?** La perdita massima se la regola è sbagliata.

Ora dagli un punteggio. Se il costo della verifica è una grossa quota del valore della transazione, il trigger è misurabile dalla macchina, e puoi impostare una perdita massima bassa, il processo è un forte candidato. Se il trigger non può essere misurato da una macchina, o la perdita massima è alta, tienici un umano dentro.

Scrivi una pagina. Porta un candidato alla tua prossima riunione.

## Checklist

### 7.9 Quando considerare un approccio trustless

- [ ] **Paghi un intermediario principalmente per trattenere o controllare qualcosa**, e quel controllo potrebbe essere scritto come una regola.
- [ ] **Le parti non si fidano già l'una dell'altra**, e costruire fiducia sarebbe lento o impossibile.
- [ ] **La condizione di rilascio può essere espressa come una singola frase verificabile** che una macchina può misurare.
- [ ] **La transazione avviene spesso**, così il costo di configurazione è spalmato su molti usi.
- [ ] **È transfrontaliera o tra aziende**, dove l'applicazione locale è lenta o poco chiara.
- [ ] **Ti serve un registro condiviso e non modificabile** che entrambe le parti e il tuo revisore possano leggere.
- [ ] **Puoi impostare un limite duro di spesa** e un arresto con un clic prima di automatizzare.
- [ ] **Nessun dato personale deve stare sul registro permanente.**
- [ ] **Un percorso di disputa esiste** e nomina un umano che può scavalcare la regola.
- [ ] **L'hai confrontato onestamente** con un normale contratto e un normale processo, e il trustless vince comunque su costo, velocità o rischio.

## Punti chiave

- Trustless non significa assenza di fiducia; significa che verifichi un fatto invece di fidarti di una persona che te lo racconti.
- Le tre parti funzionanti sono identità verificabile, registri a prova di manomissione, e applicazione automatica di una condizione scritta.
- Lo standard provvisorio ERC-8004 di Ethereum e gli standard di astrazione di account mostrano dove sta andando il business agente-ad-agente: identità, reputazione e validazione indipendente, con budget delimitati dal codice.
- L'anello debole è il trigger — il momento in cui un umano o un sensore dice al sistema cosa è successo davvero.
- Non usare il trustless dove un normale contratto funziona; usalo dove la verifica è costosa, il trigger è misurabile e la perdita massima è limitata.
