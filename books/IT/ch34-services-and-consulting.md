# Capitolo 34 — Servizi e consulenza

*Questo capitolo è un composite rappresentativo. Non è una singola azienda reale. Unisce gli schemi ricorrenti che osserviamo nelle società di consulenza e nei servizi professionali che adottano l'IA. Tutti i numeri sono illustrativi: mostrano la forma della decisione, non una promessa. Sostituiscili con i tuoi.*

## Il contesto

Immagina una società di consulenza di medie dimensioni. La chiameremo **Northbeam Advisory**. Ha circa venticinque consulenti e un piccolo team di supporto. Non vende un prodotto: vende competenza e tempo. Un cliente — di solito un'altra azienda — ha un problema, e Northbeam manda persone a risolverlo: un progetto di strategia qui, una revisione operativa là, uno studio sui dati da un'altra parte.

Ogni progetto segue più o meno lo stesso percorso. Per primo arriva il **pitch**: una proposta che dice cosa l'azienda ha capito, cosa farà e quanto costerà. Se il cliente accetta, il team fa il lavoro. Durante il lavoro, il cliente riceve regolari **rapporti di stato**. Alla fine ci sono un elaborato finale e una fattura. In mezzo a tutto questo c'una montagna di coordinamento: trovare le persone giuste per il lavoro, fissare riunioni, mettere per iscritto quanto detto e tenere traccia di chi è libero e quando.

Per anni tutto questo è andato avanti grazie alle persone. Un partner scrive una proposta aprendone una vecchia e riscrivendola. Un consulente risolve un problema che l'azienda aveva già risolto tre anni prima, ma nessuno ricorda dove, quindi lo risolve da zero. Un project manager costruisce ogni rapporto di stato a mano, copiando numeri da un file in una slide. Qualcuno passa mezza giornata a incrociare i calendari dei consulenti con le esigenze dei progetti. L'azienda ha successo. Ma spende molto tempo costoso e formato su lavoro ripetitivo, e continua a perdere conoscenza per cui ha già pagato una volta.

Una società di consulenza assomiglia a uno studio professionale sotto un aspetto importante. Tutto ciò che tocca è **riservato**. La strategia di un cliente, un modello di costi, un piano di fusione: tutto questo viene condiviso sulla fiducia. Questo singolo fatto determina come si può usare l'IA qui, esattamente come per uno studio legale. È il filo che attraversa tutto il capitolo.

## Il problema

Le perdite dell'azienda sono facili da nominare.

**Le proposte sono lente.** Ogni nuovo pitch parte da un foglio quasi bianco. L'azienda ha scritto centinaia di proposte e ha buon materiale dentro, ma trovare l'esempio passato giusto, il caso studio giusto, la struttura di prezzo giusta richiede tempo. Un partner può passare due giorni interi su una proposta che è per lo più un riassemblaggio. Proposte lente significano anche occasioni perse: alcuni affari sfuggono solo perché la risposta è arrivata troppo tardi.

**La conoscenza se ne va via.** Quando un consulente se ne va, se ne va anche il know-how che ha in testa. Un metodo che ha affinato, un vezzo di un cliente che ha imparato, una soluzione che ha messo a punto: se nessuno l'ha scritto, è perso. Così l'azienda paga per risolvere gli stessi problemi ancora e ancora. Questa è la perdita più costosa, perché è invisibile.

**Il reporting è manuale.** Un rapporto di stato è più o meno lo stesso ogni settimana: cosa si è mosso, cosa è in ritardo, cosa viene dopo. Ma una persona lo assembla a mano ogni volta, tirando fuori numeri dai file di progetto e scrivendo sempre lo stesso tipo di narrazione. È affidabile ed è noioso, e si mangia ore che potrebbero essere fatturabili.

**Overhead di coordinamento.** Incrociare le competenze del consulente giusto con un progetto, controllare chi è libero, fissare riunioni e scrivere gli appunti dopo è una tassa costante. Le riunioni avvengono, ma nessuno vuole scrivere il verbale, così le decisioni restano vaghe e qualcuno deve rifare la conversazione più tardi.

