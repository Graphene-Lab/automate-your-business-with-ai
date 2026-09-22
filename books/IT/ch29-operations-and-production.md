# Capitolo 29 — Operazioni e produzione

## In parole semplici

Le operazioni sono il motore di un'azienda. Sono tutto ciò che trasforma input in output: produrre un prodotto, spostarlo, tenere le macchine in funzione, controllare la qualità e tenere le persone al sicuro. La produzione è la parte delle operazioni che effettivamente fa la cosa. Quando il motore gira bene, i clienti ricevono ciò che hanno ordinato, in tempo, senza difetti. Quando inceppa, tutto a valle lo sente.

Pensa alla tua operazione come a un pavimento di fabbrica, che tu produca gingilli o consegni servizi. Le macchine girano, le merci si muovono, le persone lavorano, e qualcosa può sempre andare leggermente storto — una macchina sta per guastarsi, un lotto ha un difetto, una consegna farà tardi, un operaio in un punto pericoloso. Un buon operatore vede queste cose presto. L'IA aiuta guardando tutto in una volta e segnalando i piccoli segnali che un occhio umano stanco perde.

Questo capitolo copre quattro lavori: manutenzione predittiva (riparare le macchine prima che si rompano), controllo qualità (cogliere i difetti automaticamente), logistica (spostare merci e informazioni efficientemente) e sicurezza sul lavoro (tenere le persone lontano dal pericolo). Ognuno è un posto dove una piccola azienda può tagliare gli sprechi, alzare la qualità e proteggere il suo personale.

