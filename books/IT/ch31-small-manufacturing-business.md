# Capitolo 31 — Una piccola azienda manifatturiera

*Questo capitolo è un composito rappresentativo. Non è una singola azienda reale. Combina i modelli comuni che vediamo nelle piccole officine meccaniche e nei fabbri che adottano l'IA. Tutti i numeri sono illustrativi — mostrano la forma della decisione, non una promessa. Sostituiscili con i tuoi.*

## Contesto

Immagina una piccola officina di meccanica di precisione. La chiameremo **Northgate Machining**. Impiega circa venticinque persone. Produce pezzi metallici su misura a ordine — pezzi unici e serie brevi per altre fabbriche. Nulla sta su uno scaffale ad aspettare un compratore. Ogni pezzo inizia come una richiesta del cliente.

Il lavoro comincia con un **RFQ**, che sta per "richiesta di preventivo". Un cliente invia un disegno via email — di solito un PDF con la forma del pezzo, le sue misure, e il materiale da cui deve essere fatto. L'officina deve guardare quel disegno, capire quanto durerà ogni passo di taglio e finitura, sommare il costo del metallo e del tempo macchina, e restituire un prezzo. Quel prezzo è il preventivo. Se è troppo alto, il cliente va altrove. Se è troppo basso, l'officina vince il lavoro ma perde denaro a realizzarlo.

Due preventivatori esperti fanno la maggior parte di questo lavoro di preventivazione. Lo fanno da anni. Sanno guardare un disegno e sapere più o meno quanto costa. Ma "più o meno" fa molto lavoro in quella frase. L'officina non ha alcuna registrazione scritta di quanto i preventivi passati siano costati davvero da produrre. La conoscenza vive in due teste. Quando quelle due persone sono in vacanza, la preventivazione rallenta fino a fermarsi.

Dietro la preventivazione siede il resto dell'officina. Il metallo grezzo — barre, piastre, tondi — è tracciato in un foglio di calcolo aggiornato quando qualcuno se ne ricorda. Il controllo qualità è un controllo visivo finale a mano alla fine del lavoro. I report settimanali per la titolare sono digitati a mano da tre diversi fogli di calcolo. Nulla è collegato. Tutto dipende dalle persone che si ricordano di scrivere le cose.

Questo è un piccolo manifatturiere normale e sano. È in utile. È occupato. E sta lasciando denaro sul tavolo in quattro posti: preventivazione, inventario, qualità e reportistica.

## Il problema

La titolare, Elena, sente i problemi ma non sempre li vede. Nominiamoli apertamente.

**La preventivazione è lenta e incoerente.** Un pezzo semplice richiede un'ora per essere preventivato. Uno complesso mezza giornata. La media è di due giorni dall'arrivo dell'email all'uscita del preventivo. In quella finestra, il cliente ha già chiesto ad altre due officine. La velocità conta. Peggio, i due preventivatori prezzano lo stesso disegno in modo diverso. Uno è cauto e prezza alto. L'altro è aggressivo e prezza basso. Nell'arco di un anno, alcuni lavori sono silenziosamente sottoprezzati. L'officina li vince, li costruisce, e scopre dopo che il tempo macchina è costato più di quanto il prezzo coprisse. Queste perdite sono invisibili perché nessuno confronta il preventivo con il costo effettivo dopo.

**L'inventario è a intuito.** L'officina compra metallo grezzo quando qualcuno nota che lo scaffale è basso. Troppo spesso, è troppo tardi — un lavoro è ritardato perché la barra giusta non è disponibile. Proprio spesso, l'officina compra troppo, e materiale costoso giace per mesi, immobilizzando liquidità. Il foglio di calcolo non è mai del tutto giusto. Nessuno si fida, così le persone ricontrollano camminando fino allo scaffale, il che spreca tempo.

**I difetti di qualità sono colti troppo tardi.** Un pezzo cattivo è spesso trovato solo al controllo finale, dopo che tutto il lavoro è finito. Se l'errore è stato fatto al primo taglio, l'officina può aver fatto cinquanta pezzi cattivi prima di accorgersene. Quello è scarto — materiale e tempo macchina gettati via. Coglierlo dopo cinquanta pezzi invece che dopo uno è cinquanta volte la perdita.

**La reportistica divora ore.** Ogni venerdì, qualcuno spende tre o quattro ore a tirare numeri dai fogli di calcolo per costruire un riassunto per Elena. Quel tempo è puro costo generale — non produce pezzi né vince clienti.

