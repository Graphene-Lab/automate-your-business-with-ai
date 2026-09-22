# Capitolo 10 — Privacy e GDPR: quello che devi davvero sapere

## In parole semplici

GDPR sta per General Data Protection Regulation, il Regolamento generale sulla protezione dei dati. È il manuale dell'Unione Europea per gestire i dati personali, cioè qualsiasi informazione su una persona vivente che possa essere identificata. È una delle leggi sulla privacy più severe al mondo, e riguarda molte più aziende di quante la maggior parte dei titolari si aspetti.

Tutta la legge si può riassumere in un'idea sola: **se detieni informazioni su una persona, devi trattarle in modo corretto, per un motivo chiaro, conservare solo ciò che ti serve, tenerle al sicuro e rispettare ciò che quella persona ti chiede di farne.**

Sei soggetto alla legge se ti trovi nell'UE, e anche se sei fuori dall'UE ma offri beni o servizi a persone nell'UE, oppure ne osservi il comportamento. Un piccolo negozio online in un altro paese che vende a clienti in Francia ricade nel GDPR. Si chiama efficacia extraterritoriale, e sorprende molte imprese.

Perché conta per l'AI? Perché l'AI funziona con i dati, e gran parte di quei dati è personale. Nomi dei clienti, email di assistenza, curriculum, schedari dei dipendenti, visitatori del sito: tutti dati personali. Quando ne immetti anche solo una parte in uno strumento di AI, stai trattando dati personali, e le regole si applicano. Se invii quei dati a un servizio di terzi, le regole lo seguono anche fuori dalla tua porta. È qui il collegamento con il [Capitolo 9](ch09-third-party-services-and-shadow-ai.md).

Questo capitolo è la casa approfondita del GDPR in questo libro. Spiega i principi, i tipi di dati, le basi giuridiche, i tuoi obblighi e i diritti che le persone vanto nei tuoi confronti. L'AI Act europeo, una legge separata sui sistemi di AI in sé, è trattato per intero nel [Capitolo 5](ch05-rules-and-legal-responsibility.md); qui consideriamo solo dove tocca la privacy. Il lato sicurezza della protezione dei dati è nel [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md).

Una nota onesta: questa è una guida divulgativa, non un parere legale. Per decisioni reali, soprattutto oltre confine, rivolgiti a un professionista della protezione dei dati.

## Un po' di storia

**1995: la prima regola europea.** La Direttiva sulla protezione dei dati fissò i primi standard in Europa, ma ogni paese la applicò in modo diverso, creando un mosaico disomogeneo.

**27 aprile 2016: il GDPR viene adottato.** L'UE sostituì il mosaico con un unico regolamento, pensato per valere allo stesso modo in ogni Stato membro e per modernizzare le regole nell'era di internet.

**25 maggio 2018: il GDPR si applica.** Questa è la data che conta. Da quel giorno le regole sono pienamente in vigore, con multe pesanti per le violazioni gravi. Aziende di tutto il mondo hanno dovuto conformarsi o rischiare quelle sanzioni.

**Dal 2018 al 2023: l'era dell'applicazione.** Le autorità nazionali per la protezione dei dati hanno emesso multe, alcune molto elevate, per violazioni e pratiche scorrette. La privacy è diventata un tema da consiglio di amministrazione, non solo un problema degli avvocati.

**2018: l'EDPB.** È stato creato il Comitato europeo per la protezione dei dati (EDPB) per coordinare le autorità nazionali e pubblicare orientamenti, così che la legge venga applicata in modo coerente in tutta l'UE. I suoi orientamenti sono il punto di riferimento quando la legge non è chiara.

**1 agosto 2024: l'AI Act europeo entra in vigore.** Una legge separata, il Regolamento (UE) 2024/1689, ha avviato la sua introduzione graduale. Regola i sistemi di AI in base al rischio. Non sostituisce il GDPR. Dove un sistema di AI usa dati personali, entrambe le leggi si applicano insieme.

## Curiosità

### 10.9 Cosa hanno detto i regolatori europei della privacy sui modelli di AI