Se vuoi vedere come queste si classificano rispetto al resto della tua azienda, il metodo impatto-sforzo del [Capitolo 12 — Dove l'IA può aiutare la tua azienda](ch12-where-ai-can-help-your-business.md) è il posto giusto per dargli un punteggio.

Sopra tutti e quattro siede la riservatezza. Qualsiasi strumento che legga la proposta o il file di progetto di un cliente deve essere uno strumento di cui l'azienda può fidarsi, che non lo faccia trapelare. Questa domanda viene prima di tutto.

## La soluzione

Northbeam attacca le quattro perdite in ordine di sicurezza, non solo di dimensione. La regola è la stessa che usa uno studio legale: iniziare dove un errore costa poco e i dati non sono i più sensibili, e muoversi verso il lavoro sensibile solo quando gli strumenti sono affidabili.

**Un assistente per le proposte che stende dalla storia dell'azienda.** Quando arriva un nuovo pitch, un consulente scrive un breve brief: il cliente, il problema, il perimeto di massima. Un assistente IA cerca nelle proposte passate dell'azienda e tira fuori le sezioni più rilevanti, poi stende una prima versione: una comprensione del problema, un approccio suggerito, un caso studio che calza. Il partner non parte più a freddo. Modifica una bozza invece di costruire dal nulla. Due giorni diventano poche ore. È lo stesso schema "la macchina stende, l'umano revisiona" che il caso Elanco mostra nel [Capitolo 25 — Amministrazione e finanza](ch25-administration-and-finance.md).

**Una memoria ricercabile per l'azienda.** L'azienda mette i suoi elaborati passati, i metodi e gli appunti in una ricerca interna che i consulenti possono interrogare in linguaggio naturale. Spesso si chiama **base di conoscenza con ricerca IA**. Sotto il cofano usa una tecnica chiamata **retrieval-augmented generation**, o RAG. In parole povere: invece di fare una domanda a un'IA generica, il sistema prima consulta i documenti dell'azienda, poi risponde usando solo ciò che ha trovato lì. Così quando un consulente chiede: "Come abbiamo gestito una revisione del rischio fornitore per un cliente retail?", il sistema trova il vero progetto passato e risponde da quello. La conoscenza smette di andarsene via. La tecnologia di chatbot e ricerca dietro questo è trattata nel [Capitolo 27 — Assistenza e supporto clienti](ch27-customer-care-and-support.md).

**Un reporting che si stende da sé.** Lo strumento di reporting si collega ai dati del progetto — attività, date, traguardi — e stende il rapporto settimanale: cosa si è mosso, cosa è scivolato, cosa viene dopo. Il project manager lo revisiona, aggiunge il giudizio umano sul tono e su cosa sottolineare, e lo invia. Il foglio bianco è sparito.

**Pianificazione e riassunti delle riunioni.** Un assistente di pianificazione incrocia le competenze e la disponibilità dei consulenti con le esigenze dei progetti e propone chi dovrebbe lavorare su cosa. Per le riunioni, uno strumento registra la chiamata, stende il verbale ed elenca decisioni e azioni da fare. Una persona lo controlla prima che circoli. Le decisioni smettono di essere vaghe perché la messa per iscritto avviene automaticamente.

In ogni caso, l'umano resta al comando. Nella consulenza, il cliente paga per il giudizio e la responsabilità. L'IA stende, cerca e riassume. Il consulente decide, personalizza e si assume la responsabilità del lavoro.

## Gli strumenti

Gli strumenti sono ordinari, ma il modo in cui vengono impiegati è plasmato dalla riservatezza.

- **Un assistente per le proposte** che cerca nelle proposte passate dell'azienda e ne stende una nuova da un brief.
- **Una ricerca interna della conoscenza** (RAG) sugli elaborati e gli appunti dell'azienda, così i consulenti possono fare domande in linguaggio naturale e ottenere risposte fondate sul lavoro stesso dell'azienda.
- **Un assistente di reporting** che si collega ai dati di progetto e stende rapporti di stato.
- **Un assistente di pianificazione** per abbinare le persone ai progetti, più **uno strumento di riassunto delle riunioni** che trasforma una chiamata registrata in una bozza di verbale.

Come scegliere questi strumenti senza farsi abbagliare da una demo è trattato nel [Capitolo 17 — Scegliere gli strumenti senza farsi ingannare](ch17-choosing-tools-without-being-fooled.md). Come collegarli ai sistemi di gestione progetti e documenti già in uso dall'azienda è nel [Capitolo 19 — Collegare l'IA ai sistemi che usi già](ch19-connecting-ai-to-systems-you-already-use.md).