Ognuno di questi è una piccola perdita. Insieme, prosciugano denaro reale e tempo reale. Se vuoi vedere come queste quattro attività si classificano rispetto al resto della tua azienda, il metodo impatto-sforzo nel [Capitolo 12 — Dove l'IA può aiutare il tuo business](ch12-where-ai-can-help-your-business.md) è il posto per valutarle.

## La soluzione

Elena non prova a "usare l'IA ovunque". Scegle le quattro perdite e le attacca una alla volta, iniziando dalla più grande e più facile.

**Preventivazione più intelligente.** Invece di leggere ogni disegno da zero, l'officina immette i suoi lavori passati in un sistema. Per ogni lavoro passato, ora registra due cose che prima non collegava: il preventivo originale e il costo effettivo di produzione. Nel tempo questo diventa una biblioteca di riferimento. Quando arriva un nuovo disegno, un assistente IA legge il PDF, estrae le caratteristiche chiave — le dimensioni, le tolleranze (quanto esatta deve essere ogni misura), il materiale, il numero di pezzi — e suggerisce un prezzo basato su lavori passati simili. Il preventivatore non parte più da una pagina bianca. Parte da una bozza e la aggiusta. L'IA fa il primo passaggio; l'umano prende la decisione.

**Inventario che prevede.** L'officina collega il suo foglio di calcolo delle scorte a un semplice strumento di previsione. Lo strumento guarda quanto velocemente ogni materiale è usato e suggerisce quando riordinare e quanto. Non piazza l'ordine da sé. Solleva un suggerimento: "Rimarrai senza questa barra di alluminio in nove giorni; ordina ora." Una persona lo conferma. L'intuito diventa un prompt.

**Controlli qualità alla macchina.** Invece di controllare solo alla fine, l'officina mette una piccola camera a una macchina. Un sistema di computer vision — IA che legge ciò che una camera vede — guarda ogni pezzo mentre esce e segnala ciò che sembra sbagliato: una crepa, una dimensione sbagliata, un foro mancante. L'operatore vede il segnale immediatamente e si ferma prima di fare cinquanta copie cattive. Il controllo umano finale resta; la camera sposta solo l'avviso prima. (Il trattamento più approfondito del controllo qualità basato su visione e della manutenzione predittiva è nel [Capitolo 29 — Operazioni e produzione](ch29-operations-and-production.md).)

**Report che si scrivono da soli.** I fogli di calcolo sono collegati a un assistente di reportistica. Il venerdì, invece di digitare, Elena riceve un riassunto preparato: lavori preventivati, lavori vinti, tasso di scarto, livelli di scorta, liquidità immobilizzata. Lo legge e lo modifica. Tre ore diventano quindici minuti.

Nota il modello in tutti e quattro. L'IA non agisce mai da sola. Legge, suggerisce, segnala e prepara bozze. Un umano decide, conferma e approva. È lo stesso modello "l'umano revisiona la bozza della macchina" che il caso Elanco mostra nel [Capitolo 25 — Amministrazione e finanza](ch25-administration-and-finance.md). In un'officina dove un numero sbagliato può far perdere denaro vero, quella regola non è opzionale.

## Gli strumenti

Niente di tutto questo richiedeva un team di ingegneri. Gli strumenti sono pronti all'uso, rivolti alle piccole imprese.

- **Un assistente di lettura documenti** che apre il PDF del disegno ed estrae dimensioni e caratteristiche in un modulo strutturato. È la stessa classe di strumento che legge le fatture nel [Capitolo 25](ch25-administration-and-finance.md).
- **Un assistente di preventivazione** costruito sopra di esso, che confronta le caratteristiche estratte con i lavori passati e propone un prezzo. Può essere uno strumento low-code applicato al foglio di calcolo di preventivazione esistente dell'officina, collegato come descritto nel [Capitolo 19 — Collegare l'IA a sistemi che già usi](ch19-connecting-ai-to-systems-you-already-use.md).
- **Un componente aggiuntivo di previsione** per il foglio di calcolo dell'inventario o il sistema ERP (enterprise resource planning) di base dell'officina. Molti strumenti di inventario ora includono una funzione "suggerisci un riordino".
- **Una camera più uno strumento di ispezione a computer vision** a una macchina. Sono venduti come unità piccole e autosufficienti per i controlli di qualità.
- **Un assistente di reportistica** che legge i fogli di calcolo collegati e prepara il riassunto settimanale in linguaggio semplice.

