# Capitolo 6 — La cybersecurity nell'era dell'IA

## In parole semplici

Per gran parte della storia dell'informatica aziendale, la sicurezza significava una cosa sola: tenere gli estranei fuori dal tuo edificio. Avevi una porta chiusa a chiave, una password, un firewall. La persona cattiva era fuori. I tuoi dati erano dentro.

L'intelligenza artificiale ha sfumato quel confine. Oggi, quando un dipendente digita un elenco di clienti, un contratto o un foglio stipendi in uno strumento IA online, quel testo esce dall'edificio. Viaggia fino a computer che appartengono a qualcun altro. Lì può essere memorizzato. Può essere letto dal personale di assistenza. Può essere conservato per mesi. In alcuni casi può essere usato per migliorare il prodotto di quell'azienda. La maggior parte delle persone non ci pensa mai, perché lo strumento sembra una casella di ricerca. Non è una casella di ricerca. È un servizio, gestito da un'azienda, su macchine che tu non controlli.

L'IA cambia il quadro della sicurezza in due direzioni allo stesso tempo.

**Gli attaccanti sono migliorati.** Un modello linguistico dà a un criminale tre cose che prima erano costose: velocità, scala e rifinitura. Un'email di phishing che una volta sembrava una cattiva traduzione ora può essere scritta in un tedesco o giapponese aziendale fluente in pochi secondi, personalizzata con dettagli presi da un profilo pubblico. Una voce può essere copiata da pochi secondi di una registrazione, ed è così che impiegati amministrativi in casi di frode riportati hanno approvato bonifici perché chi chiamava suonava come il loro capo. Nulla di tutto questo richiede un genio. Richiede un abbonamento.

**La tua superficie di attacco è cresciuta.** "Superficie di attacco" è solo un termine per il numero di punti da cui qualcuno può entrare. Ogni funzione IA che aggiungi è una nuova porta: strumenti di chat, plugin che raggiungono la tua email, agenti che leggono cartelle e inviano messaggi, modelli addestrati sui tuoi archivi, fornitori che conservano una copia di ogni prompt e di ogni risposta. Due anni fa la tua azienda aveva una porta principale. Ora potrebbe averne quaranta, e la maggior parte le ha aperte il tuo stesso personale senza dirlo a nessuno.

Un'ulteriore idea organizza tutto il resto. La sicurezza protegge tre cose, note con tre parole brevi.

- **Riservatezza.** Solo le persone giuste vedono i dati.
- **Integrità.** I dati non sono stati modificati di nascosto.
- **Disponibilità.** Il sistema funziona quando ti serve.

La maggior parte dei titolari tratta la sicurezza dell'IA come solo un problema di riservatezza. Non lo è. Un concorrente che avvelena il tuo modello è un problema di integrità. Un fornitore i cui sistemi si bloccano e fermano i tuoi pagamenti per settimane è un problema di disponibilità, e quest'ultimo ha causato il danno maggiore nella storia più avanti in questo capitolo. Quando guardi un qualsiasi strumento IA, fai tutte e tre le domande.

Un avvertimento. Il pensiero "siamo troppo piccoli per essere attaccati" non è vero. Gli attacchi moderni sono automatizzati: un software scansiona tutto internet in cerca di porte aperte, come un ladro prova ogni auto in un parcheggio. Non vieni scelto perché sei interessante. Vieni colpito perché eri facile, e perché detieni dati dei clienti, dati bancari e registri fiscali con pochissima protezione intorno.

La buona notizia è che la maggior parte della protezione che ti serve non è alta tecnologia. È una breve lista di abitudini noiose, una mappa di dove vanno i tuoi dati, e alcuni controlli nel posto giusto.

Il lato legale dei dati personali è nel [Capitolo 10](ch10-privacy-and-gdpr.md). Il personale che usa strumenti IA senza approvazione — la "shadow AI" — è nel [Capitolo 9](ch09-third-party-services-and-shadow-ai.md). La costruzione passo per passo è nel [Capitolo 20](ch20-implementing-ai-securely.md).

## Un po' di storia

La storia della sicurezza ripete una sola lezione: il perimetro si sposta, e i difensori sono lenti ad accorgersene.

