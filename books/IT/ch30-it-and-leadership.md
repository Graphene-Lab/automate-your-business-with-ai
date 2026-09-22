# Capitolo 30 — IT e leadership

## In parole semplici

IT e leadership sono due metà di un unico lavoro: far funzionare l'azienda e guidarla nella direzione giusta. L'IT tiene in piedi sistemi, dati e rete, e li mantiene sicuri. La leadership trasforma tutto questo in decisioni — dove investire, cosa sistemare per primo, quale rischio correre. L'AI aiuta entrambe le metà. Risponde alle domande IT di routine, sorveglia le minacce, prepara i report e mette sul tavolo le opzioni, così un leader può scegliere bene.

Pensa all'IT come agli impianti e alla sicurezza di un edificio, e alla leadership come alle persone che decidono dove far andare l'edificio dopo. Quando un tubo perde, tutti lo sentono. Quando il cancello di sicurezza resta aperto, tutti sono esposti. E quando i leader devono decidere senza un quadro chiaro, tirano a indovinare. L'AI rattoppa le perdite più in fretta, sorveglia i cancelli e dà ai leader un quadro chiaro da cui decidere.

Questo capitolo copre quattro compiti: supporto interno (aiutare il personale con la tecnologia), cybersecurity (difendersi dagli attacchi), report direzionali (trasformare i dati in un quadro chiaro) e supporto alle decisioni (mettere in fila le opzioni per un leader). Ognuno è un punto in cui una piccola azienda può funzionare meglio, restare più sicura e decidere meglio.

Prima un'idea onesta: l'AI nell'IT e nella leadership è un *copilota*, non il *comandante*. Risponde, sorveglia, riassume e suggerisce. Una persona resta sempre quella che decide — se spegnere un sistema, a quale fornitore fidarsi, quale rischio accettare. Più la decisione è grande, più il giudizio umano conta. Il metodo per giudicare se tutto questo conviene sta in [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md); questo capitolo ti mostra cosa automatizzare e come. Per vedere dove si collocano IT e leadership nella mappa impatto-sforzo di tutta la tua azienda, guarda il [Capitolo 12 — Dove l'AI può aiutare la tua azienda](ch12-where-ai-can-help-your-business.md).

## Un po' di storia

**Anni '80–'90: l'help desk.** Il supporto IT è nato come help desk — un numero di telefono che il personale chiamava quando qualcosa si rompeva. Una persona registrava il problema, sistemava quello che poteva e passava in alto il resto. Funzionava, ma era lento, e le stesse semplici domande — password dimenticate, guasti alla stampante — si mangiavano la maggior parte della giornata.

**Anni '90–2000: dashboard e business intelligence.** Le aziende hanno iniziato a convogliare i dati in dashboard e strumenti di business intelligence — software che trasforma i numeri grezzi in grafici e riassunti. Per la prima volta un manager poteva vedere vendite, costi e performance su un solo schermo. Ma costruire quei report richiedeva comunque un analista, e potevi vedere solo ciò che il report era stato costruito per mostrare.

**Anni 2000: sorveglianza di sicurezza automatizzata.** Con la crescita degli attacchi, l'IT ha aggiunto strumenti di sicurezza automatici — firewall, sistemi di rilevamento delle intrusioni e di allerta che osservano la rete per attività sospette. Catturavano più di quanto potesse un umano, ma producevano anche una valanga di allarmi, quasi tutti innocui, e un analista stanco doveva distinguere la minaccia reale dal rumore.

**Anni 2010: il machine learning legge la minaccia.** Il machine learning — software che impara i modelli da molti esempi — ha cambiato la sicurezza. Invece di confrontare le firme di attacchi noti, l'AI ha imparato cosa sembrava "normale" sulla rete e ha segnalato ciò che era insolito. Ha tagliato attraverso il rumore degli allarmi individuando i pochi segnali che contavano davvero.