Come scegliere tra questi senza essere ingannati da demo patinate è trattato nel [Capitolo 17 — Scegliere gli strumenti senza farsi ingannare](ch17-choosing-tools-without-being-fooled.md). Una cautela specifica a un'officina meccanica: **i disegni sono riservati.** Il disegno del pezzo di un cliente è la loro proprietà intellettuale. Prima di immettere disegni in qualsiasi strumento cloud, controlla dove vanno i dati e chi può vederli. Per alcune officine, tenere l'IA sui propri computer — self-hosting, spiegato nel [Capitolo 8 — Self-Hosting: tieni i tuoi dati sotto controllo](ch08-self-hosting-keep-your-data-under-control.md) — è la scelta più sicura. I rischi di inviare file sensibili a servizi di terze parti sono nel [Capitolo 9 — Servizi di terze parti e shadow AI](ch09-third-party-services-and-shadow-ai.md).

## I costi

Ecco un budget illustrativo del primo anno per un'officina come Northgate. Sono numeri inventati per mostrare la forma. Usa i tuoi.

**Costi diretti.**
- Assistente preventivazione e documenti: circa 9.000 € l'anno in abbonamenti.
- Componente aggiuntivo di previsione: circa 3.000 € l'anno.
- Unità camera e ispezione a visione: circa 6.000 € una tantum, più 1.200 € l'anno.
- Assistente di reportistica: circa 2.400 € l'anno.
- Configurazione e integrazione (aiuto esterno per collegare gli strumenti ai fogli di calcolo e alla macchina): circa 10.000 € una tantum.
- Formazione dei preventivatori e degli operatori: circa 3.000 € una tantum.

Totale primo anno: circa **34.600 €**. Negli anni stabili dopo, i costi una tantum spariscono e gli abbonamenti ricorrenti arrivano a circa **15.600 €**.

**Costi indiretti.** Sono quelli che le persone dimenticano.
- I preventivatori spendono ore a imparare lo strumento e controllare le sue bozze. È tempo reale, valutato al loro costo orario caricato.
- Il calo di apprendimento: per le prime settimane, la preventivazione è più lenta, non più veloce, mentre le persone si fidano del nuovo sistema.
- La camera di visione ha bisogno di ricalibrature occasionali quando cambia la luce o il pezzo.
- Qualcuno deve rivedere i preventivi suggeriti dall'IA e i punti di riordino ogni giorno. Non saltare mai questo.

Il metodo completo per contare questi costi onestamente, e per trasformare i risparmi in una cifra di ritorno, vive nel [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md). Non fare i conti a mente. Scrivili.

## I risultati

Dopo un anno, misurato contro la linea di base che Elena ha registrato prima di iniziare, l'esito illustrativo appare così. Ricorda: i tuoi numeri differiranno. Questi mostrano a cosa può somigliare un buon adattamento, non cosa sarà il tuo.

- **Il tempo di preventivazione** è sceso da una media di due giorni a poche ore per la maggior parte dei pezzi. Il preventivatore revisiona una bozza invece di costruire da zero.
- **Meno lavori sottoprezzati.** Perché il preventivo è ancorato a ciò che lavori simili sono costati davvero, il divario tra prezzo preventivato e costo reale si è ridotto. L'officina ha smesso di perdere silenziosamente denaro sui lavori vinti.
- **Il tasso di vittoria è migliorato.** Preventivi più veloci hanno significato che Northgate rispondeva a più RFQ dentro la finestra in cui il cliente sta ancora scegliendo.
- **Lo scarto è calato.** Coglierlo alla macchina invece che alla fine ha tagliato materiale e tempo macchina sprecati. Invece di cinquanta pezzi cattivi, l'operatore l'ha colto al primo o secondo.
- **La rotazione delle scorte è migliorata.** Meno rotture di stock hanno significato meno lavori ritardati. Meno sovra-acquisti hanno significato meno liquidità congelata sullo scaffale.
- **I report** sono passati da tre o quattro ore di digitazione a circa quindici minuti di lettura e modifica.

L'avvertimento onesto: niente di tutto questo è accaduto il primo giorno. L'assistente di preventivazione era grezzo per il primo mese perché la biblioteca dei lavori passati era scarsa. La camera di visione dava falsi allarmi finché non fu calibrata. I risparmi sono saliti nel corso di settimane, esattamente come l'avviso della curva di apprendimento nel [Capitolo 16](ch16-goals-costs-and-return-on-investment.md) prevede. Elena misurò i numeri reali dopo la salita, non durante.