Nel **1988** il Morris worm disattivò circa il dieci percento dei computer connessi dei primi tempi di internet. Fu scritto da uno studente universitario, non da un criminale, e dimostrò che un programma auto-riproducenti poteva attraversare il pianeta in poche ore. Attraverso gli **anni '90 e 2000** la risposta standard fu il modello del perimetro: un firewall al confine, antivirus su ogni PC, dati su un server in un ripostiglio. Funzionava finché i dati restavano dove li avevi messi.

Nel **2013** il rivenditore americano Target fu violato. Gli attaccanti non entrarono in Target. Entrarono in una piccola azienda che forniva apparecchi di riscaldamento e condizionamento per i suoi negozi, presero le credenziali di quell'azienda e le usarono per raggiungere i sistemi di pagamento di Target. Circa 40 milioni di numeri di carta furono rubati. La lezione riguardava la connessione, non il codice: il tuo rischio ora include chiunque tu colleghi.

Nel **2016** Microsoft mise un chatbot chiamato Tay sui social media. Entro un giorno, gli utenti gli insegnarono a pubblicare materiale offensivo nutrendolo di messaggi ripetuti, e fu ritirato. Nessuno ruppe il programma. Ruppero ciò che il modello leggeva. Questo è il seme del prompt injection, anche se non aveva ancora un nome.

Nel **2017** il malware NotPetya si diffuse da un software contabile ucraino e causò danni misurati in decine di miliardi di dollari in tutto il mondo, colpendo il gigante della spedizione Maersk, il produttore farmaceutico Merck e molti altri. Un singolo link avvelenato in una catena di fornitura software divenne il problema di tutti in una volta.

Nel **2020** il lavoro da remoto rimosse il perimetro fisico quasi da un giorno all'altro. Nel **2022** ChatGPT rese l'IA generativa un normale strumento d'ufficio in poche settimane, e il personale iniziò a incollare lavoro reale in strumenti senza un contratto aziendale alle spalle. Nel **settembre 2022** il ricercatore di sicurezza Simon Willison pubblicò un post intitolato "Prompt injection attacks against GPT-3" e diede un nome a un problema che le persone vedevano ma non sapevano descrivere: istruzioni nascoste dentro un testo che un modello legge, le quali scavalcano le istruzioni che gli hai dato.

Nel **2023** i modelli a pesi aperti significarono che un'azienda poteva eseguire l'IA sul proprio hardware, come spiega il [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md). Lo stesso anno, i fornitori iniziarono a spedire "agenti" che possono agire anziché solo rispondere, il che alzò il costo di ogni errore. Nel **2024** il rischio dei fornitori divenne impossibile da ignorare, come raccontato nella sezione Curiosità qui sotto. Dal **2025** in poi, gli agenti sono arrivati con strumenti e credenziali attaccati, quindi il raggio d'azione di un singolo permesso sbagliato è ora tutto ciò che quell'agente può raggiungere.

Leggi la linea del tempo come un unico lungo argomento. Ogni passo ha spostato la fiducia da una porta chiusa a chiave a una relazione: un contraente, un fornitore, un plugin, un modello, un agente. La sicurezza ha smesso di essere un muro ed è diventata una domanda su chi, e cosa, hai collegato.

## Curiosità

### 6.8 Il fornitore che per poco non fermò un sistema sanitario

Il 12 febbraio 2024, degli attaccanti entrarono in Change Healthcare, un'azienda che elabora fatture mediche e pagamenti negli Stati Uniti. Secondo la testimonianza che l'amministratore delegato di UnitedHealth Group diede al Congresso americano nel maggio 2024, entrarono attraverso un portale di accesso remoto che non richiedeva l'autenticazione a più fattori — il secondo controllo su un login che impedisce alla maggior parte delle password rubate di funzionare. Non c'era alcun malware ingegnoso alla porta principale. C'era una password rubata e una seconda serratura mancante. Gli attaccanti passarono nove giorni dentro, muovendosi in silenzio e copiando circa sei terabyte di dati. Il 21 febbraio attivarono il ransomware e bloccarono i sistemi.