Un'idea onesta prima di tutto: l'IA nelle operazioni è un *osservatore e un aiutante*, non un pilota automatico che gestisce il pavimento da solo. Sente, prevede e suggerisce. Una persona decide ancora quando fermare una linea, quando scartare un lotto, e quando mandare qualcuno a casa perché non è sicuro. Il metodo per giudicare se tutto questo si ripaga vive nel [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md); questo capitolo ti mostra cosa automatizzare e come. Per vedere dove siedono le operazioni sulla mappa impatto-sforzo di tutta la tua azienda, guarda il [Capitolo 12 — Dove l'IA può aiutare il tuo business](ch12-where-ai-can-help-your-business.md).

## Un po' di storia

**Anni 1900-1950: la linea di montaggio e la manutenzione preventiva.** La produzione moderna iniziò con la linea di montaggio in movimento, che divideva il lavoro in piccoli passi ripetibili. Accanto ad essa arrivò la manutenzione *preventiva* — l'abitudine di revisionare una macchina su un calendario fisso, come cambiare l'olio di un'auto ogni qualche migliaio di miglia, che ne avesse bisogno o no. Questo ridusse i guasti ma sprecava assistenza su macchine che stavano bene.

**Anni 1960-1980: automazione e controllo qualità.** Le fabbriche aggiunsero macchine automatizzate e un controllo qualità formale — ispezionare i prodotti contro uno standard e separare il buono dal cattivo. Metodi statistici di qualità coglievano i difetti nei lotti. Questo alzò la qualità ma faceva ancora affidamento su umani per ispezionare e su regole fisse per revisionare le macchine.

**Anni 1990: sensori e la catena di fornitura digitale.** Sensori economici permisero alle macchine di riportare la propria condizione — temperatura, vibrazione, ore di funzionamento. Le catene di fornitura diventarono digitali, con software che tracciava le merci dal fornitore al cliente. Per la prima volta, un operatore poteva vedere, su uno schermo, cosa stava succedendo sul pavimento e attraverso la catena di fornitura. Ma i dati erano per lo più letti a mano.

**Anni 2000: il machine learning prevede il guasto.** Il machine learning — software che impara schemi da molti esempi — cambiò la manutenzione. Invece di revisionare su un calendario fisso, potevi imparare dai dati dei sensori quando una macchina *effettivamente* stava per guastarsi. Uno schema di vibrazione crescente che un umano non poteva sentire divenne un chiaro avviso con giorni di anticipo. Questa fu la nascita della manutenzione *predittiva*.

**Anni 2010: la computer vision ispeziona la qualità.** La computer vision — IA che legge ciò che una camera vede — iniziò a ispezionare i prodotti automaticamente. Una camera poteva individuare una crepa, un graffio o una parte mancante più velocemente e più costantemente di un ispettore umano, e senza stancarsi. Il controllo qualità si spostò dal campionamento al controllo di ogni unità.

**Anni 2020: gli agenti gestiscono il flusso di lavoro.** Grandi modelli linguistici e agenti IA — software che prende un intero compito e lo porta attraverso parecchi passi — ora gestiscono parti del flusso operativo stesso: leggere una richiesta, prelevare dati dai sistemi backend ed eseguire il passo successivo. L'esempio SOK Finance qui sotto è esattamente questo: agenti IA che gestiscono le operazioni di servizio quotidiane di un centro di servizi finanziari, con umani che supervisionano.

L'arco: da calendari fissi, a ispezione manuale, a dati dei sensori, a IA che prevede e vede, ad agenti che agiscono. Ogni passo ha spostato l'osservare e il lavoro di routine al software e ha lasciato agli umani decidere e intervenire.

## Curiosità

### 29.5 Il centro di servizi che mise agenti IA in prima linea

Quando sentiamo "operazioni e produzione", immaginiamo una fabbrica. Ma operazioni significa anche il centro di servizi che tiene in funzione un'azienda — il posto dove arrivano le richieste e qualcuno deve agire su di esse in fretta.

SOK Finance, in Finlandia, gestisce un centro di servizi chiamato Palveluässä che fornisce servizi di gestione finanziaria e paghe per il Gruppo S — una rete finlandese di proprietà dei clienti di aziende di vendita al dettaglio e servizi con circa 2.000 punti vendita. Ogni giorno arrivano richieste: "Mandatemi una copia di questa fattura", "Cambiate la scadenza di questo pagamento". Routine, ad alto volume e sensibili al tempo.

La curiosità è cosa l'azienda ne ha fatto. Invece di assumere più persone per rispondere alle stesse richieste, misero *agenti* IA in prima linea per gestire quelli di routine, così il personale umano poteva concentrarsi sui casi che richiedevano giudizio. Quel cambiamento — da umani che fanno ogni richiesta ad agenti che fanno la routine e umani che supervisionano — è la stessa silenziosa rivoluzione che avvenne sul pavimento della fabbrica, ora applicata a un centro di servizi. La storia completa, con la fonte reale, è qui sotto.

## Un esempio aziendale reale

**SOK Finance: agenti IA che gestiscono il flusso di lavoro del centro di servizi.**

SOK Finance gestisce il centro di servizi Palveluässä, che fornisce servizi di gestione finanziaria e paghe per il Gruppo S, una rete finlandese di proprietà dei clienti di aziende di vendita al dettaglio e servizi con circa 2.000 punti vendita. Il centro di servizi gestisce un flusso costante di richieste di routine da tutta quella rete — cose come chiedere una copia di una fattura o cambiare la scadenza di un pagamento. Ogni richiesta è piccola, ma insieme sono un carico di lavoro grande e ripetitivo che deve essere gestito velocemente e in modo coerente.

Secondo un comunicato stampa di CGI (Helsinki, 23 aprile 2026), CGI ha progettato, implementato e distribuito una **soluzione multi-agente IA costruita su AWS Bedrock** per SOK Finance, portando l'IA all'uso produttivo in amministrazione finanziaria e servizio clienti. Una soluzione "multi-agente" significa che parecchi agenti IA lavorano insieme su un compito, ciascuno gestendo un passo. In questo caso, gli agenti elaborano i messaggi di servizio clienti in arrivo, recuperano i dati necessari dai sistemi backend e eseguono automaticamente parti del processo.

Il comunicato descrive la soluzione come significativamente più veloce nei processi di routine come **richieste di copia fattura e cambi di scadenza**, e come un miglioramento di efficienza e coerenza rispetto alla precedente gestione manuale. CGI fu responsabile della progettazione, dell'implementazione, della distribuzione e dell'integrazione con i sistemi chiave di SOK Finance.

Due cose vale la pena notare. Primo, il ruolo umano si sposta dal *fare ogni richiesta* al *supervisionare gli agenti e gestire le eccezioni*. Gli agenti prendono la routine; le persone prendono l'insolito e il sensibile. Secondo, la vittoria è la coerenza tanto quanto la velocità — un agente segue gli stessi passi accurati ogni volta, dove una persona stanca in un pomeriggio affollato potrebbe scivolare.

Una nota sulla fonte e sui numeri: le cifre sopra vengono dall'annuncio pubblicato di CGI. Il comunicato descrive i risultati in termini qualitativi — processi più veloci, migliore coerenza — e non pubblica una percentuale dura per tempo risparmiato o costo ridotto. Tratta l'esito come l'esperienza riportata dall'azienda, e ricorda che i tuoi numeri dipenderanno dal tuo volume e dai tuoi sistemi. Il punto del caso è il *modello*: agenti IA che gestiscono un flusso di servizio di routine in produzione, con umani che supervisionano, alla scala di una rete di 2.000 punti vendita.

## Come si fa

### 29.1 Manutenzione predittiva

La manutenzione predittiva significa riparare una macchina *prima* che si rompa, prevedendo il guasto dai dati invece di aspettarlo o revisionare su un calendario fisso.

**Il vecchio modo e il suo costo.** Tradizionalmente avevi due scelte: far girare una macchina finché non guastava (e pagare una fermata non pianificata), o revisionarla su un calendario fisso (e sprecare denaro revisionando macchine che stavano bene). Entrambe perdono. Un guasto non pianificato ferma la produzione nel momento peggiore e costa molto più di una riparazione pianificata.

**Come l'IA prevede.** Metti sensori sulla macchina per misurare cose come vibrazione, temperatura, suono e ore di funzionamento. L'IA impara lo schema normale e individua i primi segni di problema — una vibrazione che sale lentamente, una temperatura che corre un po' calda. Quei piccoli cambiamenti spesso appaiono giorni prima di un guasto. L'IA ti avvisa in tempo per riparare la macchina durante una fermata pianificata, non in mezzo a una corsa.

**Cosa risparmia.** Il grande risparmio è evitare i tempi di inattività non pianificati — il guasto a sorpresa che ferma tutto. Una riparazione pianificata un martedì pomeriggio è economica; un guasto durante il tuo ordine più grande del mese è costoso. La manutenzione predittiva trasforma il secondo nel primo.

**Inizia piccolo.** Non ti servono sensori su ogni macchina. Inizia con l'una o due macchine il cui guasto fa più male — il collo di bottiglia, quella con il lungo tempo di riparazione, quella che ferma tutta la linea. Mettici alcuni sensori e osserva. Prova il valore lì prima di espanderti.

**L'umano decide la fermata.** L'IA segnala il rischio; una persona decide quando abbattere la macchina. Non lasciare che il sistema fermi la produzione da solo senza un umano che confermi la chiamata. L'avviso è il valore; la decisione resta umana.

### 29.2 Controllo qualità

Il controllo qualità significa verificare che un prodotto soddisfi il suo standard e cogliere i difetti prima che il prodotto raggiunga il cliente. L'IA cambia il controllo qualità dal *campionamento* al *controllo di ogni unità*, e dagli *occhi stanchi* a *occhi costanti*.

**La computer vision ispeziona.** Una camera più IA può guardare ogni prodotto sulla linea e individuare una crepa, un graffio, una parte mancante, un'etichetta sbagliata o una cucitura difettosa. Controlla ogni unità, non solo un campione, e non si stanca né si annoia. Un ispettore umano che controlla migliaia di unità al giorno perderà cose; la camera no.

**La coerenza è la vittoria.** Gli umani variano. Una persona è più acuta al mattino, più lenta dopo pranzo, e facilmente influenzata da ciò che ha visto l'ultima volta. L'IA applica lo stesso standard a ogni unità, tutto il giorno. Quella coerenza vale molto in un'azienda dove un difetto che raggiunge un cliente costa un reso, un reclamo o una reputazione.

**Coglilo presto.** Prima cogli un difetto, più è economico. Un difetto colto alla macchina che l'ha fatto costa un pezzo. Lo stesso difetto colto all'assemblaggio finale costa una rilavorazione. Colto dal cliente, costa un reso e fiducia. L'IA a ogni postazione coglie i problemi alla fonte, non alla fine.

**Inizia dal difetto costoso.** Non provare a ispezionare tutto all'inizio. Trova il difetto che ti costa di più — quello che causa più resi o reclami — e metti un controllo di visione su quello. Prova che coglie il problema costoso, poi aggiungi altri controlli.

**Tieni un umano per la decisione di giudizio.** L'IA può segnalare un'unità sospetta; una persona decide se è davvero difettosa, specialmente per i casi borderline. Non lasciare che un sistema di visione scarti buon prodotto perché troppo severo. Rivedi gli scarti e regola la soglia.

### 29.3 Logistica

La logistica è il movimento di merci e informazioni: far arrivare la cosa giusta nel posto giusto al momento giusto, al costo più basso. È un rompicapo di rotte, scorte, tempi e fornitori, e l'IA è molto brava in rompicapi come questo.

**Ottimizzazione di rotte e consegne.** L'IA può pianificare rotte di consegna che risparmiano miglia, carburante e tempo, tenendo conto del traffico, delle finestre di consegna e della dimensione del carico. Per un'azienda con una flotta, anche un piccolo risparmio per rotta si somma in fretta nell'arco di un anno.

**Previsione di scorte e domanda.** L'IA guarda la tua storia di vendite e prevede cosa ti servirà e quando, così tieni abbastanza scorta senza sovra-acquistare. Troppa poca scorta significa una vendita persa; troppa significa liquidità immobilizzata e spreco. L'IA bilancia le due cose imparando i tuoi schemi e la stagionalità.

**Individua il collo di bottiglia.** L'IA può vedere dove le merci rallentano — un fornitore sempre in ritardo, un passo di magazzino che si intasa, una rotta che sfora sempre. Vedere il collo di bottiglia è il primo passo per sistemarlo. Tutto il valore è rendere visibile il ritardo invisibile.

**Collega i sistemi.** La IA logistica funziona al meglio quando può vedere i tuoi ordini, le tue scorte e le tue consegne insieme. Collegare l'IA ai sistemi che già usi — i tuoi ordini, il tuo inventario, il tuo tracciamento — è ciò che rende il quadro completo. Il come per quella connessione è nel [Capitolo 19 — Collegare l'IA a sistemi che già usi](ch19-connecting-ai-to-systems-you-already-use.md).