**Anni 2020: i grandi modelli linguistici rispondono e consigliano.** I grandi modelli linguistici — AI addestrata su enormi quantità di testo — oggi possono rispondere in linguaggio semplice alla domanda IT di un dipendente, riassumere un incidente di sicurezza, costruire un report direzionale dai dati grezzi e mettere in fila opzioni e compromessi per la decisione di un leader. È il passo più recente: un'AI che legge, spiega e consiglia su tutti e quattro i compiti insieme. L'esempio IBM sul rischio dei fornitori qui sotto mostra la stessa idea applicata al decidere quali fornitori sono sicuri.

Il percorso: da un help desk al telefono, alle dashboard, agli allarmi automatici, a un'AI che legge la minaccia e risponde alla domanda, fino a un'AI che consiglia la decisione. Ogni passo ha spostato il lavoro di routine sul software e ha lasciato agli umani il decidere e il guidare.

## Curiosità

### 30.5 Il problema più vecchio del leader: decidere senza un quadro chiaro

Da quando esistono manager, esiste la stessa lamentela: "Devo decidere, ma non riesco a vedere con chiarezza." I dati sono sparsi nei vari sistemi. Il report richiede una settimana per essere costruito. La dashboard mostra il mese scorso, non oggi. Così i leader decidono a istinto e con una speranza.

L'AI cambia questo più di quasi ogni altra cosa in questo libro. Può riunire i dati sparsi, costruire il quadro su richiesta e rispondere alla domanda di un leader con parole semplici in pochi secondi — "Quale linea di prodotto sta perdendo denaro?", "Dove sono i nostri contanti il mese prossimo?", "Quale fornitore è il rischio più grande?" Il leader decide comunque. Ma ora decide con un quadro chiaro invece che a intuito. È questa la rivoluzione silenziosa della leadership: non l'AI che prende la decisione, ma l'AI che rende la decisione *informata*. La storia IBM sul rischio dei fornitori qui sotto è esattamente questo, applicata a una decisione difficile — a quali fornitori possiamo fidarci?

## Un esempio reale di azienda

**IBM: valutazione assistita da AI del rischio di terze parti (fornitori).**

Ogni azienda che compra da fornitori esterni porta con sé il *rischio di terze parti* — il rischio che un fornitore da cui dipendi si riveli inaffidabile, insicuro o non conforme. Controllare ogni fornitore è un lavoro lento e scrupoloso. Un modo comune di verificare è un questionario dettagliato che il fornitore compila, e che un valutatore umano poi legge e mette a punteggio. Quando hai centinaia di fornitori, quel lavoro diventa un collo di bottiglia.

IBM Client Engineering ha pubblicato un caso reale su questo, intitolato "Evaluating Third Party Risk with AI". Il cliente era un istituto finanziario che eseguiva **oltre 1.000 valutazioni di fornitori all'anno**, e ogni valutazione richiedeva **circa 45 ore di lavoro** per essere completata — leggere il questionario, verificare le prove e assegnare il punteggio di rischio. È un'enorme quantità di tempo qualificato speso sullo stesso compito scrupoloso, ancora e ancora.

IBM ha usato la sua piattaforma watsonx.ai per assistere i valutatori. L'AI leggeva le risposte al questionario del fornitore e le prove a supporto, e aiutava il valutatore a capire la qualità di ciò che il fornitore aveva fornito, così l'umano poteva concentrarsi sul giudizio invece di leggere tutto da zero. La stima pubblicata indicava **una riduzione di circa il 20% del tempo di valutazione**, che su quel carico di lavoro corrispondeva a **circa 10.000 ore di lavoro risparmiate** e **circa 800.000 dollari di costo del lavoro all'anno**.

Una nota sul numero "50%". Potresti vedere questo tipo di lavoro IBM sul rischio dei fornitori citato come "una riduzione di circa il 50% del tempo". Quel numero **non** è ciò che riporta il caso pubblicato da IBM. La stima pubblicata per questo incarico è di circa il 20%, con i risparmi espressi come ~10.000 ore e ~800.000 dollari l'anno. Considera il "50%" come non verificato, e usa i numeri pubblicati — ~20% di riduzione del tempo, ~10.000 ore, ~800.000 dollari — come i numeri reali e documentati. (Fonte: IBM Client Engineering, "Evaluating Third Party Risk with AI".)