## Lezioni apprese

**Inizia dalla preventivazione.** Delle quattro perdite, la preventivazione era il massimo impatto e il minimo rischio da provare. Un preventivo sbagliato è colto dal preventivatore prima che esca. Questo la rese il progetto primo perfetto — la stessa regola "prima alto impatto, alta facilità" dal [Capitolo 12](ch12-where-ai-can-help-your-business.md).

**I tuoi lavori passati sono il carburante.** L'assistente di preventivazione era buono solo quanto il record dei preventivi passati e dei loro costi reali. La cosa di maggior valore singolo che Elena fece fu iniziare a collegare ogni preventivo al suo costo di produzione effettivo. Senza quei dati, l'IA non aveva nulla da cui imparare. La prontezza dei dati è trattata nel [Capitolo 14 — Dati: la materia prima](ch14-data-the-raw-material.md).

**L'IA prepara bozze; l'umano decide.** Nemmeno un preventivo uscì senza che una persona lo approvasse. Nemmeno un riordino fu piazzato senza che una persona lo confermasse. In un'officina dove un numero sbagliato è denaro vero, il controllo umano è la sicurezza, non un ritardo.

**I disegni sono riservati.** Tratta ogni disegno del cliente come proprietà intellettuale sensibile. Decidi dove può andare prima di immetterlo da qualche parte. Per alcune officine questo significa self-hosting; per altre significa un fornitore vagliato con un contratto chiaro.

**Calibra la camera; non fidarti ciecamente.** Il sistema di visione non era plug-and-play. Aveva bisogno di messa a punto per distinguere un vero difetto da un'ombra. Mettilo a budget, e tieni il controllo umano finale in atto.

**Aspettati la salita.** Il primo mese fu più lento e disordinato del dodicesimo. Giudica il progetto dopo la curva di apprendimento, non durante.

**Collega, non sostituire.** Northgate non gettò via i suoi fogli di calcolo né il suo ERP. Applicò l'IA su ciò che già funzionava, come descritto nel [Capitolo 19](ch19-connecting-ai-to-systems-you-already-use.md). L'officina tenne i suoi sistemi e aggiunse uno strato più intelligente sopra.

La lezione del piccolo manifatturiere è la stessa di ogni altro settore: trova la perdita, scegli la più facile ad alto valore, lascia che l'IA prepari bozze e segnali, tieni un umano sulla decisione, e misura onestamente. Un'officina con venticinque persone e nessun ingegnere può farlo. Gli strumenti sono pronti. L'unica cosa che manca è uno sguardo chiaro su dove il denaro sta perdendo.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come appare lo stesso lavoro con AgentBridge. Ogni riquadro mostra il risultato finito e la singola riga che digiti per ottenerlo.

### Progetta un pezzo semplice

![Un pezzo semplice modellato con lo strumento CAD](../../assets/examples/part-design.png)
*Un pezzo semplice modellato con lo strumento CAD*

**Cosa chiedi:** `Progetta una piccola staffa metallica di 80 per 40 millimetri con quattro fori di montaggio.`

L'agente pilota lo strumento CAD per modellare il pezzo con le dimensioni giuste, e ottieni un file che puoi rivedere o esportare.

*Suggerimento: descrivi la forma e le misure; l'agente gestisce i passi CAD.*

---

### Controlla come combaciano i pezzi

![Un controllo di insieme tra due pezzi](../../assets/examples/assembly-check.png)
*Un controllo di insieme tra due pezzi*

**Cosa chiedi:** `Metti insieme questi due pezzi e controlla se ci sono sovrapposizioni o problemi di gioco.`

L'agente assembla i pezzi nel modello CAD e segnala dove cozzano o dove l'accoppiamento è troppo stretto.

*Suggerimento: cogli i problemi di accoppiamento sullo schermo, non sul banco dell'officina.*

---

### Un disegno per l'officina

![Un disegno tecnico quotato per la produzione](../../assets/examples/technical-drawing.png)
*Un disegno tecnico quotato per la produzione*

**Cosa chiedi:** `Produce un disegno tecnico della staffa con le dimensioni principali segnate.`

L'agente genera un disegno con le dimensioni segnate, pronto per la persona che farà il pezzo.

*Suggerimento: chiedi la vista che ti serve — dall'alto, laterale — così il disegno è chiaro.*

<!-- END agentbridge-examples -->
