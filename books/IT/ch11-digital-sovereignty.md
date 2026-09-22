# Capitolo 11 — Sovranità digitale: il diritto di controllare la tua IA

## In parole semplici

Sovranità, nel suo senso più antico, significa il diritto di governarsi da soli senza che qualcun altro ti dica cosa fare. La sovranità digitale prende quell'idea e la applica alla tua vita digitale: il diritto di controllare i tuoi dati, il tuo software e le macchine che li eseguono.

Applicata all'IA, la sovranità digitale risponde a tre domande semplici su ogni strumento IA che usi.

- **Dove sono i miei dati?** Quale paese, i server di quale azienda, sotto quale legge?
- **Chi può accedervi?** Il personale del fornitore, subappaltatori, o un governo straniero?
- **Come vengono elaborati?** Su un modello che non posso vedere, o su un sistema che posso ispezionare e cambiare?

Se non riesci a rispondere a quelle tre domande, non hai sovranità su quella parte del tuo business. Hai preso in prestito quella di qualcun altro, e puoi perderla ogni volta che lui cambia idea.

Questo non è la stessa cosa che self-hosting, anche se si sovrappongono. Il self-hosting, trattato nel [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md), è un modo per acquisire controllo. La sovranità digitale è l'obiettivo più ampio: controllo su da dove derivano le tue capacità digitali e chi tiene il guinzaglio. Puoi perseguirla con i tuoi server, con software aperto, con contratti, o con un misto.

Un'analogia utile è il cibo. Puoi comprare piatti pronti da una fabbrica che non vedi mai, e la maggior parte dei giorni va bene. Ma se hai un'allergia, o semplicemente vuoi sapere cosa c'è nel tuo cibo, inizi a interessarti alla ricetta e alla cucina. La sovranità digitale è interessarsi alla ricetta e alla cucina della tua IA — non per paura, ma perché in gioco ci sono i tuoi dati, i tuoi clienti e il tuo futuro.

Il modello opposto, i servizi di terze parti non gestiti e la shadow AI, è nel [Capitolo 9](ch09-third-party-services-and-shadow-ai.md). I doveri legali sui dati personali sono nel [Capitolo 10](ch10-privacy-and-gdpr.md). Questo capitolo riguarda la scelta strategica: quanto della tua IA vuoi davvero controllare.

## Un po' di storia

**Anni 2000-2010: la comodità cancella la domanda.** Mentre le aziende si spostavano sul cloud, quasi nessuno chiedeva dove andassero i dati. Gli strumenti erano buoni ed economici. Il controllo non era un criterio d'acquisto.

**2013: Snowden cambia il clima.** Le rivelazioni sulla sorveglianza di massa fecero capire a governi e aziende che i dati archiviati in un altro paese potevano essere raggiunti dalle autorità di quel paese. La domanda "dove sono i miei dati" divenne una domanda di sicurezza, non solo di privacy.

**2018: il GDPR rende la località rilevante legalmente.** La legge europea sulla privacy diede alle persone diritti sui loro dati e rese le aziende responsabili di dove fossero e come fossero trattati. La residenza dei dati — tenere i dati dentro una regione — divenne un requisito reale, non uno slogan.

**2019-2022: appare il "cloud sovrano".** I fornitori cloud iniziarono a offrire opzioni sovrane: dati tenuti in un paese specifico, gestiti sotto la legge locale, a volte con partner locali. La sovranità divenne una caratteristica di prodotto.

**2022-2023: i modelli a pesi aperti aprono un nuovo percorso.** Quando potenti modelli IA divennero scaricabili ed eseguibili da chiunque, un'azienda poteva, per la prima volta, eseguire un modello capace interamente secondo le proprie condizioni. La sovranità non era più solo una promessa di un fornitore cloud; divenne qualcosa che potevi costruire.

**2024-2025: la sovranità diventa strategia nazionale e aziendale.** Paesi e blocchi iniziarono a trattare la capacità IA come strategica. L'Europa lanciò progetti finanziati per costruire propri modelli aperti, affinché l'IA europea non dipendesse interamente da fornitori stranieri. La sezione Curiosità ne tratta uno.