**La riservatezza viene prima di tutto.** Un chatbot generico in cui incolli la proposta di un cliente potrebbe conservarla, addestrarsi su di essa o esporla. Per una società di consulenza, questo può rompere la fiducia di un cliente e un obbligo contrattuale di segretezza. L'azienda deve usare strumenti che mantengano privati i dati dei clienti: o un servizio di livello business con un contratto chiaro di nessun-addestramento e nessuna-condivisione, o un modello eseguito sulle macchine stesse dell'azienda. L'auto-ospitaggio è spiegato nel [Capitolo 8 — Self-hosting: tieni i tuoi dati sotto controllo](ch08-self-hosting-keep-your-data-under-control.md). Il pericolo che il personale incolli di nascosto dati dei clienti in strumenti pubblici — la shadow AI — è l'oggetto del [Capitolo 9 — Servizi di terze parti e shadow AI](ch09-third-party-services-and-shadow-ai.md). E poiché i file dei clienti e le liste di contatti contengono dati personali, le regole sulla privacy del [Capitolo 10 — Privacy e GDPR](ch10-privacy-and-gdpr.md) si applicano pienamente.

## I costi

Ecco un budget illustrativo del primo anno per un'azienda come Northbeam. Sono numeri inventati per mostrare la forma. Usa i tuoi.

**Costi diretti.**
- Assistente per le proposte (di livello business, con contratto di riservatezza): circa 12.000 € l'anno.
- Ricerca interna della conoscenza (piattaforma RAG): circa 9.000 € l'anno.
- Assistente di reporting: circa 4.800 € l'anno.
- Strumenti di pianificazione e riassunto riunioni: circa 6.000 € l'anno.
- Configurazione e integrazione con i sistemi di gestione progetti e documenti: circa 12.000 € una tantum.
- Formazione dei consulenti e del personale di supporto: circa 5.000 € una tantum.

Totale primo anno: circa **48.800 €**. Negli anni a regime, gli abbonamenti ricorrenti arrivano a circa **31.800 €**.

**Costi indiretti.**
- I consulenti spendono tempo a rivedere ogni bozza dell'IA. È il costo della rete di sicurezza, e deve restare.
- Il calo di produttività mentre tutti si adattano.
- Il costo di curare la base di conoscenza. Una ricerca vale quanto ciò che ci metti dentro, e qualcuno deve tenerla pulita e aggiornata.
- Il tempo speso a verificare ogni strumento per riservatezza e conformità prima dell'uso.
- Il costo di un errore se una bozza viene creduta senza controllo: nella consulenza, un numero sbagliato in un rapporto al cliente può costare molto più di un abbonamento.

Il metodo completo per contare questi costi e trasformare i risparmi in una cifra di ritorno è nel [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md). Non fare i conti a mente. Scrivili.

## I risultati

Dopo un anno, misurato rispetto a una baseline che l'azienda ha registrato prima di iniziare, il risultato illustrativo appare così. I tuoi numeri saranno diversi. Questi mostrano come può essere un buon adattamento.

- **Le proposte sono diventate più veloci.** Un pitch che richiedeva due giorni ora richiede poche ore, perché il partner modifica una bozza invece di costruire da un foglio bianco. L'azienda risponde anche prima, e questo vince alcuni affari che avrebbe perso.
- **La conoscenza è rimasta.** Quando i consulenti se ne sono andati, il loro know-how è rimasto nella base ricercabile. L'azienda ha risolto meno problemi due volte.
- **Il tempo di reporting è calato.** Il rapporto di stato settimanale è diventato una revisione di una bozza, non una costruzione manuale, liberando ore tra i project manager.
- **Le riunioni hanno prodotto verbali.** Decisioni e azioni da fare venivano messe per iscritto automaticamente, così meno conversazioni dovevano essere ripetute.
- **Più tempo fatturabile.** Con meno tempo speso in riassemblaggio e ricerca, i consulenti hanno dedicato più della loro giornata a lavoro per cui il cliente paga.

L'avvertimento onesto: nulla di tutto questo è stato istantaneo. L'assistente per le proposte produceva bozze rozze all'inizio, finché non ha avuto abbastanza buone proposte passate da cui imparare lo stile dell'azienda. La ricerca della conoscenza dava risposte deboli finché i documenti non sono stati organizzati e etichettati. Lo strumento di riassunto riunioni etichettava male gli interlocutori all'inizio. I guadagni sono cresciuti nel giro di settimane, come prevede l'avvertimento sulla curva di apprendimento del [Capitolo 16](ch16-goals-costs-and-return-on-investment.md). L'azienda ha misurato i numeri reali dopo la salita, non durante.