Nel dicembre 2024 l'EDPB, l'organismo che coordina tutti i regolatori nazionali della privacy dell'UE, ha adottato il **Parere 28/2024** sulla protezione dei dati personali nel contesto dei modelli di AI. È la dichiarazione sulla privacy più importante finora su come l'AI si concilia con il GDPR.

Alcuni punti interessano un titolare d'azienda:

**Un modello si può guardare in tre fasi.** L'EDPB divide la vita di un modello di AI in sviluppo (addestrarlo), distribuzione (metterlo al lavoro) e uso (le persone che interagiscono con esso). Ogni fase può coinvolgere dati personali, e ognuna ha le proprie domande sulla privacy. È utile perché ti dice di porre la domanda a ogni fase, non solo all'inizio.

**L'interesse legittimo può essere una base giuridica, ma non è un lasciapassare.** Il parere dice che un'azienda può contare sull'"interesse legittimo" per sviluppare o usare un modello di AI, ma solo se il trattamento è davvero necessario e una prova di bilanciamento mostra che non prevale sui diritti delle persone. Non puoi semplicemente dichiarare un interesse e ignorare le persone coinvolte.

**Un modello è "anonimo" solo se non riesci a farne uscire dati personali.** Questa è la parte tagliente. L'EDPB dice che perché un modello sia trattato come anonimo, e quindi fuori dal GDPR, deve essere molto improbabile che qualcuno possa estrarne dati personali facendogli delle domande. Se un modello può essere indotto a ripetere dettagli personali che ha memorizzato durante l'addestramento, non è davvero anonimo, e le regole sulla protezione dei dati continuano a mordere.

**I dati di addestramento sbagliati possono seguire il modello.** Il parere avverte che se un modello è stato addestrato su dati personali trattati illecitamente, questo può influire sulla liceità del suo impiego successivo, a meno che il modello non sia stato ben anonimizzato. In parole povere: un modello costruito su dati sporchi può restare sporco, e usarlo può portare quel problema nella tua azienda.

Il messaggio pratico per una piccola impresa è chiaro. Quando scegli un fornitore di AI, la domanda sulla privacy non è solo "cosa fate dei miei dati adesso", ma "su quali dati è stato addestrato questo modello, e si possono risucchiare fuori dati personali?". Questa domanda va nella tua lista di controllo dei fornitori.

## Un esempio reale di azienda

### Lo strumento per le Risorse Umane e la richiesta di accesso

Una società di medie dimensioni con 120 dipendenti adotta uno strumento di AI per filtrare le candidature di lavoro. Carica curriculum e lettere di presentazione: tutti dati personali, alcuni sensibili, perché un curriculum può rivelare lacune di salute, età, nazionalità e attività sindacale. Lo strumento classifica i candidati.

Tre mesi dopo, una candidata scartata scrive all'azienda. Presenta una **richiesta di accesso agli atti**: ai sensi del GDPR ha diritto di sapere quali dati personali l'azienda detiene su di lei e come sono stati usati. L'azienda deve rispondere, di norma entro un mese e gratuitamente.

Ora l'azienda deve rispondere a domande difficili che non si era mai posta. Dove sono il suo curriculum e la classifica dell'AI? Riesce a produrre i dati e a spiegare la logica? C'era una base giuridica per trattare il suo curriculum con questo strumento? Aveva fatto prima una valutazione dei rischi? Se lo strumento era un servizio di terzi, il contratto copriva tutto questo? Se la classifica dell'AI conta come processo decisionale automatizzato con un effetto grave su di lei, si applicano regole extra, incluso il suo diritto a non essere sottoposta a una decisione puramente automatizzata con effetti giuridici o analogamente significativi.

L'azienda si affanna perché ha adottato lo strumento prima di pensare ai dati. La lezione è l'ordine delle operazioni: devi capire i dati e la base giuridica **prima** di accendere lo strumento, non quando arriva una richiesta. Il resto di questo capitolo ti dà i pezzi per farlo.

## Come si fa

### 10.1 Il GDPR in una pagina: i principi di base

Il GDPR si fonda su pochi principi. Se li rispetti, stai rispettando gran parte della legge.