L'arco è chiaro. La comodità ci aveva fatto smettere di chiedere chi controlla i nostri strumenti. Una serie di shock ci ha fatto chiedere di nuovo. Ora il controllo è una scelta di progettazione che puoi fare deliberatamente.

## Curiosità

### 11.6 Costruire il proprio assistente, e un continente che fa lo stesso

**Un modello rappresentativo (illustrativo).** Considera una studio professionale di medie dimensioni — diciamo una società di consulenza ingegneristica o uno studio legale — che ha bisogno di un assistente IA interno per rispondere a domande sui propri documenti: rapporti passati, standard, contratti e note. I dati sono riservati e non possono lasciare il palazzo.

Invece di inviare quei dati a un servizio IA pubblico, lo studio fa qualcosa di diverso. Scarica un modello a pesi aperti — un modello i cui file addestrati sono pubblicati perché chiunque li esegua — e lo esegue sui propri server. Collega il modello ai suoi documenti tramite recupero, così l'assistente risponde dai file dello studio anziché dall'internet aperto. Nessuna domanda lascia la rete. Nessun fornitore legge il lavoro. Lo studio sceglie il modello, controlla i dati, e può cambiare o sostituire il sistema quando vuole.

Questo modello è reale e sempre più comune, ma lo studio specifico qui è un composito, non una singola azienda con un nome, perché le organizzazioni che lo fanno raramente lo pubblicizzano — tutto il senso è che il lavoro resti privato. Ciò che conta è che il modello esiste e funziona oggi con strumenti aperti pronti all'uso, esattamente come descrive il [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md).

**Una versione reale, con un nome, a scala nazionale.** Lo stesso istinto ora guida interi paesi. In Europa, due progetti finanziati mirano a costruire IA aperta e sovrana affinché il continente non dipenda da fornitori stranieri.

**OpenEuroLLM** è un consorzio europeo di venti partner che ha iniziato i lavori il 1 febbraio 2025, finanziato nell'ambito del programma Digital Europe dell'UE con circa 55 milioni di €. È coordinato da Jan Hajic dell'Università Carlo e co-guidato da Peter Sarlin di AMD Silo AI. Il suo obiettivo dichiarato è l'autonomia strategica per l'Europa nell'IA — costruire una capacità che l'Europa controlli.

Accanto ad esso, il progetto **EuroLLM**, sostenuto da Horizon Europe, dal Consiglio Europeo della Ricerca e dall'organizzazione di supercomputing EuroHPC, ha prodotto **EuroLLM-22B**, un grande modello linguistico completamente aperto costruito per tutte le 24 lingue ufficiali dell'UE. È stato addestrato sui supercomputer europei — il sistema MareNostrum 5 — e rilasciato come open source su Hugging Face, così chiunque può scaricarlo, ispezionarlo ed eseguirlo. Il lavoro si appoggia all'iniziativa "AI Factories" di EuroHPC, che mette in comune la capacità di supercomputing in tutta Europa; un bando ha allocato tre milioni di ore GPU sul Leonardo Booster al CINECA in Italia per costruire dati di addestramento aperti.

Perché raccontare questa storia qui? Perché mostra che "costruisci il tuo, tienilo aperto, tienilo sotto il tuo controllo" non è un hobby paranoico. È ora strategia ufficiale a livello di nazioni. La stessa logica che porta un paese a costruire il proprio modello aperto porta una piccola ditta a eseguire un modello aperto sul proprio server. La scala cambia; il principio è identico.

## Un esempio aziendale reale

### La clinica che non poteva inviare i suoi dati da nessuna parte

Una clinica medica privata vuole usare l'IA per riassumere le note dei pazienti e preparare bozze di corrispondenza di routine. I dati sono dati sanitari — il tipo più protetto secondo la legge, come spiega il [Capitolo 10](ch10-privacy-and-gdpr.md). Invierli a un servizio IA di terze parti solleva seri problemi legali ed etici, e la clinica non se la sente a prescindere dalla legge.