Due cose vale la pena notare. Primo, il valutatore umano è rimasto al comando. L'AI non approvava né bocciava un fornitore; aiutava l'umano a leggere più in fretta e a giudicare meglio. Secondo, il risparmio veniva dalla parte di *lettura e verifica* del lavoro — la lettura lenta e scrupolosa in cui l'AI è brava — mentre la *decisione* sul fornitore restava alla persona. È questo il modello da copiare nei tuoi lavori di rischio: lascia all'AI la lettura, tieni l'umano per il giudizio.

## Come si fa

### 30.1 Supporto interno

Il supporto interno significa aiutare il tuo personale con la sua tecnologia — la password dimenticata, la stampante che non funziona, il software da configurare. È l'help desk, ed è pieno delle stesse domande ripetute. L'AI è bravissima con le domande ripetute.

**L'assistente dell'help desk IT.** Un chatbot addestrato sulla tua base di conoscenza IT può rispondere alle domande del personale all'istante: "Come mi collego alla VPN?", "Come reimposto la mia password?", "Come installo questa app?" Questo elimina i ticket di routine che si mangiano la giornata di un team di supporto, così il team può concentrarsi sui problemi veri.

**Risolvi automaticamente i più semplici.** Alcuni ticket richiedono una semplice azione — reimpostare una password, sbloccare un account, reinstallare un'app. L'AI può farli automaticamente o preparare l'azione per l'approvazione di un umano. Il lavoro di routine sparisce dalla coda.

**Instrada subito i più difficili.** Quando il bot non riesce a risolverlo, deve passare il ticket alla persona giusta con il contesto intatto — cosa il dipendente ha già detto e provato — così l'umano non riparte da zero. Un passaggio pulito è la funzione più importante.

**Costruisci dai tuoi ticket.** Recupera gli ultimi mesi di ticket IT e trova le domande più comuni. Quelle diventano la base di conoscenza del bot. La stessa tecnologia di chatbot, applicata ai clienti invece che al personale, è trattata nel [Capitolo 27 — Assistenza e supporto clienti](ch27-customer-care-and-support.md); qui è rivolta all'interno per servire il tuo stesso team.

**Tieni un umano per il problema difficile.** L'AI gestisce la routine; una persona gestisce il guasto, il bug strano, l'incidente di sicurezza. Non lasciare mai che un bot sia l'unica strada quando qualcosa è davvero rotto. Il personale deve sempre poter raggiungere un umano.

### 30.2 Cybersecurity

La cybersecurity significa difendere i tuoi sistemi, i tuoi dati e la tua rete dagli attacchi. L'AI è ormai uno strumento centrale su entrambi i lati di questa battaglia — i difensori la usano per individuare le minacce, e la usano anche gli attaccanti — quindi è importante che tu capisca cosa può e non può fare per te.

**L'AI nota ciò che è insolito.** L'AI impara cosa sembra "normale" sulla tua rete — traffico normale, accessi normali, accesso ai dati normale — e segnala ciò che stona. Un accesso da un paese strano alle 3 di notte, un'improvvisa raffica di download di file, un dispositivo che si comporta in modo bizzarro. Sono questi piccoli segnali, visti tutti insieme sull'intera rete, il modo in cui l'AI cattura una minaccia che un umano perderebbe.

**Taglia attraverso il rumore degli allarmi.** Gli strumenti di sicurezza producono migliaia di allarmi, per lo più innocui. L'AI li ordina per priorità, così la minaccia reale sale in cima e il rumore scivola via. Questo è uno dei suoi valori più grandi: non più allarmi, ma *meno allarmi, e migliori*, che un piccolo team può davvero gestire.

**Rispondi più in fretta.** Quando l'AI segnala una minaccia reale, può anche suggerire o compiere una rapida prima azione — isolare una macchina infetta, bloccare un indirizzo sospetto — per fermare la propagazione mentre un umano indaga. La velocità conta in un attacco; i primi minuti decidono quanto danno viene fatto.