**Liceità, correttezza, trasparenza.** Ti serve un valido motivo giuridico per trattare dati personali, non devi usarli in modi che le persone riterrebbero scorretti, e devi dire alle persone cosa stai facendo.

**Limitazione della finalità.** Raccogli i dati per uno scopo chiaro e dichiarato. Non riutilizzarli dopo per qualcosa di non correlato senza una nuova base giuridica.

**Minimizzazione dei dati.** Raccogli solo ciò che ti serve davvero. Se non ti serve un numero di telefono, non chiederlo. Questo conta per l'AI: non rovesciare l'intero database in uno strumento quando basterebbe una piccola fetta.

**Esattezza.** Tieni i dati corretti e aggiornali. Le persone possono pretendere correzioni.

**Limitazione della conservazione.** Non conservare i dati personali più a lungo del necessario. Abbi un piano di cancellazione.

**Integrità e riservatezza.** Tienili al sicuro dalle violazioni. Il come si fa è nel [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md).

**Responsabilizzazione.** Devi essere in grado di *dimostrare* di conformarti, con registri, politiche e documenti. Ecco perché la modulistica nella sezione Lista di controllo non è facoltativa.

### 10.2 Dati personali, dati sensibili, dati anonimi: le differenze che contano

**Dato personale** è qualsiasi informazione su una persona vivente identificabile, direttamente o indirettamente. Un nome, un'email, un numero di telefono, una foto, un numero di documento, una posizione, un identificativo online come l'ID di un cookie. Persino una combinazione di dettagli che distingue una persona conta. Se puoi indicare una persona, è un dato personale.

**Dato sensibile** (la legge lo chiama "categorie particolari") riceve una protezione più forte. Comprende: origine razziale o etnica, opinioni politiche, convinzioni religiose o filosofiche, appartenenza sindacale, dati genetici, dati biometrici usati per identificare una persona, dati sulla salute e dati sulla vita sessuale o sull'orientamento sessuale di una persona. La regola è che trattarli è vietato, a meno che non si applichi una condizione specifica, come il consenso esplicito o un chiaro obbligo di legge. Nell'AI, fai attenzione a dove si nascondono dentro curriculum, ticket di assistenza e schedari del personale. Un chatbot che impara "questo cliente è in chemioterapia" ha toccato dati sulla salute.

**Dato anonimo** è un'informazione che non può più identificare una persona, nemmeno combinandola con altri dati. Un dato davvero anonimo è fuori dal GDPR, perché non c'è una persona identificabile. Ma il vero anonimato è difficile da ottenere. Se potessi reidentificare qualcuno, non è anonimo. È questa la differenza che inganna le persone, ed è il fuoco della sezione 10.8.

La regola pratica: tratta quasi tutto ciò che riguarda un cliente, un dipendente o un candidato come dato personale, di default. Tratta come sensibile e con cura extra tutto ciò che tocca salute, convinzioni o identità. Definisci un dato anonimo solo se hai davvero rimosso la capacità di identificare chiunque.

### 10.3 Consenso: quando serve e quando no

Il consenso è una base giuridica per il trattamento, non l'unica, e viene spesso frainteso.

Perché il consenso sia valido, deve essere **libero, specifico, informato e non ambiguo**, ed espresso da un'azione chiara. Una casella già spuntata non è consenso. Clausole sepolte non sono consenso. Un consenso per "il marketing e tutto il resto" non è un consenso valido.

Ti serve il consenso quando nessun'altra base si applica, e sempre per i dati sensibili nella maggior parte dei casi, e per certe cose come le email di marketing ai consumatori in molti paesi dell'UE.

Spesso **non** ti serve il consenso quando si applica un'altra base. Se tratti dati per eseguire un contratto che hai con il cliente, quella è la base "contratto", non il consenso. Se una legge ti impone di conservare registri, quella è "obbligo legale". Chiedere il consenso quando hai già un contratto può anzi creare problemi, perché il consenso può essere revocato in qualsiasi momento, e allora non puoi più fornire ciò che avevi promesso.