Così la clinica sceglie il controllo. Esegue un modello aperto sul proprio server, dentro la propria rete, dietro il proprio firewall. Il modello legge solo le note della clinica e risponde solo al personale della clinica. Nulla attraversa internet verso un fornitore. La clinica può dire con verità ai pazienti, ai regolatori e alla propria coscienza: questi dati non hanno mai lasciato il nostro edificio.

Il costo è reale. La clinica ha dovuto comprare hardware e trovare qualcuno che lo mantenesse. Il modello è buono ma non il migliore assoluto disponibile. Alcuni compiti hanno ancora bisogno di un umano. Ma la clinica ha guadagnato l'unica cosa che non poteva comprare da alcun fornitore: la certezza su dove vanno i suoi dati più sensibili.

Ora confronta la clinica con uno studio che non ci ha pensato e ha incollato dati dei pazienti in una chatbot gratuita. La differenza non è l'intelligenza. È che uno studio ha fatto prima le tre domande di sovranità, e l'altro non le ha mai fatte.

## Come si fa

### 11.1 Cos'è la sovranità digitale: una definizione semplice

La sovranità digitale è la capacità di controllare le proprie risorse e decisioni digitali, invece di dipendere da quelle di qualcun altro.

Scomposta, ha tre livelli.

**Sovranità dei dati.** Controlli dove i tuoi dati sono archiviati, chi può accedervi, e sotto quale legge ricadono. Puoi spostarli o cancellarli.

**Sovranità operativa.** Controlli i sistemi che elaborano i tuoi dati. Puoi eseguirli, cambiarli, e mantenerli funzionanti anche se un fornitore scompare.

**Sovranità strategica.** Controlli la tua direzione. Il tuo futuro non è ostaggio del prezzo di un fornitore, delle regole di un governo straniero, o delle decisioni di business di un fornitore.

La sovranità non è tutto-o-niente. È una manopola, non un interruttore. Puoi essere altamente sovrano su un processo e appena sovrano su un altro. L'obiettivo è decidere, di proposito, dove vuoi la manopola impostata per ogni parte del tuo business, anziché derivare verso ciò che è più comodo.

L'opposto della sovranità è una dipendenza che non hai scelto — uno stato in cui un cambiamento nei piani di qualcun altro forza un cambiamento nei tuoi.

### 11.2 Perché conta per le aziende: sapere dove sono i dati, chi vi accede, come sono elaborati

La sovranità conta perché le tre domande hanno conseguenze reali.

**Dove sono i dati.** I dati archiviati in un altro paese ricadono sotto le leggi di quel paese. Un'autorità straniera può essere in grado di imporre l'accesso. La ubicazione del centro dati di un fornitore non è un dettaglio minore; fissa il terreno legale su cui poggiano i tuoi dati.

**Chi vi accede.** Un servizio di terze parti può permettere al proprio personale, ai propri team di supporto e ai propri subappaltatori di raggiungere i tuoi dati, in paesi che non hai mai accettato. Potresti non vedere mai un elenco di loro. Sovranità significa che sai, o controlli, quell'accesso.

**Come sono elaborati.** Se l'elaborazione avviene dentro un sistema chiuso che non puoi ispezionare, non puoi verificare cosa fa con i tuoi dati né se sia equo. Se esegui tu il sistema, puoi guardare dentro.

Queste contano per tre ragioni pratiche. **Conformità:** leggi come il GDPR richiedono che tu conosca e controlli la gestione dei dati. **Sicurezza:** ogni parte in più con accesso è una possibilità in più di violazione. **Continuità operativa:** se un fornitore fallisce, alza i prezzi, o viene tagliato fuori da sanzioni, la sovranità è la differenza tra un contrattempo e una crisi.

La sovranità non è un'ideologia. È gestione del rischio per la parte del tuo business che gira sui dati.

### 11.3 Modelli proprietari contro modelli open source: cosa cambia davvero

La scelta tra un modello proprietario e un modello open source cambia parecchie cose insieme.