**Tieni un umano per l'eccezione.** L'IA pianifica la routine; una persona gestisce la sorpresa — lo sciopero, la tempesta, il fornitore che viene meno. Non lasciare che un piano ottimizzato finisca contro un'interruzione del mondo reale senza un umano pronto a scavalcarlo. Il piano è un punto di partenza, non una camicia di forza.

### 29.4 Sicurezza sul lavoro

La sicurezza sul lavoro significa tenere le persone lontano dal pericolo. L'IA può sorvegliare condizioni pericolose e comportamento pericoloso e avvisare prima che accada un incidente. Questo è uno degli usi più preziosi dell'IA, perché ciò che protegge è una persona.

**La computer vision sorveglia i pericoli.** Camere più IA possono individuare un operaio senza il corretto equipaggiamento protettivo, una persona in piedi in una zona pericolosa, una fuoriuscita sul pavimento, o un'uscita di emergenza bloccata. Quando ne vede uno, solleva un allarme così il pericolo viene sistemato prima che qualcuno si faccia male.

**Prevedi il momento rischioso.** L'IA può imparare quando gli incidenti sono più probabili — un certo turno, una certa macchina, una certa ora del giorno in cui le persone sono stanche — e aumentare la sorveglianza allora. È come avere un responsabile della sicurezza che non sbatte mai le palpebre e vede tutto il pavimento in una volta.