Per l'AI il consenso è delicato. Se vuoi usare i dati dei clienti per addestrare un modello, un vago "potremmo usare i tuoi dati per migliorare i nostri servizi" di solito non basta. Devi essere specifico, e devi permettere alle persone di dire no senza perdere il servizio. La via più sicura è evitare del tutto di aver bisogno di un consenso ampio: minimizza i dati, usali solo dove esiste una base reale, e preferisci input non personali o anonimizzati per l'addestramento.

### 10.4 Interesse legittimo: quando puoi usare i dati senza consenso esplicito

L'interesse legittimo è la base più flessibile e più abusata. Ti permette di trattare dati personali senza consenso quando hai un motivo d'impresa genuino e lecito, ma solo dopo un test attento.

Il test ha tre parti. **Finalità:** il tuo motivo è legittimo? Migliorare l'antifrode o la sicurezza di rete di solito lo è. **Necessità:** trattare il dato personale è davvero necessario per ottenerlo, o potresti farlo con meno dati o con dati anonimi? **Bilanciamento:** i tuoi interessi prevalgono sui diritti e le aspettative della persona? Una persona ragionevole resterebbe sorpresa o danneggiata?

Devi documentare questo test di bilanciamento. Non è una sensazione; è una valutazione scritta che puoi mostrare.

Per l'AI, l'interesse legittimo può coprire alcuni usi, per esempio usare i dati dell'assistenza clienti per migliorare la qualità del servizio, se è necessario ed equilibrato. Ma non ti permette di fare ciò che un cliente riterrebbe invadente. Addestrare un modello su dati sensibili in nome dell'"interesse legittimo" è molto difficile da giustificare. E come dice il parere dell'EDPB nella sezione Curiosità, i test di necessità e bilanciamento devono superare davvero la prova.

La regola pratica: se ti sentiresti a disagio a spiegare quell'uso ad alta voce alla persona interessata, probabilmente l'interesse legittimo non lo copre.

### 10.5 Diritti dell'interessato: accesso, rettifica, cancellazione, portabilità

Le persone vanto diritti sui loro dati, e devi essere in grado di onorarli. I principali:

**Diritto di essere informati.** Devi dire alle persone, con chiarezza, quali dati raccogli e perché, di norma in un'informativa sulla privacy.

**Diritto di accesso.** Una persona può chiedere quali dati detieni su di lei e come li usi. È la richiesta di accesso dell'esempio. Devi fornirne una copia, di norma entro un mese, gratuitamente.

**Diritto di rettifica.** Se il dato è errato, possono farlo correggere.

**Diritto alla cancellazione ("diritto all'oblio").** Possono chiederti di cancellare i loro dati, e devi farlo, a meno che una ragione legale per conservarli non prevalga, per esempio un registro fiscale che sei obbligato a trattenere.

**Diritto di limitazione del trattamento.** Possono sospendere il modo in cui usi i dati in certe situazioni, mentre si risolve una controversia.

**Diritto alla portabilità dei dati.** Possono chiedere i loro dati in un formato strutturato, di uso comune e leggibile da dispositivo automatico, così da poterli spostare altrove. Si collega al problema del lock-in nel [Capitolo 9](ch09-third-party-services-and-shadow-ai.md).

**Diritto di opposizione.** Possono opporsi a un trattamento basato sull'interesse legittimo e al marketing diretto.

**Diritti sulle decisioni automatizzate.** Ai sensi dell'articolo 22, una persona ha il diritto di non essere sottoposta a una decisione basata unicamente su un trattamento automatizzato che abbia su di lei effetti giuridici o analogamente significativi, con eccezioni limitate, e ha diritto all'intervento umano. Questo è critico per l'AI che filtra le persone per posti di lavoro, credito o servizi.

Costruisci un processo semplice e scritto per ricevere e rispondere a queste richieste nei tempi. Quando usi un'AI di terzi, assicurati che il fornitore possa aiutarti a produrre e cancellare i dati, altrimenti non potrai onorare la richiesta.

### 10.6 L'AI Act europeo: cosa cambia per la privacy

L'AI Act europeo è una legge separata dal GDPR, ed è trattato per intero nel [Capitolo 5](ch05-rules-and-legal-responsibility.md). Qui c'è solo l'angolo della privacy, così le due non vengono confuse.