**Un modello proprietario** è un prodotto chiuso. Lo usi attraverso un servizio o un'API. Non puoi vedere come funziona, non puoi eseguirlo da solo, e non puoi cambiarlo. Dipendi dal proprietario per accesso, prezzo e continuità. La comodità è alta; il controllo è basso. Se il proprietario cambia i termini o ferma il servizio, ti adatti o ti fermi.

**Un modello open source o a pesi aperti** pubblica il suo codice o i suoi file addestrati così che tu possa scaricarlo ed eseguirlo da solo. Puoi ispezionarlo, eseguirlo sul tuo hardware, metterlo a punto, e continuare a usarlo anche se il creatore originale sparisce. Il controllo è alto; la comodità è più bassa, perché devi eseguirlo e mantenerlo.

Ciò che cambia davvero è **chi detiene il potere e chi porta il peso.** Il proprietario consegna il potere al fornitore e porta il peso per te. L'aperto consegna a te il potere e ti dà il peso.

Nessuno dei due è automaticamente migliore. Il proprietario è giusto quando vuoi capacità senza manutenzione e i dati non sono sensibili. L'aperto è giusto quando ti servono controllo, trasparenza o indipendenza, e puoi sostenere il lavoro. Molte aziende usano entrambi: proprietario per la comodità a basso rischio, aperto e autogestito per i dati e i processi che contano di più.

Una cautela: "aperto" è uno spettro, e la licenza conta. Alcuni modelli aperti limitano l'uso commerciale o come puoi descrivere il tuo uso. Leggi la licenza prima di costruirci sopra.

### 11.4 Il ruolo dell'open source: trasparenza, controllo, comunità

L'open source è lo strumento principale della sovranità digitale, per tre ragioni.

**Trasparenza.** Perché il codice o i pesi sono pubblicati, tu o un terzo potete leggerli e verificare cosa fa davvero il sistema. Non ti viene chiesto di fidarti di una scatola nera. È lo stesso istinto dietro le idee di auditing nel [Capitolo 7](ch07-trustless-trust-without-trusting.md).

**Controllo.** Puoi eseguirlo dove scegli, cambiarlo per adattarlo alle tue esigenze, e tenerlo finché vuoi. Nessuno può portartelo via o forzarti un aggiornamento che non hai chiesto.

**Comunità.** Un progetto aperto è mantenuto da molte persone, non dalla roadmap di un'unica azienda. I bug vengono trovati da estranei. Il progetto può sopravvivere al team originale. Non sei solo se qualcosa si rompe.

L'open source abbassa anche la barriera d'ingresso. Una piccola ditta può usare lo stesso modello aperto di una grande. Questo livella il campo in un modo che i prodotti proprietari non fanno.

Ma l'open source non è gratuito nel senso reale. Qualcuno deve installarlo, aggiornarlo, metterlo in sicurezza e sostenerlo. Se non hai nessuno che lo faccia, l'open source può diventare una passività. Una sovranità che non puoi mantenere è peggio di una comoda dipendenza. Usa l'open source dove hai, o puoi assumere, la capacità.

### 11.5 Come costruire un'infrastruttura IA sovrana: i passi concreti

Se decidi di acquisire controllo, ecco un percorso pratico.

1. **Decidi cosa deve essere sovrano.** Elenca i dati e i processi che non possono dipendere da estranei — dati sensibili, flussi di lavoro centrali, lavoro regolamentato. Non tutto ha bisogno del trattamento.
2. **Scegli modelli aperti.** Scegli modelli a pesi aperti la cui licenza si adatta al tuo uso. Abbina la dimensione al tuo compito, come spiega il [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md).
3. **Eseguili su un'infrastruttura che controlli.** Può essere un server nel tuo ufficio, una macchina nel tuo account cloud personale sotto le tue chiavi, o una workstation locale per un inizio piccolo.
4. **Tieni i dati locali e connessi.** Usa il recupero così l'assistente risponde dai tuoi documenti senza inviarli fuori.
5. **Controlla accessi e chiavi.** Tu detieni le credenziali. Nessun terzo ha una porta sul retro. Registra chi fa cosa.
6. **Pianifica la manutenzione.** Nomina chi installa, aggiorna, mette in sicurezza e fa il backup del sistema. Scrivi il runbook.
7. **Mantieni un'uscita da tutto.** Anche per le parti che tieni proprietarie, assicurati di poter esportare i dati e scambiare gli strumenti. La sovranità include la capacità di andarsene.
8. **Rivedi il terreno legale.** Conferma la residenza dei dati e i doveri dell'AI Act e del GDPR per la configurazione, come coprono il [Capitolo 5](ch05-rules-and-legal-responsibility.md) e il [Capitolo 10](ch10-privacy-and-gdpr.md).
9. **Inizia piccolo e cresci.** Sperimenta un flusso sovrano, prova che funziona, poi estendi. Non ricostruire tutta l'azienda in una volta.