**Il quadro completo della sicurezza è un argomento a sé.** Le minacce, le difese e le abitudini umane che contano di più sono trattate in profondità nel [Capitolo 6 — Cybersecurity nell'era dell'AI](ch06-cybersecurity-in-the-ai-era.md), e il rollout sicuro nel [Capitolo 20 — Implementare l'AI in modo sicuro](ch20-implementing-ai-securely.md). Leggi quelli prima di affidarti all'AI per la tua difesa. L'AI è un potente strumento, non uno scudo magico.

**Tieni un umano per la grande decisione.** L'AI può isolare una macchina, ma è una persona che decide se spegnere un sistema, se pagare o rifiutare un riscatto, se chiamare le autorità. In un incidente reale, il giudizio umano è l'ultima linea di difesa. Non lasciare mai che l'automazione prenda da sola le grandi decisioni di sicurezza.

### 30.3 Report direzionali

Un report direzionale trasforma i dati grezzi in un quadro chiaro che un leader può leggere e su cui può agire — conto profitti e perdite, vendite per prodotto, costi per categoria, posizione di cassa. L'AI cambia chi costruisce il report e quanto in fretta.

**Il report si costruisce da sé.** Invece di un analista che ogni settimana tira i numeri in un foglio di calcolo, il report può generarsi secondo un calendario dai tuoi sistemi in tempo reale e arrivare nella casella del leader. I numeri sono sempre aggiornati, e nessuno deve ricordarsi di farlo.

**Riassunti in linguaggio semplice.** L'AI può leggere i numeri e scrivere un breve riassunto a parole: "I ricavi sono saliti dell'8% questo mese, trainati dal prodotto X; i costi sono saliti del 3%, soprattutto nelle spedizioni." Questo trasforma una tabella di cifre in una frase che un leader può davvero leggere e su cui può agire. È come avere un junior analyst che scrive il commento.

**Chiedi in linguaggio semplice.** Alcuni strumenti permettono a un leader di chiedere: "Quale linea di prodotto ha perso denaro il trimestre scorso?" e ottenere una risposta senza scrivere una formula. È utile per le domande estemporanee che prima significavano "ci guardo più tardi" e poi non succedevano mai. Il leader ottiene la risposta mentre la domanda è ancora fresca.

**Non saltare la lettura umana.** Un report automatico è un punto di partenza, non un documento decisionale finito. Leggi il riassunto, verifica che i numeri abbiano senso e aggiungi il tuo giudizio prima di agire o condividere. L'AI può riassumere con sicurezza e comunque sbagliare se i dati di base sono disordinati. Spazzatura dentro, spazzatura sicura di sé fuori.

**Mantieni stabile il formato.** Una volta fissato un layout per il report, tienilo coerente. Un formato stabile è più facile da leggere di mese in mese e più facile da controllare quando qualcosa sembra stonato. Cambialo deliberatamente, non ogni volta. (Le stesse idee di costruzione dei report, applicate alla finanza, sono nel [Capitolo 25 — Amministrazione e finanza](ch25-administration-and-finance.md).)

### 30.4 Supporto alle decisioni

Il supporto alle decisioni significa usare l'AI per mettere in fila le opzioni, le prove e i compromessi di una decisione, così un leader può scegliere bene. Non prende la decisione. Rende la decisione *informata*.

**Metti in fila le opzioni.** Per una scelta come "Dobbiamo aprire una nuova regione?" o "Quale fornitore dovremmo scegliere?", l'AI può raccogliere i dati rilevanti e presentare le opzioni affiancate, con i pro, i contro e i numeri dietro ciascuna. Il leader vede il quadro intero, non il preferito di una persona.

**Modella i compromessi.** L'AI può mostrare cosa succede sotto diverse ipotesi: "Se la domanda sale del 10%, questa opzione vince; se resta piatta, quella è più sicura." Questo trasforma un'ipotesi in un confronto di scenari, molto più utile per una grande decisione.

**Fai emergere ciò che hai mancato.** L'AI può segnalare un rischio o un'opportunità che un leader indaffarato non ha visto, perché ha guardato tutto insieme. Il caso IBM sul rischio dei fornitori qui sopra è esattamente questo: l'AI che legge le risposte di ogni fornitore così il valutatore vede il rischio con chiarezza prima di decidere.

**Tieni la decisione al leader.** L'AI consiglia; il leader decide e si assume il risultato. Un leader che segue ciecamente il modello ha smesso di guidare. Usa l'AI per informare il tuo giudizio, non per sostituirlo. La strategia dietro queste scelte è nel [Capitolo 13 — Definire una semplice strategia AI](ch13-defining-a-simple-ai-strategy.md).

**Attenzione alle sciocchezze sicure di sé.** L'AI può presentare un'opzione sbagliata con totale sicurezza. Verifica le prove dietro il suo consiglio, soprattutto per una decisione grande o insolita. Chiedi al modello di mostrare il suo ragionamento e mettilo alla prova contro ciò che sai. Fidati, ma verifica.

## Etica e responsabilità

IT e leadership portano la fiducia di tutta l'azienda, quindi qui la responsabilità è ampia.

**Tieni l'umano nella grande decisione.** L'AI consiglia su sicurezza, report e strategia. È una persona che decide su spegnere un sistema, fidarsi di un fornitore o correre un rischio. Più la decisione è grande, più è dell'umano.

**Proteggi i dati che dai in pasto ai modelli.** I dati di IT e leadership — registri di rete, bilanci, archivi dei fornitori — sono tra i più sensibili che un'azienda possieda. Tienili al sicuro e, dove conta, dentro il tuo stesso ambiente. Non immettere dati sensibili in strumenti AI pubblici senza verificare le implicazioni di sicurezza (vedi [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md) e [Capitolo 8 — Self-hosting: tieni i tuoi dati sotto controllo](ch08-self-hosting-keep-your-data-under-control.md)).

**Sorveglia l'AI di terze parti e l'AI ombra.** Fornitori e personale possono introdurre strumenti AI in azienda senza approvazione — il rischio di "shadow AI". Sappi quale AI sta girando sulla tua rete e chi l'ha approvata. Quel rischio è trattato nel [Capitolo 9 — Servizi di terze parti e shadow AI](ch09-third-party-services-and-shadow-ai.md).

**Sii onesto nei report e nei consigli.** Un riassunto AI può far sembrare ok un trimestre pessimo, e un consiglio AI può essere sicuro di sé e sbagliato. Leggi i numeri, verifica il consiglio e riporta la verità, soprattutto quando è scomoda. Il compito di un leader è vedere con chiarezza, non essere consolato.

**Tieni presente il pavimento legale.** Alcuni usi dell'AI nell'IT e nelle risorse umane toccano le regole ad alto rischio e di trasparenza dell'AI Act europeo. Conosci il tuo ruolo e i tuoi doveri prima di deployare (vedi [Capitolo 5 — Regole e responsabilità legale](ch05-rules-and-legal-responsibility.md)). La conformità è il pavimento; il tuo giudizio stabilisce lo standard sopra di esso.

**Usa l'AI per rafforzare la fiducia, non per controllare le persone.** Monitoraggio e analisi devono rendere l'azienda più sicura e meglio gestita, non diventare uno strumento per sorvegliare e fare pressione sul personale. Usali per proteggere e migliorare, non per fare la polizia.

## Errori da evitare

**Un help desk solo bot.** Personale con un problema reale bloccato dietro un bot senza una via umana. Permetti sempre il passaggio a un umano.

**Fidarsi ciecamente di un allarme di sicurezza.** Agire su un falso positivo, o peggio, ignorare una minaccia reale perché l'allarme era sepolto. Tarare il sistema e tenere un investigatore umano.

**Lasciare che l'automazione prenda la grande decisione di sicurezza.** Spegnere, pagare o escalation senza un umano. Tieni la decisione umana in un incidente.

**Saltare la lettura umana sui report.** Agire su un riassunto AI senza verificare i numeri. Leggilo tu per primo.

**Sciocchezze sicure di sé nei consigli.** Seguire un consiglio AI sbagliato ma ben formulato. Verifica le prove dietro di esso.

**Fede cieca nel modello per le grandi decisioni.** Un leader che smette di guidare e segue solo la dashboard. La decisione è del leader.

**Dare dati sensibili all'AI pubblica.** Registri di rete, bilanci e archivi dei fornitori in strumenti insicuri. Verifica prima sicurezza e privacy.

**Shadow AI che gira senza controllo.** Personale e fornitori che usano strumenti AI non approvati. Sappi cosa gira e chi l'ha approvato.

**Automatizzare un processo rotto.** Se il tuo supporto IT o il tuo reporting è un disastro, l'AI fa un disastro più veloce. Prima sistema il processo.

**Nessuna linea di base.** Non misurare il tempo dei ticket, il tasso di incidenti o il tempo dei report prima, così non puoi dimostrare il guadagno. Misura prima (vedi [Capitolo 22 — Misurare i risultati e il ROI](ch22-measuring-results-and-roi.md)).

**Citare il numero del fornitore come il tuo.** Usare il dato migliore del fornitore invece del tuo risultato misurato. Usa i tuoi numeri.

## Esercizio pratico

### 30.7 Esercizio: pianifica un'automazione IT o di leadership

Scegli un compito e pianifica la sua assistenza AI dall'inizio alla fine, con la decisione umana integrata.

**Passo 1 — Scegli il compito.** Scegline uno: supporto interno, cybersecurity, report direzionali o supporto alle decisioni. Fanne uno, non tutti.

**Passo 2 — Definisci l'obiettivo e la metrica.** Risoluzione dei ticket più rapida? Meno minacce perse? Report più veloci? Decisioni migliori? Scegli un numero da misurare.

**Passo 3 — Misura la linea di base.** Qual è quel numero adesso? Tempo medio di un ticket, incidenti persi, giorni per costruire un report, tempo di una decisione. Scrivilo.

**Passo 4 — Trova l'obiettivo costoso.** Identifica il singolo punto più doloroso — il tipo di ticket che divora più tempo, la minaccia che sfugge, il report sempre in ritardo, la decisione che continui a sbagliare. Punta a quello per primo.

**Passo 5 — Marca ogni passo.** Per ogni passo, marcalo: **lo fa l'AI** (rispondere, segnalare, riassumere, mettere in fila le opzioni), **l'umano lo verifica** (controllare l'allarme, leggere il report) oppure **l'umano lo decide** (spegnere il sistema, scegliere il fornitore, correre il rischio). Ogni grande decisione deve essere umana.

**Passo 6 — Verifica i dati e la legge.** Decidi quali dati servono all'AI, tienili al sicuro e verifica se l'uso tocca le regole ad alto rischio o di trasparenza dell'AI Act (vedi [Capitolo 5](ch05-rules-and-legal-responsibility.md)).

**Passo 7 — Collega i sistemi.** Decidi quali sistemi l'AI deve vedere — ticket, registri, bilanci, archivi dei fornitori — e come li collegherai (vedi [Capitolo 19 — Collegare l'AI ai sistemi che già usi](ch19-connecting-ai-to-systems-you-already-use.md)).