**Una linea legale seria: non leggere le emozioni.** L'IA che inferisce le *emozioni* di un lavoratore dal suo volto o dalla sua voce è vietata sul luogo di lavoro secondo l'AI Act europeo. La visione di sicurezza riguarda *pericoli ed equipaggiamento*, non come un lavoratore *si sente*. Tieni la camera sul pavimento e sulla macchina, non sull'umore della persona. L'elenco completo delle pratiche vietate è nel [Capitolo 5 — Regole e responsabilità legale](ch05-rules-and-legal-responsibility.md).

**Dillo ai tuoi lavoratori.** Se usi un monitoraggio di sicurezza basato su IA che riguarda i lavoratori, devi informare i tuoi lavoratori e i loro rappresentanti prima di iniziare, come la legge richiede per l'IA ad alto rischio sul luogo di lavoro. Sii aperto su cosa sorvegliano le camere e perché. Il segreto rompe la fiducia. La regola dell'avviso ai lavoratori è trattata nella Curiosità di questo capitolo e nel [Capitolo 5](ch05-rules-and-legal-responsibility.md).

**Usala per proteggere, non per punire.** I dati di sicurezza dovrebbero rendere il luogo di lavoro più sicuro — sistema il pericolo, cambia il processo, forma il team. Non dovrebbero diventare uno strumento per disciplinare individui per ogni piccolo errore. Usali per trovare e rimuovere il pericolo, non per costruire un caso contro un lavoratore.