## Lezioni apprese

**La riservatezza è il primo vincolo, non un ripensamento.** Nella consulenza la domanda non è mai solo "questo strumento funziona?". È "questo strumento si può fidare con il file privato di un cliente?". Rispondi a questo prima di ogni altra cosa. Usa strumenti di livello business con un contratto chiaro di nessun-addestramento, oppure auto-ospita. Vedi il [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md) e il [Capitolo 9](ch09-third-party-services-and-shadow-ai.md).

**L'IA stende; il consulente consiglia.** Il valore di un consulente è il giudizio e la responsabilità. L'IA fa una cernita, stende e riassume; il consulente decide e firma. Non lasciare mai che una bozza diventi lavoro per il cliente senza una mente umana sopra.

**Una base di conoscenza è un giardino, non una discarica.** La ricerca IA vale quanto i documenti che ci sono dietro. Se ci butti dentro file disordinati, obsoleti o sbagliati, ottieni risposte sicure ma errate. Qualcuno deve possedere la base, tenerla aggiornata e controllare chi vede cosa. Il controllo degli accessi conta: un consulente sul progetto di un cliente non dovrebbe poter cercare il materiale riservato di un altro cliente. Il principio di prontezza dei dati è nel [Capitolo 14 — Dati: la materia prima](ch14-data-the-raw-material.md).

**Registrare le riunioni richiede consenso.** Uno strumento di riassunto riunioni funziona registrando la chiamata. Registrare una conversazione è trattamento di dati personali, e le persone devono saperlo e accettare. Avvisa i partecipanti prima di registrare, e segui le regole del [Capitolo 10 — Privacy e GDPR](ch10-privacy-and-gdpr.md). Non registrare di nascosto.

**Attenzione alla risposta sicura ma sbagliata.** Questi strumenti possono produrre testo che suona giusto ma è errato: un caso studio mai avvenuto, un numero che torna. Nella consulenza, un dato inventato in un rapporto al cliente è un disastro. Verifica ogni numero e ogni affermazione contro la fonte reale. Il problema dell'affidabilità è trattato nel [Capitolo 2 — L'IA spiegata semplice](ch02-ai-explained-simply.md), e il dovere di essere onesti su ciò che l'IA può e non può fare è nel [Capitolo 4 — IA etica: fare la cosa giusta](ch04-ethical-ai-doing-the-right-thing.md).

**Inizia dal lavoro sicuro.** Northbeam è partita con la ricerca interna e le bozze di reporting: basso rischio, non ancora le proposte ai clienti più sensibili. Si è mossa verso la stesura delle proposte solo quando gli strumenti sono diventati affidabili. È la regola "prima ciò che è più facile" del [Capitolo 12](ch12-where-ai-can-help-your-business.md).

**Misura onestamente e metti in conto la salita.** Registra la baseline prima di iniziare. Giudica il progetto dopo la curva di apprendimento, non durante. Il metodo è nel [Capitolo 22 — Misurare risultati e ROI](ch22-measuring-results-and-roi.md).

La lezione della società di consulenza è la stessa di ogni altro settore, con una ringhiera in più: trova il lavoro ripetitivo — proposte, ricerca, reporting, coordinamento — lascia che l'IA stenda e recuperi, tieni un umano sul giudizio e sulla relazione con il cliente, e misura onestamente. E in un'azienda costruita sulla fiducia, non lasciare mai che lo strumento tocchi il file riservato di un cliente finché non sei certo che sia sicuro farlo.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come appare lo stesso lavoro con AgentBridge. Ogni riquadro mostra il risultato finito e l'unica riga che digiti per ottenerlo.

### Disegna la tua area di servizio

![Una mappa dell'area di servizio per i clienti](../../assets/examples/service-area.png)
*Una mappa dell'area di servizio per i clienti*

**Cosa chiedi:** `Mostra la nostra area di servizio su una mappa con le principali città che copriamo.`

L'agente produce una mappa chiara della tua copertura che puoi mettere sul tuo sito web o inviare ai clienti.

*Suggerimento: tienila aggiornata mentre cresci: chiedi semplicemente una nuova versione.*

<!-- END agentbridge-examples -->