**Passo 8 — Lancia in piccolo e misura.** Provalo prima su un team, un sistema o un report. Confronta la metrica con la linea di base. Scala solo ciò che dimostra di funzionare.

Fai bene un solo compito. L'analisi dell'obiettivo costoso nel passo 4 ha valore di per sé — ti mostra dove il tuo lavoro di IT e leadership perde davvero più tempo o corre più rischio, il che è utile anche prima di comprare qualsiasi strumento.

## Checklist

### 30.8 Checklist IT e leadership

Prima di automatizzare un compito IT o di leadership, verifica queste cose.

- [ ] **Hai misurato la linea di base** — tempo dei ticket, tasso di incidenti, tempo dei report, tempo di una decisione.
- [ ] **Hai puntato al punto più costoso per primo**, non al più facile.
- [ ] **Un umano prende ogni grande decisione** — spegnimento del sistema, fiducia al fornitore, accettazione del rischio.
- [ ] **Il bot dell'help desk passa a un umano** con il contesto completo.
- [ ] **Gli allarmi di sicurezza sono tarati** così la minaccia reale sale e il rumore scende.
- [ ] **Un umano indaga su ogni vero incidente di sicurezza.**
- [ ] **I report direzionali sono letti da un umano** prima di agire o condividerli.
- [ ] **Verifichi le prove dietro il consiglio AI**, soprattutto per le grandi decisioni.
- [ ] **I dati sensibili sono tenuti al sicuro**, non inviati a servizi AI pubblici.
- [ ] **Sai quale AI gira sulla tua rete** e chi l'ha approvata (niente shadow AI).
- [ ] **Hai verificato l'AI Act** per eventuali doveri ad alto rischio o di trasparenza.
- [ ] **Sistemi il processo rotto prima di automatizzarlo.**
- [ ] **Riporti i tuoi numeri misurati**, non il caso migliore del fornitore.