Pensala così. **Il GDPR governa i dati personali che scorrono attraverso un sistema di AI. L'AI Act governa il sistema di AI in sé: il suo livello di rischio, i suoi obblighi e come può essere usato.** Se il tuo sistema di AI usa dati personali, entrambi si applicano allo stesso tempo. Non sono alternative; si sommano.

Per un sistema di AI ad alto rischio che tratta dati personali, finisci per fare due lavori collegati. Sotto l'AI Act, segui un processo di rischio e conformità per il sistema. Sotto il GDPR, ti serve una base giuridica per i dati personali e, dove il rischio è alto, una Valutazione d'impatto sulla protezione dei dati. La buona notizia è che il lavoro si sovrappone: capire i tuoi dati, documentare il tuo processo e valutare il rischio servono a entrambe le leggi.

L'AI Act insiste anche sulla qualità dei dati per i sistemi ad alto rischio: i dati di addestramento e di test devono essere pertinenti e rappresentativi, e privi di errori per quanto appropriato. Questo si allinea con il principio di esattezza del GDPR. E gli obblighi di trasparenza dell'AI Act, dire alle persone che stanno interagendo con un'AI, si affiancano agli obblighi di trasparenza del GDPR.

Il punto pratico: non trattare l'AI Act e il GDPR come un'unica lista di controllo. Fai due domande su ogni sistema di AI. *Qual è il rischio del sistema secondo l'AI Act?* E *quali dati personali vi scorrono dentro, e sono leciti secondo il GDPR?* La prima è il lavoro del Capitolo 5; la seconda è il lavoro di questo capitolo.

### 10.7 Valutazione d'impatto sulla protezione dei dati (DPIA): quando è obbligatoria e come farla

La Valutazione d'impatto sulla protezione dei dati è una revisione strutturata che fai **prima** di avviare un'attività di trattamento probabilmente ad alto rischio per le persone. Per l'AI, spesso ti servirà.