## Etica e responsabilità

Le operazioni toccano la sicurezza e l'ambiente, quindi le poste etiche sono reali e concrete.

**Le decisioni di sicurezza restano umane.** L'IA può avvisare di un pericolo, ma una persona decide quando fermare una linea o mandare qualcuno a casa. Non lasciare mai che un sistema prenda una decisione critica per la sicurezza senza un umano nel ciclo. Un "tutto libero" falso può ferire qualcuno.

**Rispetta la privacy e i diritti dei lavoratori.** Camere e sensori sul luogo di lavoro sorvegliano le persone. Usali per la sicurezza e le operazioni, non per la sorveglianza. Dì ai lavoratori cosa è sorvegliato e perché, e segui le regole sulla privacy nel [Capitolo 10 — Privacy e GDPR](ch10-privacy-and-gdpr.md).

**Non leggere mai le emozioni.** Il riconoscimento delle emozioni sul luogo di lavoro è vietato. Tieni il monitoraggio su pericoli ed equipaggiamento, mai sui sentimenti di un lavoratore.

**Proteggi i dati operativi.** I dati dei sensori, i calendari di produzione e i registri della catena di fornitura sono sensibili e preziosi. Tienili al sicuro e, dove conta, dentro il tuo ambiente. Le basi della sicurezza sono nel [Capitolo 6 — La cybersecurity nell'era dell'IA](ch06-cybersecurity-in-the-ai-era.md), e l'opzione di self-hosting nel [Capitolo 8 — Self-Hosting: tieni i tuoi dati sotto controllo](ch08-self-hosting-keep-your-data-under-control.md).

**Sii onesto sui risultati.** Un numero di qualità o efficienza che sembra troppo bello andrebbe controllato prima di riportarlo. Riporta le cifre reali, incluse le mancanze, così puoi sistemare ciò che è ancora rotto.

**Usa i dati per migliorare, non per punire.** I dati operativi e di sicurezza dovrebbero rendere il lavoro migliore e più sicuro per tutti. Quando diventano un bastone per percuotere gli individui, avvelenano il luogo di lavoro e nascondono i veri problemi.

## Errori da evitare

**Aspettare il guasto.** Restare con il "far girare finché non si rompe" quando una riparazione pianificata era economica e prevedibile. Prevedi e agisci presto.

**Sensori senza un piano.** Raccogliere dati su cui non agisci mai. Inizia dalla macchina che fa più male e lega ogni sensore a una decisione.

**Lasciare che l'IA fermi o scarti da sola.** Nessun controllo umano su una fermata linea o uno scarto prodotto. Tieni la decisione umana.

**Controlli di visione troppo severi.** Un sistema di qualità che scarta buon prodotto perché la soglia è troppo stretta. Rivedi gli scarti e regolalo.

**Ispezionare il difetto sbagliato.** Mettere la visione su un problema economico mentre quello costoso scivola via. Prendi di mira il difetto costoso prima.

**Un piano che ignora il mondo reale.** Lasciare che un piano logistico ottimizzato finisca contro un'interruzione senza override umano. Tieni una persona pronta.