Se una casella è vuota, il rischio — per i tuoi sistemi, i tuoi dati o le tue decisioni — è ancora tuo. Riempila prima di far avvicinare l'AI ai comandi.

## Punti chiave

- L'AI nell'IT e nella leadership è un copilota: risponde alle domande di supporto, individua le minacce, costruisce report e mette in fila le opzioni, mentre un umano conserva ogni grande decisione.
- Il caso IBM sul rischio dei fornitori (IBM Client Engineering, "Evaluating Third Party Risk with AI") ha aiutato un istituto finanziario con oltre 1.000 valutazioni l'anno da ~45 ore ciascuna, con una stima pubblicata di ~20% di riduzione del tempo, ~10.000 ore e ~800.000 dollari risparmiati all'anno — il numero "circa 50%" non è ciò che riporta la fonte pubblicata.
- Il risparmio viene dal lasciare all'AI la lenta lettura e verifica mentre l'umano conserva il giudizio; lo stesso modello funziona su supporto, sicurezza, report e decisioni.
- Tieni i dati sensibili al sicuro, sappi quale AI gira sulla tua rete e verifica le regole ad alto rischio e di trasparenza dell'AI Act prima di deployare.
- Misura la tua linea di base, tieni un umano in ogni grande decisione e tratta la legge come il pavimento e il tuo giudizio come lo standard sopra di esso.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come lo stesso compito appare con AgentBridge. Ogni riquadro mostra il risultato finito e l'unica riga che digiti per ottenerlo.