Devi fare una DPIA quando il trattamento è ad alto rischio. Inneschi chiari includono: valutazione sistematica ed estesa delle persone basata su un trattamento automatizzato che produce effetti significativi (questo copre l'AI che assegna punteggi, classifica o profila le persone); trattamento su larga scala di dati sensibili; e sorveglianza sistematica su larga scala di aree accessibili al pubblico. Anche le nuove tecnologie usate in modi nuovi alzano il rischio.

Come farla, in passi semplici:

1. **Descrivi il trattamento.** Quali dati, quale scopo, per quanto tempo, chi li vede, dove sono conservati, e se è coinvolto un terzo o un'AI.
2. **Verifica necessità e proporzionalità.** È questo il modo meno invasivo per raggiungere il tuo obiettivo?
3. **Valuta i rischi per le persone.** Non il rischio per la tua azienda: il rischio per la loro privacy, correttezza e diritti. Pensa a distorsioni, errori, raccolta eccessiva e reidentificazione.
4. **Elenca le misure per ridurre quei rischi.** Minimizza i dati, anonimizza dove possibile, aggiungi una revisione umana, metti in sicurezza il sistema, imposta una conservazione breve.
5. **Decidi.** Se un rischio elevato resta dopo le tue misure, devi consultare la tua autorità nazionale per la protezione dei dati prima di procedere.
6. **Documenta e rivedi.** Scrivilo e riesaminalo quando il sistema cambia.

Una DPIA non è un modulo da spuntare. È un esercizio di pensiero che, fatto onestamente, spesso cambia in meglio il tuo progetto.

### 10.8 Anonimizzazione e pseudonimizzazione: cosa sono e perché contano

Queste due parole suonano simili e sono molto diverse. Confonderle crea guai reali.

**Pseudonimizzazione** significa che sostituisci gli identificatori diretti con un sostituto, come un codice, e tieni la chiave che collega il codice alla persona separatamente e in modo sicuro. "Cliente 4471" invece di "Maria Rossi", con la tabella di corrispondenza sotto chiave. I dati pseudonimizzati sono **ancora dati personali** secondo il GDPR, perché con la chiave puoi reidentificare la persona. È una misura di sicurezza preziosa: riduce il rischio se i dati vengono rubati, ma non ti tira fuori dalla legge.

**Anonimizzazione** significa che rimuovi le informazioni identificative così a fondo che nessuno può reidentificare una persona, nemmeno combinando i dati con altre fonti. La legge chiede se la reidentificazione sia "ragionevolmente probabile", considerando costo, tempo e tecnologia attuale. Un dato davvero anonimo è **fuori dal GDPR**, perché non c'è una persona identificabile. Ma il vero anonimato è davvero difficile. Dataset che sembravano anonimi sono stati reidentificati incrociando altri dati pubblici.

Perché conta per l'AI: se vuoi addestrare un modello su dati senza che si applichi il GDPR, ti serve un anonimato reale, non la pseudonimizzazione. E come avverte il parere dell'EDPB, persino un modello addestrato potrebbe non essere anonimo se si possono estrarne dati personali con domande astute. Quindi "abbiamo anonimizzato i dati di addestramento" è un'affermazione che devi poter difendere, non solo dichiarare.

La regola di lavoro sicura: tratta i dati pseudonimizzati come dati personali, perché lo sono. Tratta un dato come anonimo solo se hai verificato che la reidentificazione non sia ragionevolmente possibile. In caso di dubbio, lascia attive le protezioni del GDPR.

## Etica e responsabilità

Il GDPR è il pavimento, non il soffitto. La conformità significa evitare le multe; l'etica significa fare la cosa giusta anche dove la legge tace.

**Rispetta la persona dietro il dato.** Ogni registro è la vita privata di qualcuno. Chiediti se il tuo uso ti sembrerebbe equo se fossi tu quello profilato da un'AI.

**Non nasconderti dietro "l'ha fatto il modello".** Se un'AI prende una decisione ingiusta su una persona usando i tuoi dati, la responsabilità è tua. Tieni un umano che sia proprietario del risultato, come illustra il [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md).

**Sii trasparente sull'AI.** Dì alle persone quando un'AI tocca i loro dati e cosa fa. Le sorprese erodono la fiducia più di qualsiasi difetto tecnico.

**Minimizza come abitudine morale.** Raccogliere di meno non è solo una regola legale: è rispetto. Ogni campo che non raccogli è un campo che non può essere trapelato o abusato.

**Proteggi i più vulnerabili.** I dati sensibili su salute, convinzioni o finanze meritano la massima cura. Se uno strumento non può garantirla, non metterceli dentro.

## Errori da evitare

1. **"Siamo troppo piccoli per il GDPR."** La dimensione non ti esonera. Se tratti dati personali di persone nell'UE, le regole si applicano.
2. **Credere che il consenso serva sempre, o non serva mai.** È una base fra sei. Usa quella giusta e documenta il perché.
3. **Confondere la pseudonimizzazione con l'anonimato.** I dati pseudonimizzati sono ancora dati personali e ancora nell'ambito della legge.
4. **Rovesciare l'intero database in uno strumento di AI.** Questo viola la minimizzazione dei dati e diffonde il rischio.
5. **Nessuna base giuridica per addestrarsi su dati personali.** "Migliorare i nostri servizi" di solito non basta.
6. **Ignorare i dati sensibili nascosti nei curriculum e nei ticket.** Salute, convinzioni e attività sindacale possono stare dentro documenti ordinari.
7. **Nessuna DPIA prima di un lancio di AI ad alto rischio.** Falla prima, non dopo un reclamo.
8. **Nessun processo per le richieste di accesso e cancellazione.** Se non riesci a trovare e cancellare i dati, non puoi onorare il diritto.
9. **Perdere il controllo dei dati verso un terzo.** Se il fornitore non può aiutarti a cancellare o esportare, sei esposto. Vedi il [Capitolo 9](ch09-third-party-services-and-shadow-ai.md).
10. **Trattare la legge come un progetto una tantum.** Il GDPR è continuo. Conservazione, violazioni e richieste continuano ad arrivare.

## Esercizio pratico

### 10.10 La tua lista di controllo GDPR per l'AI

Prendi mezza giornata e lavora su questo per un caso d'uso di AI che tocca dati personali.

1. **Mappa i dati.** Elenca con esattezza quali dati personali affluiscono nell'AI. Nomina ogni campo. Segna ogni categoria sensibile. (Una template di inventario dei dati è negli appendici.)
2. **Nomina la base giuridica.** Per ogni uso, scrivi quale delle sei basi si applica e perché. Se non riesci a nominarne una, fermati e ripensa la cosa.
3. **Cerca i dati sensibili.** Se è presente un dato di categoria particolare, conferma che una condizione specifica lo consenta, oppure rimuovilo.
4. **Applica la minimizzazione.** Taglia ogni campo di cui non hai strettamente bisogno.
5. **Decidi la destinazione.** I dati vanno a un terzo? Se sì, fai le domande sul fornitore del [Capitolo 9](ch09-third-party-services-and-shadow-ai.md).
6. **Fai una DPIA.** Se l'uso è ad alto rischio — profilazione, dati sensibili su larga scala, decisioni automatizzate — completa i passi della DPIA nella sezione 10.7.
7. **Pianifica i diritti.** Scrivi come gestirai le richieste di accesso, correzione e cancellazione per questi dati, inclusi i dati detenuti dal fornitore.
8. **Imposta la conservazione.** Decidi per quanto tempo conservi i dati e quando li cancelli.
9. **Verifica le regole sulle decisioni automatizzate.** Se l'AI decide sulle persone con effetto significativo, assicurati che esista un percorso di revisione umana.
10. **Documenta tutto.** Scrivi le risposte. La responsabilizzazione significa che puoi mostrare il tuo lavoro.

Se qualche passo lascia un vuoto che non riesci a riempire, quel vuoto è la tua lista di cose da fare.

## Lista di controllo

### 10.11 I documenti che devi avere

Per un sistema di AI che tocca dati personali, tieni pronti e aggiornati questi documenti.

- [ ] **Informativa sulla privacy** che spieghi con chiarezza quali dati raccogli, perché, e come è coinvolta l'AI.
- [ ] **Registro delle attività di trattamento** che descriva ogni uso dei dati personali.
- [ ] **Dichiarazione della base giuridica** per ogni finalità di trattamento, messa per iscritto.
- [ ] **Inventario dei dati** che elenchi ogni campo di dati personali e dove si trova.
- [ ] **DPIA** per ogni trattamento di AI ad alto rischio, con la decisione sul rischio residuo.
- [ ] **Test di bilanciamento** se ti basi sull'interesse legittimo.
- [ ] **Accordo di trattamento dei dati** con ogni fornitore che gestisce i tuoi dati.
- [ ] **Piano di conservazione** che indichi per quanto tempo ogni tipo di dato è conservato e quando viene cancellato.
- [ ] **Procedura per le richieste dell'interessato** per accesso, rettifica, cancellazione e portabilità, con un orologio di un mese.
- [ ] **Piano di risposta alle violazioni** che includa la notifica all'autorità entro 72 ore e alle persone interessate quando richiesto.
- [ ] **Salvaguardie per le decisioni automatizzate** con un percorso di revisione umana per le decisioni significative.
- [ ] **Contatto del Responsabile della protezione dei dati**, se il tuo trattamento lo richiede.

Tienili vivi. Un documento che non aggiorni mai è un documento che ti tradirà quando un regolatore o un cliente chiederà.

## Punti chiave

- Il GDPR si applica a qualsiasi dato personale su persone identificabili nell'UE, anche quando scorre attraverso uno strumento di AI, e raggiunge le aziende fuori dall'UE che servono clienti europei.
- Ti serve una base giuridica per ogni uso; il consenso è solo una di sei, e i dati sensibili richiedono una condizione specifica in più.
- Le persone vanto diritti reali — accesso, correzione, cancellazione, portabilità — e devi essere in grado di onorarli, anche per i dati detenuti da un fornitore terzo.
- La pseudonimizzazione non è anonimato; solo un dato che non può ragionevolmente essere reidentificato esce dal GDPR, e un modello che lascia trapelare dati personali non è anonimo.
- Per l'AI ad alto rischio, fai una DPIA prima di iniziare, e ricorda che l'AI Act e il GDPR si applicano insieme, non l'uno al posto dell'altro.