Change Healthcare è una controllata di UnitedHealth Group, e siede nel mezzo della catena dei pagamenti sanitari americani. Quando si fermò, una quota molto ampia di richieste dei medici, pagamenti delle farmacie e autorizzazioni assicurative si fermò con essa. Piccole cliniche non riuscivano a essere pagate e finirono la liquidità in poche settimane; gruppi di settore riportarono perdite dei fornitori per decine di milioni di dollari al giorno nella rete colpita. Grandi nomi che non avevano nulla a che fare con la violazione — catene di farmacie, assicurazioni regionali, un ospedale navale — si ritrovarono le proprie operazioni bloccate, perché tutti facevano passare dati attraverso lo stesso intermediario.

UnitedHealth in seguito anticipò più di 2 miliardi di dollari in prestiti di emergenza ai fornitori colpiti entro metà marzo, e più di 6 miliardi entro metà aprile. Reportage di Reuters e Wired dissero che un riscatto di circa 22 milioni di dollari in bitcoin fu pagato a un wallet collegato al gruppo criminale ALPHV, noto anche come BlackCat, che UnitedHealth confermò il 29 febbraio come l'attaccante. Nell'ottobre 2024 UnitedHealth stimò che circa 190 milioni di persone avevano subito la compromissione dei dati, una delle più grandi violazioni mai registrate.

Perché conta per una piccola azienda che non toccherà mai una richiesta medica? Per chi fu la vera vittima. Gli ospedali e le farmacie che soffrirono non furono hackerati. Molti di loro avevano una buona sicurezza. Furono feriti perché un'azienda nel mezzo del loro flusso di lavoro fu hackerata, e loro non potevano sopravvivere senza quell'azienda. La loro sicurezza era buona solo quanto il fornitore meno protetto nella loro catena.

Ora aggiungi l'angolo dell'analisi, perché è più vicino a casa di quanto sembri. Nel 2024, OpenAI divulgò un incidente che non era affatto una violazione dei propri sistemi. Il problema era in Mixpanel, un servizio di analisi di terze parti usato sul sito per sviluppatori della sua interfaccia di programmazione. I servizi di analisi sono piccoli pezzi di software che un'azienda mette sul proprio sito per contare le visite e vedere come le persone cliccano. Quel fornitore fu violato, e i nomi, gli indirizzi email e i dettagli dei dispositivi di alcuni titolari di account furono esposti. I contenuti delle chat, le password e le chiavi segrete no.

Il danno lì fu limitato. La lezione no. Quando compri un servizio IA, compri anche ogni azienda su cui quel servizio si appoggia: la sua analisi, il suo hosting, i suoi strumenti di supporto, i suoi plugin. Eredi una catena di fornitura che non hai mai scelto e di cui forse non avevi mai sentito parlare.

## Un esempio aziendale reale

### L'ingegnere che chiese aiuto alla chatbot

Nell'aprile 2023 Bloomberg riportò che Samsung aveva vietato gli strumenti di IA generativa come ChatGPT sulle apparecchiature aziendali. La ragione non era una teoria sul rischio. Gli ingegneri avevano incollato codice sorgente riservato in una chatbot pubblica mentre cercavano la correzione di un bug, in più di un'occasione, in una divisione che lavorava sui semiconduttori — uno dei tipi di codice più sorvegliati al mondo. Una nota interna esaminata da Bloomberg riportava che un sondaggio interno aveva scoperto che il 65 percento degli intervistati riteneva già lo strumento un rischio per la sicurezza.

Guarda la cosa dal lato dell'ingegnere. Nulla fu rubato. Nessuno entrò. Una persona era bloccata su un problema, trovò uno strumento che lo risolveva in dieci secondi, e lo usò. Lo strumento era eccellente. Il giudizio era scarso. Il codice non era suo da regalare.

Questo è il singolo fallimento di sicurezza IA più comune che esista, e non è esotico. Succede negli studi legali quando qualcuno incolla il contratto di un cliente per riassumerlo. Negli studi contabili con una dichiarazione dei redditi. Nelle agenzie con una campagna non ancora rilasciata di un cliente. Nelle risorse umane con un mucchio di CV. Lo schema è sempre lo stesso: uno strumento utile, una persona di corsa, e un copia-incolla che attraversa un confine che nessuno ha tracciato.