### Verbali di riunione puliti

![Verbali di riunione ordinati con decisioni e azioni](../../assets/examples/meeting-minutes.png)
*Verbali di riunione ordinati con decisioni e azioni*

**Cosa chiedi:** `Trasforma queste note approssimative in verbali di riunione puliti con un elenco di decisioni e azioni: [incolla le note]`

L'agente trasforma le tue note disordinate in verbali strutturati: cosa è stato discusso, cosa è stato deciso e un elenco di azioni con i responsabili. Puoi inviarli subito al team.

*Suggerimento: Incolla le tue note come sono — l'agente sistema l'ordine e le parole.*

---

### Una revisione trimestrale del consiglio

![Una diapositiva di una presentazione di revisione trimestrale](../../assets/examples/board-review.png)
*Una diapositiva di una presentazione di revisione trimestrale*

**Cosa chiedi:** `Crea una presentazione di revisione trimestrale: risultati, punti salienti, sfide e piano per il prossimo trimestre.`

L'agente assembla la presentazione di revisione con i risultati, i successi, i problemi e il piano — disposta così che la riunione proceda veloce.

*Suggerimento: Allega il tuo foglio dei KPI e l'agente mette i grafici nelle diapositive.*

---

### Vedi tutti i tuoi agenti a colpo d'occhio

![La vista OfficeManager dei tuoi agenti](../../assets/examples/officemanager-view.png)
*La vista OfficeManager dei tuoi agenti*

**Cosa chiedi:** `(browser) Apri la vista OfficeManager.`

OfficeManager mostra i tuoi agenti in una sola pagina semplice, così puoi vedere cosa sta girando e a che punto sono le cose.

*Suggerimento: Un modo rapido per tenere d'occhio più di un assistente alla volta.*

---

### Un briefing che puoi ascoltare

![Un briefing audio pronto per essere riprodotto](../../assets/examples/audio-briefing.png)
*Un briefing audio pronto per essere riprodotto*

**Cosa chiedi:** `Trasforma il riassunto di questa settimana in un breve briefing audio che posso ascoltare mentre vado al lavoro.`

L'agente converte il riassunto scritto in un chiaro briefing audio, così il tuo tragitto diventa tempo utile.

*Suggerimento: Pianifica il riassunto settimanale e la sua versione audio insieme.*

<!-- END agentbridge-examples -->