**Riconoscimento delle emozioni al lavoro.** Usare l'IA per leggere i sentimenti dei lavoratori. È vietato e sbagliato.

**Monitoraggio segreto.** Non dire ai lavoratori prima che il monitoraggio di sicurezza o operazioni basato su IA inizi. Questo viola la legge e la fiducia.

**Scivolamento della sorveglianza.** Usare i dati di sicurezza e operazioni per sorvegliare e punire individui invece di rimuovere i pericoli.

**Automatizzare un processo rotto.** Se la linea o la catena di fornitura è un disastro, l'IA fa un disastro più veloce. Sistema il processo prima.

**Nessuna linea di base.** Non misurare tempi di inattività, tasso di difetti o tempo di consegna prima, così non puoi provare il guadagno. Misura prima (vedi [Capitolo 22 — Misurare risultati e ROI](ch22-measuring-results-and-roi.md)).

**Sovrapromettere i numeri.** Citare la cifra migliore del fornitore come tuo risultato. Usa i tuoi numeri misurati.

## Esercizio pratico

### 29.7 Esercizio: pianifica un'automazione delle operazioni

Scegli un lavoro operativo e pianifica il suo supporto IA dall'inizio alla fine, con la sicurezza e la decisione umana costruite dentro.

**Passo 1 — Scegli il lavoro.** Scegline uno: manutenzione predittiva, controllo qualità, logistica, o sicurezza sul lavoro. Fanne uno, non tutti.

**Passo 2 — Definisci l'obiettivo e la metrica.** Meno tempi di inattività? Meno difetti? Consegna più veloce? Meno incidenti di sicurezza? Scegli un numero da misurare.

**Passo 3 — Misura la linea di base.** Cos'è quel numero ora? Ore di tempo di inattività non pianificato, tasso di difetti, consegne puntuali, incidenti al mese. Scrivilo.

**Passo 4 — Trova il bersaglio costoso.** Identifica il singolo fallimento più costoso in quel lavoro — la macchina il cui guasto fa più male, il difetto che costa di più, la rotta che arriva sempre in ritardo, il pericolo che causa più danno. Prendi di mira quello prima.