Due cose ne seguono. Primo, la soluzione non è solo un divieto, perché un divieto senza alternativa non ferma il comportamento; lo nasconde, il che è peggio, dato che ora non riesci a vedere i dati fluire. Secondo, la soluzione non è solo formazione, perché una persona di corsa alle cinque di sera non ricorderà una policy di quaranta pagine. La soluzione è rendere il percorso sicuro quello facile: uno strumento approvato più veloce di quello non sicuro, più un controllo che intercetta i dati peggiori prima che escano. Entrambi sono nella prossima sezione.

## Come si fa

### 6.7 Come proteggersi: firewall IA, filtri, monitoraggio

Fallo in ordine. Ogni passo dipende da quello prima.

**Passo 1: Disegna la mappa prima di comprare qualsiasi cosa.**
Prendi un foglio. Elenca ogni strumento IA che tocca la tua azienda, inclusi quelli gratuiti sui telefoni del personale. Per ciascuno: quali dati entrano, quali escono, dove sono memorizzati, chi è il fornitore, e se hai un contratto firmato. Troverai strumenti di cui non sapevi. Questo è il documento di sicurezza più prezioso che produrrai quest'anno.

**Passo 2: Metti una porta tra la tua gente e i servizi IA.**
Un "gateway IA" o "firewall IA" è un singolo punto da cui tutto il traffico IA passa, così puoi vederlo e controllarlo. I prodotti principali fanno questo: servizi di sicurezza dei contenuti e di protezione dei prompt delle grandi piattaforme cloud, barriere di sicurezza integrate nei servizi di modelli cloud, gateway consapevoli dell'IA, e strumenti di prevenzione della perdita di dati che ispezionano ciò che i dipendenti inviano. Devi sapere che la categoria esiste e cosa compra: un unico posto per consentire o bloccare strumenti, ispezionare i contenuti e conservare registri.

**Passo 3: Filtra ciò che esce.**
Il controllo di maggior valore in questa lista. Configura il tuo gateway o strumento anti-perdita per bloccare o avvisare sulle categorie che non devono mai uscire: numeri di identità nazionale e codice fiscale, numeri bancari e di carta, informazioni sanitarie, file paga, contratti firmati, codice sorgente e documenti riservi dei clienti. Un pop-up che dice "questo sembra un dato personale, sei sicuro?" da solo ferma una grossa quota di incidenti, perché la maggior parte di essi sono incidenti.

**Passo 4: Filtra ciò che entra.**
Questa è la difesa dal prompt injection, e ha una regola d'oro: **non lasciare mai che uno strumento IA agisca su istruzioni che trova dentro un documento, un'email, una pagina web o un foglio di calcolo.** Un modello che legge la tua casella di posta deve riassumere, non obbedire. Dove uno strumento deve agire, richiedi che un umano confermi prima che esegua. Tratta ogni documento esterno come input non affidabile, come tratti un allegato di uno sconosciuto.

**Passo 5: Dai agli agenti il minor potere possibile.**
Decidi i permessi di un agente sulla carta prima di collegarlo. Sola lettura dove puoi. Il proprio account di servizio, mai un login amministratore condiviso. Una cartella, non tutto il disco. Un limite di spesa su tutto ciò che costa denaro. Un limite di tempo. Un proprietario umano con un nome. Se non deve cancellare, non lasciargli cancellare. Dai allo strumento il più piccolo insieme di chiavi che gli consente comunque di fare il lavoro.

**Passo 6: Registra tutto e leggi i registri.**
Registra chi ha usato quale strumento IA, quando, e più o meno per cosa — poi rivedilo. Uno sguardo settimanale di quindici minuti ti mostra strumenti non approvati, volumi insoliti e schemi che puoi trasformare in policy. Niente registri significa nessuna indagine: dopo un incidente starai a indovinare.

**Passo 7: Mantieni un checkpoint umano su tutto ciò che è irreversibile.**
Qualsiasi azione che non può essere annullata — inviare denaro, cancellare record, email a un elenco clienti, firmare qualcosa — ha bisogno di un passo di approvazione umana. Non una notifica. Un'approvazione.

**Passo 8: Non trascurare le basi noiose.**
L'IA non sostituisce la sicurezza ordinaria; ci si siede sopra. Autenticazione a più fattori su ogni account che può raggiungere i dati aziendali, inclusi i portali dei fornitori. Un gestore di password così che nessuno riutilizzi le password. Aggiornamenti tempestivi. Backup testati tenuti offline. Protezione degli endpoint su ogni macchina. Se queste sono deboli, nessun controllo specifico per l'IA ti salverà.