Lo scopo non è l'indipendenza totale. È il controllo deliberato sulle parti che contano, con una linea chiara tra ciò che esegui e ciò che noleggi.

## Etica e responsabilità

La sovranità porta con sé i propri doveri etici, ed è facile sbagliarli.

**Il controllo non è la stessa cosa che buono.** Un sistema sovrano può comunque essere di parte, sbagliato o ingiusto. Eseguirlo tu stesso non lo rende etico. I doveri nel [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md) si applicano ancora.

**La sovranità non deve diventare segretezza.** "Noi lo controlliamo" non è una ragione per nascondere come tratti i dati delle persone. Devi ancora trasparenza a clienti e regolatori. Controlla il sistema; non nasconderti dal controllo altrui.

**Non usare la sovranità per schivare la cooperazione.** Alcuni problemi — frode, danni, richieste legali — richiedono di lavorare con le autorità. La sovranità riguarda proteggere gli innocenti, non bloccare la legittima supervisione.

**Sii onesto sui tuoi limiti.** Se dichiari piena sovranità ma non puoi correggere, fare il backup o verificare il sistema, la dichiarazione è vuota e fuorviante. Di' cosa controlli e cosa no.

**Valuta il bene collettivo.** Modelli aperti e ricerca condivisa avvantaggiano tutti. Un mondo in cui ogni ditta costruisce un silo chiuso perde qualcosa. L'approccio più sano è controllare ciò che è sensibile e contribuire a ciò che è condiviso.

## Errori da evitare

### 11.7 La sovranità fine a sé stessa

L'errore più comune è inseguire la sovranità come un ideale invece che come uno strumento.

La sovranità costa denaro, tempo e competenze. Se la insegui ovunque, spendi molto per controllare cose che non hanno mai avuto bisogno di controllo. Potresti costruire un costoso sistema in sede per dati che non sono mai stati sensibili, mentre un servizio economico e contrattualizzato ti avrebbe servito bene e liberato il tuo personale per lavoro vero.

Il test non è "posso controllare questo?". È "cosa perdo se non posso controllare questo?". Se la risposta è poco, non spendere per controllarlo. Riserva il tuo budget di sovranità per i dati e i processi dove perdere il farebbe davvero male — dati sensibili, lavoro regolamentato, e i sistemi senza cui il tuo business non può funzionare.

La sovranità è un mezzo, non un fine. Comprala dove il rischio giustifica il costo, e sii comodamente dipendente dove non lo fa.

Oltre quella trappola, fai attenzione a queste:

1. **Costruire una fortezza che non puoi mantenere.** Sovranità senza un manutentore diventa un sistema rotto e un falso senso di sicurezza.
2. **Confondere open source con gratuito.** Qualcuno deve eseguirlo. Mettilo a budget.
3. **Ignorare la licenza.** Aperto non significa sempre che puoi usarlo come ti pare.
4. **Dare per scontato che locale equivalga a sicuro.** Un server sovrano ha comunque bisogno di sicurezza, come copre il [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md).
5. **Tagliar fuori tutti i fornitori per principio.** Molti fornitori si guadagnano il loro posto. L'indipendenza totale raramente vale la pena.
6. **Nessun piano d'uscita per le parti che tieni a noleggio.** La sovranità include la capacità di lasciare qualsiasi singolo fornitore.
7. **Sovrapromettere ai clienti.** Non dichiarare un controllo che non hai.
8. **Ignorare che i modelli aperti possono comunque perdere dati.** Un modello addestrato su dati cattivi può comunque esporre dati personali, come nota il [Capitolo 10](ch10-privacy-and-gdpr.md).