**Passo 5 — Segna ogni passo.** Per ogni passo, segnalo: **l'IA lo fa** (sentire, prevedere, ispezionare, pianificare), **l'umano lo revisiona** (confermare l'avviso, controllare lo scarto), o **l'umano lo decide** (fermare la linea, scartare il lotto, mandare qualcuno a casa). Ogni decisione critica per la sicurezza deve essere umana.

**Passo 6 — Controlla la linea legale.** Se il lavoro coinvolge il monitoraggio dei lavoratori, conferma che stai sorvegliando pericoli ed equipaggiamento, non emozioni, e pianifica come informerai i lavoratori e i loro rappresentanti prima di iniziare.

**Passo 7 — Collega i dati.** Decidi quali sistemi l'IA deve vedere — sensori, inventario, tracciamento — e come li collegherai (vedi [Capitolo 19](ch19-connecting-ai-to-systems-you-already-use.md)).

**Passo 8 — Lancia piccolo e misura.** Eseguilo su una macchina, una linea, o una rotta prima. Confronta la metrica con la linea di base. Scala solo ciò che prova di funzionare.

Fai un lavoro bene. L'analisi del bersaglio costoso nel passo 4 è preziosa di per sé — ti mostra dove la tua operazione effettivamente perde più denaro o causa più danno, il che è utile anche prima di comprare qualsiasi strumento.

## Checklist

### 29.8 Checklist operazioni e produzione

Prima di automatizzare qualsiasi compito operativo, controlla queste.

- [ ] **Hai misurato la linea di base** — tempi di inattività, tasso di difetti, tempo di consegna, incidenti di sicurezza.
- [ ] **Hai preso di mira il fallimento più costoso prima**, non il più facile.
- [ ] **Un umano prende ogni decisione critica per la sicurezza** — fermare una linea, scartare un lotto.
- [ ] **La manutenzione predittiva è legata a una vera azione**, non solo dati raccolti.
- [ ] **I controlli di qualità sono regolati** così non scartano buon prodotto.
- [ ] **La IA logistica può vedere i tuoi ordini, scorte e consegne insieme.**
- [ ] **Un umano può scavalcare il piano ottimizzato** quando il mondo reale lo interrompe.
- [ ] **Il monitoraggio di sicurezza sorveglia pericoli ed equipaggiamento, mai emozioni** (il riconoscimento delle emozioni è vietato).
- [ ] **Hai informato i lavoratori e i loro rappresentanti** prima di qualsiasi monitoraggio IA che li riguarda.
- [ ] **I dati operativi sono tenuti al sicuro**, non inviati a servizi IA pubblici.
- [ ] **Usi i dati per rimuovere pericoli e migliorare il processo**, non per punire individui.
- [ ] **Sistemi il processo rotto prima di automatizzarlo.**
- [ ] **Riporti i tuoi numeri misurati**, non il caso migliore del fornitore.

Se una casella è vuota, il rischio — per il tuo prodotto, la tua gente, o la tua fiducia — è ancora tuo. Riempila prima di lasciare che l'IA si avvicini al pavimento.

## Punti chiave

- L'IA nelle operazioni è un osservatore e aiutante: sente, prevede, ispeziona e pianifica, mentre un umano mantiene ogni decisione critica per la sicurezza.
- Il caso SOK Finance (un annuncio CGI) mise IA multi-agente su AWS Bedrock in produzione live in un centro di servizi che serve una rete di ~2.000 punti vendita, accelerando richieste di routine come copie fattura e cambi di scadenza, con umani che supervisionano le eccezioni.
- La manutenzione predittiva trasforma un guasto a sorpresa in una riparazione pianificata economica; il controllo qualità con computer vision controlla ogni unità in modo coerente invece di campionare con occhi stanchi.
- Nella sicurezza sul lavoro, monitora pericoli ed equipaggiamento protettivo — mai le emozioni dei lavoratori, che l'AI Act UE vieta — e avvisa i lavoratori prima di qualsiasi monitoraggio che li riguarda.
- Prendi di mira il fallimento più costoso prima, tieni un override umano per le interruzioni del mondo reale, e misura la tua linea di base prima di fidarti del numero di qualsiasi fornitore.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come appare lo stesso lavoro con AgentBridge. Ogni riquadro mostra il risultato finito e la singola riga che digiti per ottenerlo.

### Tieni l'inventario in ordine

![Un foglio di inventario con gli articoli a scorta bassa evidenziati](../../assets/examples/inventory-list.png)
*Un foglio di inventario con gli articoli a scorta bassa evidenziati*

**Cosa chiedi:** `Crea un foglio di inventario con articolo, quantità, livello di riordino e fornitore, ed evidenzia ciò che è sotto il livello di riordino.`

L'agente imposta il foglio di inventario e segna gli articoli che devono essere riordinati. Aggiorna le quantità e chiedigli di ricontrollare in qualsiasi momento.

*Suggerimento: un controllo settimanale programmato può dirti cosa riordinare prima che finisca.*

---

### Pianifica una rotta di consegna

![Una rotta di consegna mappata tra le soste](../../assets/examples/delivery-route.png)
*Una rotta di consegna mappata tra le soste*

**Cosa chiedi:** `Pianifica la rotta migliore per questi cinque indirizzi di consegna e mostrala su una mappa.`

L'agente piazza le soste su una mappa in un ordine efficiente e ti dà la distanza e il tempo stimato. Tu segui la rotta e risparmi carburante.

*Suggerimento: aggiungi finestre temporali ('sosta B prima di mezzogiorno') e l'agente le tiene conto.*

---

### È disponibile?

![Un controllo di scorta live risposto in pochi secondi](../../assets/examples/stock-check.png)
*Un controllo di scorta live risposto in pochi secondi*

**Cosa chiedi:** `Abbiamo l'articolo SKU 3391 disponibile, e quanti?`

L'agente controlla la scorta nel tuo sistema e risponde con la quantità, così puoi promettere o non promettere con sicurezza.

*Suggerimento: abbinalo a un avviso di scorta bassa programmato quotidianamente per evitare sorprese.*

<!-- END agentbridge-examples -->