**Passo 9: Forma con una regola, non un manuale.**
Dai al personale una frase che possa portare con sé: *se non lo metteresti in un'email a uno sconosciuto, non metterlo in uno strumento IA.* Poi di' loro cosa fare invece, e rendi quell'alternativa facile. Le regole senza alternative vengono ignorate.

**Passo 10: Pianifica il fornitore fuori servizio.**
Chiedi a ogni fornitore IA: cosa succede se siete irreperibili per una settimana? Abbi una fallback manuale per ogni processo che hai reso dipendente da loro. La disponibilità è una proprietà di sicurezza, e la storia sanitaria qui sopra è la prova.

## Etica e responsabilità

La sicurezza è una questione etica prima ancora che tecnica. Quando i clienti ti danno il loro indirizzo, il loro dettaglio sanitario o la loro informazione di pagamento, si fidano che tu li custodisca in modo sicuro. Perderli non è un incidente capitato a te; è un danno fatto a loro. È lo stesso dovere di diligenza discusso nel [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md), applicato ai sistemi anziché alle decisioni.

Tre doveri ne seguono. **Dovere di competenza:** distribuire uno strumento che non capisci non è neutrale. Se non sai dove vanno i tuoi dati, non puoi proteggerli, e "non lo sapevamo" è una difesa debole davanti a un regolatore, a un cliente o a un tribunale. Il dovere di alfabetizzazione nell'AI Act europeo, trattato nel [Capitolo 5](ch05-rules-and-legal-responsibility.md), lo rende esplicito. **Dovere di divulgazione:** se sei violato, informa le persone colpite prontamente e chiaramente. Nasconderlo per proteggere la tua reputazione trasferisce il costo del tuo problema sulle persone che si sono fidate di te; le scadenze legali sono nel [Capitolo 10](ch10-privacy-and-gdpr.md). **Proporzionalità nel monitoraggio:** registrare l'uso dell'IA protegge l'azienda, e significa anche leggere ciò che il tuo personale digita. Metti una policy scritta che dica cosa viene registrato, perché, chi può vederlo, e per quanto tempo. Monitora il flusso di dati, non la persona. La sorveglianza segreta danneggia la fiducia e spesso viola la legge locale.

Un'ultima regola: non usare strumenti IA per attaccare altri sistemi, e non testare le tue difese su dati reali o su account clienti reali. Usa un ambiente di test separato.

## Errori da evitare

1. **Trattare uno strumento IA come un motore di ricerca.** Un motore di ricerca indicizza pagine pubbliche. Un servizio IA riceve il tuo testo, lo memorizza e lo elabora sui computer di qualcun altro.
2. **Concedere permessi ampi "per farlo funzionare".** La comodità oggi è una violazione domani. Concedi il minimo e allarga solo per un bisogno provato.
3. **Lasciare che un'IA legga tutto.** Puntare un assistente su un'unità condivisa che contiene paga, file legali e record dei clienti trasforma un singolo account compromesso in esposizione totale.
4. **Nessuna registrazione.** Senza registri non puoi scoprire cosa è successo, né provare che eri in controllo.
5. **Accettare "di livello aziendale" come risposta.** Chiedi invece: addestrate sui miei dati, per quanto tempo conservate i prompt, chi sono i vostri sub-responsabili del trattamento, dove sono archiviati i dati, mi avviserete se sono violato.
6. **Ignorare il piano consumer gratuito.** Personale su account personali significa che i tuoi dati vanno da qualche parte senza contratto e senza controlli.
7. **Bloccare tutto.** Un divieto senza alternativa approvata non ferma l'uso; lo nasconde.
8. **Confondere la riservatezza con l'integrità.** Avvelenamento e manomissione non sono perdite. Proteggiti solo dai dati che escono e ti perderai i dati corrotti.
9. **Fidarti di un fornitore perché è grande.** La più grande violazione dei pagamenti sanitari della storia iniziò con un secondo fattore di login mancante.
10. **Trattare la sicurezza come un progetto una tantum.** Minacce, strumenti e personale cambiano. Rivedi la mappa ogni trimestre.

## Esercizio pratico

### 6.9 Mappa i tuoi punti di vulnerabilità