## Esercizio pratico

### 11.8 Definisci il tuo livello desiderato di sovranità

Prendi un'ora e mappa i tuoi usi di IA su una semplice manopola di controllo.

Elenca ogni uso di IA nel tuo business. Per ciascuno, rispondi a tre domande e imposta un livello obiettivo.

- **Quanto è sensibile il dato?** Basso (pubblico o innocuo), Medio (interno), Alto (riservato al cliente, regolamentato o personale).
- **Quanto è critico il processo?** Basso (bello averlo), Medio (usato ogni giorno), Alto (il business si ferma senza).
- **Qual è il costo di perdere il controllo?** Basso, Medio o Alto.

Ora imposta un obiettivo per ciascuno:

- **Alta sensibilità o alta criticità → punta in alto.** Esegui tu o sotto un contratto che ti dia vero controllo e un'uscita.
- **Bassa sensibilità e bassa criticità → punta in basso.** Un comodo servizio di terze parti va bene; non sprecare denaro a controllarlo.
- **Misto → punta nel mezzo.** Usa un fornitore ma tieni i dati esportabili e il flusso di lavoro scambiabile.

Scrivi una frase per uso: *"Per [uso], voglio sovranità [alta/media/bassa] perché [ragione]."*

Il risultato è la tua mappa di sovranità. Dovrebbe mostrare un misto deliberato, non una singola risposta. Se tutto è "alto", stai spendendo troppo. Se tutto è "basso", sei esposto sulle cose che contano. Aggiusta finché la mappa corrisponde al tuo rischio reale.

## Checklist

### 11.9 I pilastri della sovranità digitale

Usa questo per verificare se una data configurazione IA ti dà vero controllo.

- [ ] **Sai dove sono archiviati i dati** — il paese e l'operatore.
- [ ] **Sai chi può accedervi** — personale del fornitore, subappaltatori e ogni portata governativa.
- [ ] **Puoi spostare o cancellare i dati** ogni volta che scegli.
- [ ] **Puoi esportare i tuoi dati** in un formato comune e utilizzabile (nessun lock-in).
- [ ] **Sai come sono elaborati i dati** — oppure esegui tu l'elaborazione.
- [ ] **Usi modelli aperti dove il controllo conta**, e hai letto le loro licenze.
- [ ] **Detieni le chiavi e le credenziali** dei sistemi che contano.
- [ ] **Hai un manutentore nominato** per tutto ciò che esegui tu, con un runbook scritto.
- [ ] **Hai un piano d'uscita** per ogni fornitore, così nessun singolo fornitore può tenerti in ostaggio.
- [ ] **Hai verificato il terreno legale** — residenza dei dati, GDPR e AI Act.
- [ ] **Hai impostato un livello di sovranità deliberato** per ogni uso, non un default.
- [ ] **Puoi verificare le tue stesse affermazioni** — se dici che i dati restano dentro, puoi provarlo.

Se un pilastro manca per un uso ad alto rischio, quella è la tua priorità da sistemare.

## Punti chiave

- La sovranità digitale significa controllare dove sono i tuoi dati, chi vi accede e come sono elaborati — ed essere in grado di rispondere a quelle tre domande per ogni strumento IA.
- È una manopola, non un interruttore: impostala deliberatamente in alto per il lavoro sensibile e critico, e in basso dove la comodità è innocua.
- I modelli open source e a pesi aperti ti danno trasparenza, controllo e comunità, ma solo se hai la capacità di eseguirli e mantenerli.
- La sovranità è un mezzo, non un fine; inseguirla ovunque spreca denaro, quindi comprala solo dove perdere il controllo farebbe davvero male.
- La vera sovranità include sempre un'uscita: tieni i tuoi dati esportabili così che nessun singolo fornitore possa tenere in ostaggio il tuo business.