Metti da parte novanta minuti con un collega che conosce il lavoro quotidiano. Non farlo da solo.

**Parte A — Elenca i dati (20 minuti).** Scrivi ogni categoria di informazione sensibile che la tua azienda detiene. Righe tipiche: nomi e contatti dei clienti, dettagli di pagamento o bancari, numeri di identità nazionale o codice fiscale, record dipendenti e paga, CV e dati dei candidati, informazioni sanitarie o assicurative, contratti e preventivi, codice sorgente o progetti, strategia e piani finanziari.

**Parte B — Traccia ciascuno (40 minuti).** Per ogni riga rispondi per iscritto a cinque domande:

1. Dove vive? (sistema, cartella, foglio di calcolo, carta)
2. Chi può raggiungerlo? (ruoli, persone con nome, contraenti)
3. Quale strumento IA lo tocca, se uno?
4. Esce dal nostro edificio? Dove va, e sotto quale contratto?
5. Riesciamo a vedere che accade? (registrazione, sì o no)

**Parte C — Assegna un punteggio e scegli (30 minuti).** Segna ogni riga:

- **Rosso** — dati sensibili che lasciano l'azienda senza contratto e senza registrazione.
- **Ambra** — dati sensibili che restano dentro ma sono ampiamente raggiungibili, o escono sotto un contratto che non hai letto.
- **Verde** — dati a bassa sensibilità, o dati sensibili con un contratto, un filtro e registri.

Ogni riga rossa è un'azione per questo mese. Scegli le prime cinque e scrivi un proprietario e una scadenza accanto a ciascuna. Una tipica prima cinquina: autenticazione a più fattori sugli account dei fornitori, uno strumento IA approvato per il personale, una regola anti-perdita per i numeri di identità, accesso alle unità condivise ridotto alle cartelle che ogni ruolo necessita, e una regola d'uso accettabile di una pagina. Tieni la mappa su una pagina, e aggiornala ogni trimestre e ogni volta che aggiungi un nuovo strumento IA.

## Checklist

### 6.10 Le 10 azioni di sicurezza minime

- [ ] **Ogni account ha l'autenticazione a più fattori**, inclusi portali dei fornitori, email, home banking, cloud storage e login amministrativi.
- [ ] **Esiste una mappa scritta** di ogni strumento IA in uso, quali dati entrano in ciascuno, e dove sono memorizzati quei dati.
- [ ] **Esiste uno strumento IA approvato ed è più facile da usare** delle alternative non approvate.
- [ ] **Il filtro in uscita è in atto** per numeri di identità e codice fiscale, dettagli di pagamento, dati sanitari, paga, contratti e codice sorgente.
- [ ] **Nessuno strumento IA agisce su istruzioni trovate dentro i documenti che legge**; le azioni richiedono conferma umana.
- [ ] **Ogni agente IA gira con il minimo privilegio**: proprio account, sola lettura dove possibile, spesa limitata, nessun diritto di amministratore.
- [ ] **Esistono registri per l'uso dell'IA, e qualcuno li rivede settimanalmente.**
- [ ] **Le azioni irreversibili richiedono un passo di approvazione umana**, non solo una notifica.
- [ ] **La due diligence sul fornitore è fatta per iscritto**: addestramento sui tuoi dati, periodo di conservazione, sub-responsabili, ubicazione dei dati, termini di notifica delle violazioni.
- [ ] **I backup sono testati e tenuti offline, ed esiste una fallback manuale** per ogni processo che dipende da un fornitore IA.

## Punti chiave

- L'IA rende gli attacchi più economici e veloci, e moltiplica il numero di porte nella tua azienda; entrambe le cose cambiano insieme.
- La perdita più comune non è un hack — è un dipendente sollecito che incolla dati riservati in uno strumento che non ha mai verificato.
- Proteggi tutte e tre le proprietà: riservatezza (dati che escono), integrità (dati avvelenati) e disponibilità (un fornitore che si blocca).
- Le difese principali sono una mappa dei dati, un gateway controllato, il filtro in uscita, il minimo privilegio per gli agenti, e registri che qualcuno legge davvero.
- Il tuo rischio include il rischio dei tuoi fornitori, e anche quello dei loro fornitori; chiedi a chi si appoggiano prima di appoggiarti a loro.
