# Capitolo 14 — I dati: la materia prima

## In parole semplici

L'AI non pensa da sola. Lavora sui dati, come una cucina lavora sugli ingredienti. La qualità del piatto dipende dalla qualità di ciò che ci metti. Nessuno chef, per quanto bravo, può fare un buon piatto con verdure marce. Con l'AI è lo stesso: buoni dati in entrata, risultati utili in uscita; cattivi dati in entrata, risultati inutili o dannosi.

Questa è la verità più importante sull'AI che i titolari d'azienda non colgono. Si concentrano sul modello — quanto è intelligente, quale marca comprare — e ignorano i dati su cui gira. Ma il modello è solo lo chef. I dati sono il cibo. La maggior parte dei progetti di AI fallisce non perché il modello era debole, ma perché i dati erano disordinati, incompleti o sbagliati.

I dati, in parole povere, sono informazioni registrate. Nomi dei clienti, storici degli ordini, fatture, email, fogli di calcolo, archivi dei dipendenti, clic sul sito, letture delle macchine — tutto dati. Una parte è in ordine, seduta in tabelle pulite. La maggior parte è disordinata, sparsa fra file, caselle di posta e carta. Il tuo compito è sapere cosa hai, dove si trova, ed è abbastanza buono per costruirci sopra.

Questo capitolo parla di trattare i tuoi dati come la preziosa materia prima che sono. Copre quali dati hai e dove vivono, come capire se sono puliti e aggiornati, le regole di base per i dati personali, come tenerli al sicuro e come organizzarli senza stravolgere tutta l'azienda. Il trattamento legale approfondito della privacy è nel [Capitolo 10](ch10-privacy-and-gdpr.md); questo capitolo ti dà le basi operative per preparare i tuoi dati all'AI.

Un'immagine semplice da tenere a mente: prima di cucinare, controlli la dispensa. Vedi cosa hai, butti ciò che è andato a male, e annota cosa manca. È esattamente ciò che fai con i dati prima di ogni progetto di AI.

## Un po' di storia

**Anni '60–'70: i dati vivono nei database.** Le aziende conservavano le informazioni in database strutturati — tabelle pulite di numeri e testi brevi. Era tutto pulito per costruzione, ma copriva solo una piccola fetta di ciò che l'azienda sapeva. La maggior parte della conoscenza viveva su carta o nella testa delle persone.

**Anni '80–'90: fogli di calcolo e file.** I personal computer hanno sparso i dati ovunque. Fogli di calcolo, unità condivise, allegati email. I dati sono diventati abbondanti ma sparsi e incoerenti. Il disastro che tutti conosciamo oggi è iniziato qui.

**Anni 2000: "big data".** Internet e i sistemi digitali hanno prodotto dati a una scala mai vista. Le aziende hanno iniziato a parlare di "big data" come di un asset. Ma la quantità senza qualità ha creato un nuovo problema: oceani di dati, poca parte affidabile.

**Anni 2010: la qualità dei dati diventa il collo di bottiglia.** Con la crescita dell'analisi e del machine learning, è emersa una verità dura: la maggior parte dei progetti passava l'80% del tempo a pulire i dati, non a modellarli. "Spazzatura dentro, spazzatura fuori" è diventata la lezione simbolo dell'epoca. La preparazione dei dati, non gli algoritmi geniali, era il vero lavoro.

**2018: il GDPR alza la posta.** La legge europea sulla privacy ha reso la gestione dei dati un dovere legale, non solo una questione di qualità. Ora i dati disordinati non erano solo inutili; i dati personali mal gestiti erano punibili. La governance dei dati è diventata un tema da consiglio di amministrazione.

**Anni 2020: l'AI generativa conta la portata dei dati.** L'AI moderna sa leggere testi e immagini disordinati, quindi ha bisogno di dati meno in ordine dei vecchi sistemi. Ma dipende comunque dall'avere i dati giusti disponibili e affidabili. La lezione resta: il modello vale quanto ciò che gli dai da mangiare.

L'arco è chiaro. Siamo passati da troppi pochi dati strutturati a troppi dati sparsi. L'abilità non è mai cambiata: trovarli, pulirli e sapere di cosa ti puoi fidare.

## Curiosità

### 14.6 Il modello che scriveva Python da libri degli anni '30

Ecco un fatto sorprendente su come i dati plasmano ciò che un modello sa fare: dei ricercatori hanno addestrato un modello linguistico solo su libri precedenti al 1931 — niente computer, niente internet e nessun codice di programmazione, perché Python non esisteva ancora — eppure sapeva scrivere un po' di Python, copiando la struttura degli esempi che gli mettevano davanti.

Quell'esperimento, e ciò che insegna su dati e struttura, è raccontato per intero nel [Capitolo 3](ch03-the-words-of-ai-without-the-big-words.md), la sua casa canonica. Il punto per questo capitolo è una riga: **ciò che un modello sa fare dipende interamente da ciò che gli è stato dato.** Cambia i dati, e cambi la capacità. Ecco perché i tuoi dati sono la materia prima che vale la pena curare.

## Un esempio reale di azienda

### Il grossista i cui "dati" erano tre fogli di calcolo in conflitto

Un grossista di materiali edili credeva di avere buoni dati sui clienti. Quando ha provato a usare l'AI per prevedere quali prodotti avrebbe ordinato ogni cliente, il progetto si è arenato nella prima settimana. Il motivo erano i dati, non il modello.

Le informazioni sui clienti vivevano in tre posti: un vecchio sistema contabile, un foglio di calcolo delle vendite tenuto da un agente, e una mailing list in un programma di posta. Lo stesso cliente compariva tre volte con tre grafie e indirizzi diversi. Gli storici degli ordini non coincidevano fra i sistemi. Metà dei record non aveva il numero di telefono. I dati non erano esattamente sbagliati — erano frammentati e incoerenti, il che è altrettanto grave.

La soluzione non era high-tech. Hanno scelto un sistema come unica fonte di verità per gli archivi clienti. Hanno fuso i duplicati a mano. Hanno messo una regola semplice: ogni nuovo cliente entra in quell'unico sistema, una volta sola. È servito qualche settimana di lavoro poco entusiasmante. Dopo, il progetto di previsione ha funzionato, perché per la prima volta c'era un unico insieme affidabile di dati su cui costruire.

La lezione: l'AI era pronta. I dati no. La maggior parte dei progetti di AI aspetta i dati, non gli strumenti.

## Come si fa

### 14.1 Quali dati hai e dove sono

Non puoi usare ciò che non riesci a trovare. Il primo passo è un inventario dei dati: un semplice elenco di ogni posto in cui la tua azienda conserva informazioni.

Percorri la tua azienda ed elenca ogni fonte di dati. Quelle tipiche:

- **Sistemi aziendali.** Software di contabilità, CRM, magazzino, piattaforma e-commerce, sistema HR.
- **File e fogli di calcolo.** Unità condivise, portatili personali, Google Drive, file Excel.
- **Email e messaggi.** Caselle di posta, strumenti di chat, conversazioni salvate.
- **Carta.** Archivi fisici, moduli firmati, appunti.
- **Tracce web e digitali.** Analytics del sito, log delle app, attività del portale clienti.
- **Dati esterni.** Feed dei fornitori, dati di mercato, registri pubblici.

Per ogni fonte, annota quattro cose: cosa contiene, chi lo possiede, più o meno quanto ce n'è, e quanto è aggiornato. Non puntare alla perfezione; punta a una mappa. Vuoi vedere tutto il paesaggio, così sai dove sono i dati buoni e dove sono le lacune.

Aspettati sorprese. La maggior parte dei titolari scopre dati che aveva dimenticato e lacune che dava per colmate. L'inventario in sé è prezioso perché trasforma un vago sentore di "abbiamo dati da qualche parte" in un quadro chiaro.

Un buon inventario è una tabella. Tienila semplice e aggiornala man mano. Diventa il riferimento per ogni futuro progetto di AI.

### 14.2 Dati puliti, completi e aggiornati

Una volta che sai cosa hai, giudica la sua qualità. I dati buoni hanno tre qualità.

**Puliti.** Liberi da errori, duplicati e incoerenze. Lo stesso cliente non è scritto in tre modi. I numeri sono davvero numeri, non testo. Le date sono date vere. Pulire significa correggere o eliminare i record cattivi.

**Completi.** Hanno compilati i campi che ti servono. Se ti serve la regione di un cliente per prevedere la domanda, ma metà dei record non ha la regione, i dati sono incompleti. Completezza significa che i campi importanti sono compilati.

**Aggiornati.** Riflettono la realtà adesso, non tre anni fa. Una lista clienti dove metà delle aziende si è trasferita o ha chiuso è stantia. I dati stantii portano a conclusioni sbagliate, non importa quanto puliti sembrino.

Come verificare la qualità senza strumenti speciali:

- **Controllo a campione.** Prendi 20 record a caso e cerca errori, duplicati e campi vuoti. Il tasso di errore che vedi è più o meno il tasso di errore che hai.
- **Conta i vuoti.** Per i campi che ti servono, quale quota è vuota? Molti vuoti significano bassa completezza.
- **Controlla le date.** Quando è stata aggiornata ogni fonte l'ultima volta? Vecchio significa stantio.

Non ti servono dati perfetti. Ti servono dati abbastanza buoni per il compito specifico. Una previsione approssimativa tollera più rumore di una fattura cliente. Adatta l'asticella della qualità al lavoro. Ma sappi dove stai prima di costruire.

Pulire è lavoro vero e spesso noioso. Mettilo a budget. È l'80% del progetto che tutti dimenticano di pianificare.

### 14.3 Dati personali e GDPR: regole di base

Alcuni dei tuoi dati sono dati personali — qualsiasi informazione su una persona vivente identificabile: nomi, email, numeri di telefono, indirizzi, ID cliente, perfino un indirizzo IP. I dati personali portano doveri legali, e il trattamento completo è nel [Capitolo 10](ch10-privacy-and-gdpr.md). Ecco le basi operative che ti servono prima di usarli con l'AI.

**Sappi cosa è personale.** Segna, nel tuo inventario, ogni fonte che contiene dati personali. Non puoi proteggere ciò che non hai identificato.

**Abbi una ragione lecita.** Sotto il GDPR, puoi trattare dati personali solo su una valida base giuridica — per esempio, un contratto con la persona, il suo consenso, o un legittimo interesse che non prevalga sui suoi diritti. Sappi su quale base ti appoggi prima di dare i dati all'AI.

**Usa solo ciò che serve.** Non riversare tutti i tuoi dati personali in uno strumento di AI quando il compito ne richiede solo una parte. Riduci al minimo ciò che usi.

**Guarda dove va.** Se invii dati personali a un servizio di AI di terze parti, i dati escono dal tuo controllo e il GDPR li segue fuori dalla porta. La gestione del fornitore diventa tua responsabilità. I rischi delle terze parti sono nel [Capitolo 9](ch09-third-party-services-and-shadow-ai.md).

**Rispetta i diritti delle persone.** Le persone possono chiedere di vedere, correggere o cancellare i loro dati. Il tuo uso dell'AI non deve rendere ciò impossibile.

Questa è una guida semplice, non un parere legale. Per decisioni vere, soprattutto oltre confine, consulta un professionista della protezione dei dati. Ma l'abitudine — segnare i dati personali, conoscere la tua base, usare il minimo — tocca a te costruirla ora.

### 14.4 Sicurezza, backup e accessi

I dati sono un asset, e gli asset vanno protetti. Tre basi coprono la maggior parte del rischio.

**Sicurezza.** Proteggi i dati da attaccanti e fughe. Usa password robuste e autenticazione a più fattori, tieni i sistemi aggiornati, crittografa i dati sensibili, e fai attenzione ad allegati e link nelle email. Il quadro completo della sicurezza, incluse le minacce specifiche dell'AI, è nel [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md).

**Backup.** Tieni copie dei tuoi dati al sicuro dal sistema principale. Se un sistema si schianta, viene colpito da ransomware, o un file viene cancellato, il backup è la differenza fra una giornata storta e perdere l'azienda. Segui una regola semplice: tieni copie in più di un posto, fai il backup regolarmente, e verifica di poter davvero ripristinare. Un backup di cui non hai mai testato il ripristino è solo una speranza.

**Accessi.** Controlla chi può vedere e modificare cosa. Non tutti hanno bisogno di accesso a tutto. Dai alle persone l'accesso minimo che il loro ruolo richiede. Registra chi accede ai dati sensibili. Limitare l'accesso limita sia gli incidenti sia i furti.

Queste tre lavorano insieme. La sicurezza tiene fuori gli estranei. Il backup ti salva quando qualcosa va storto comunque. Gli accessi limitano il danno che una singola persona o un singolo errore possono fare. Nessuna di esse è opzionale.

Un'abitudine pratica: fai il backup in automatico, controlla il backup ogni mese, e rivedi chi ha accesso ogni trimestre. Piccole routine, ripetute, prevengono i disastri.

### 14.5 Come organizzare i dati senza stravolgere tutto

La paura più grande sul lavoro coi dati è che significhi un'enorme, dirompente revisione generale. Non è così. Puoi migliorare i tuoi dati passo dopo passo senza fermare l'azienda.

**Scegli una fonte di verità per ogni cosa.** Per ogni tipo importante di dati — clienti, prodotti, ordini — scegli un sistema che sia quello ufficiale. Tutto il resto diventa una copia o una vista. Questa singola regola risolve la maggior parte della confusione senza cambiare i tuoi strumenti.

**Correggi al punto di ingresso.** Il momento più economico per pulire i dati è quando vengono creati. Metti regole semplici così che i nuovi record vadano nel posto giusto, una volta sola, con i campi chiave compilati. Fermare il nuovo disastro batte pulire quello vecchio per sempre.

**Non voler svuotare il mare.** Non provare a pulire tutto. Pulisci solo i dati che i tuoi primi progetti di AI richiedono. Dati perfetti che non usi mai sono uno sforzo sprecato. Una pulizia mirata che serve a un progetto reale vale la pena farla.

**Standardizza un poco, non alla perfezione.** Mettiti d'accordo su pochi formati semplici — come scrivere una data, un numero di telefono, un nome cliente — e applicali da ora in poi. Non ti serve uno standard grandioso, solo coerenza per i campi che contano.

**Migliora man mano.** Tratta la qualità dei dati come un'abitudine, non un progetto. Ogni piccola correzione rende più facile il prossimo uso dell'AI. In un anno, piccoli miglioramenti costanti si sommano in una solida base di dati.

La mentalità: non stai ricostruendo la casa. Stai riordinando la dispensa, uno scaffale alla volta, così il prossimo piatto è più facile da cucinare. Inizia dallo scaffale che serve al tuo primo progetto.

## Etica e responsabilità

I dati portano un peso etico oltre la qualità e la legge.

**I dati personali sono persone.** Dietro ogni record c'è una persona con diritti e sentimenti. Trattala tenendo questo a mente, non solo come una risorsa da scavare. I principi sono nel [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md).

**Il bias vive nei dati.** Se i tuoi dati sottorappresentano un gruppo, l'AI addestrata su di essi tratterà male quel gruppo. Un set di dati per le assunzioni con per lo più un solo tipo di candidato biascerà l'AI nello stesso modo. Controlla i dati di chi manca, non solo se i dati sono puliti.

**Non usare dati che le persone non si aspettano.** Il fatto che tu detenga dati non significa che li debba usare per qualsiasi scopo. Usare i dati dei clienti in un modo a cui non hanno mai acconsentito rompe la fiducia, anche se è legale. Resta entro le aspettative ragionevoli.

**Sii onesto su cosa raccoglii e perché.** Dì alle persone quali dati raccogli e come li usi. Una raccolta nascosta è una violazione della fiducia e spesso della legge.

**Proteggili come se fossero tuoi.** Una violazione danneggia persone vere, non solo la tua reputazione. Tratta la sicurezza come un dovere verso le persone nei tuoi dati, non solo una casella da spuntare.

## Errori da evitare

### 14.7 Errori comuni con i dati

1. **Ignorare i dati finché il progetto non fallisce.** L'errore più comune. Controlla i tuoi dati prima di iniziare, non dopo che si è arenato.
2. **Dare per scontato di avere dati quando hai frammenti.** Tre fogli di calcolo in conflitto non sono un set di dati. Trova prima la verità.
3. **Confondere la quantità con la qualità.** Tanti dati non sono dati buoni. Un piccolo set pulito batte uno grande e disordinato.
4. **Non pianificare il tempo di pulizia.** La preparazione dei dati è la maggior parte del lavoro. Mettila a budget o il progetto slitta.
5. **Nessuna unica fonte di verità.** Multiple versioni "ufficiali" garantiscono confusione. Scegline una.
6. **Usare dati personali senza una base lecita.** Un rischio legale e un rischio di fiducia. Conosci prima la tua base.
7. **Inviare dati personali a un'AI di terze parti con noncuranza.** Il GDPR segue i dati fuori dalla porta.
8. **Backup non testati.** Un backup che non può ripristinare non è un backup. Testalo.
9. **Tutti hanno accesso a tutto.** Un accesso ampio significa un rischio ampio. Limitarlo al ruolo.
10. **Provare a pulire tutto in una volta.** Paralisi da revisione. Pulisci solo ciò che il tuo progetto richiede.
11. **Ignorare i dati stantii.** Dati puliti ma vecchi danno comunque risposte sbagliate. Controlla le date.
12. **Dimenticare il bias nei dati.** Una lacuna su chi è rappresentato diventa un bias nell'output.

## Esercizio pratico

### 14.8 Inventario dei dati

Passa un pomeriggio a costruire un semplice inventario dei dati. È la preparazione più utile in assoluto che tu possa fare per l'AI.

Fai una tabella con una riga per ogni fonte di dati. Per ciascuna, compila:

- **Fonte** — il sistema, il file o il posto (per es. "software di contabilità", "foglio di calcolo vendite", "casella email").
- **Cosa contiene** — clienti, ordini, fatture, CV, ecc.
- **Responsabile** — chi ne è responsabile.
- **Volume** — più o meno quanto (righe, file, GB).
- **Dati personali?** — Sì / No.
- **Qualità** — controlla a campione 20 record; annota vuoti, duplicati, errori. Valuta pulito / misto / scarso.
- **Aggiornato?** — quando è stato aggiornato l'ultima volta.
- **Unica fonte di verità?** — Sì / No / candidato.

Riempi ogni fonte che riesci a trovare. Quando hai finito, guarda il quadro:

- Quali fonti sono pulite e aggiornate? Quelle sono la tua miglior materia prima di partenza.
- Quali contengono dati personali? Marchiale per le basi GDPR del 14.3.
- Dove hai duplicati senza un'unica fonte di verità? Quelli sono i tuoi primi obiettivi di ripulitura.
- Cosa manca che il tuo primo progetto di AI richiede? Quelle sono lacune da colmare.

Questa tabella ti dice, onestamente, se sei pronto a iniziare un progetto di AI o se devi prima sistemare i dati. Conservalo e aggiornalo. È la lista della dispensa per tutto ciò che costruirai dopo.

## Checklist

### 14.9 Checklist dei dati

Prima di dare dati in pasto a un progetto di AI, controlla queste cose.

- [ ] **Hai un inventario dei dati** che elenca ogni fonte e cosa contiene.
- [ ] **Sai dove sono i dati buoni** e dove sono le lacune.
- [ ] **Hai un'unica fonte di verità** per ogni tipo chiave di dati.
- [ ] **Hai controllato a campione la qualità** e conosci il tasso di errori e vuoti.
- [ ] **I dati sono abbastanza puliti per il compito specifico** che stai facendo.
- [ ] **I dati sono aggiornati** e riflettono la realtà attuale.
- [ ] **Hai segnato tutti i dati personali** nell'inventario.
- [ ] **Hai una base lecita** per ogni dato personale che usi (vedi [Capitolo 10](ch10-privacy-and-gdpr.md)).
- [ ] **Usi solo il minimo di dati personali** che il compito richiede.
- [ ] **Sai dove vanno i dati** se un servizio di AI di terze parti li tocca.
- [ ] **Le basi della sicurezza sono in atto** — autenticazione robusta, aggiornamenti, crittografia per i dati sensibili.
- [ ] **I backup esistono, sono recenti e sono stati testati per il ripristino.**
- [ ] **Gli accessi sono limitati** ai ruoli che ne hanno bisogno, con registrazione sui dati sensibili.
- [ ] **Stai correggendo i nuovi dati al punto di ingresso**, non solo pulendo quelli vecchi.
- [ ] **Hai controllato il bias** — i dati di chi mancano?

Se una casella è vuota e il tuo progetto dipende da essa, sistemala prima di costruire. I dati buoni non sono un dettaglio; sono la materia prima su cui gira tutto il resto.

## Punti chiave

- I dati sono la materia prima dell'AI: buoni dati in entrata, risultati utili in uscita; cattivi dati in entrata, risultati inutili o dannosi — il modello è solo lo chef.
- Inizia con un inventario dei dati: non puoi usare ciò che non riesci a trovare, e la maggior parte dei titolari è sorpresa da ciò che ha e da ciò che manca.
- La qualità significa puliti, completi e aggiornati; pianifica il tempo di pulizia, perché è la maggior parte del lavoro che tutti dimenticano.
- I dati personali portano doveri legali — marchiali, conosci la tua base lecita, usa il minimo, e ricorda che il GDPR li segue fino a qualsiasi servizio di terze parti.
- Puoi migliorare i dati passo dopo passo senza una revisione generale: scegli un'unica fonte di verità, correggi al punto di ingresso, e pulisci solo ciò che il tuo progetto richiede.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come appare lo stesso lavoro con AgentBridge. Ogni riquadro mostra il risultato finito e la riga che digiti per ottenerlo.

### Fai domande sui tuoi file

![L'agente che risponde dai tuoi documenti](../../assets/examples/ask-your-documents.png)
*L'agente che risponde dai tuoi documenti*

**Cosa chiedi:** `Qual è la nostra politica di recesso con il fornitore di stampa?`

L'agente cerca nella tua area documenti e risponde con ciò che i tuoi file dicono davvero, indicando la fonte.

*Suggerimento: Tieni i file della tua azienda nell'area documenti e diventano conoscenza consultabile.*

---

### Trova quel vecchio documento

![Una ricerca nel tuo archivio indicizzato](../../assets/examples/find-in-archive.png)
*Una ricerca nel tuo archivio indicizzato*

**Cosa chiedi:** `Trova la proposta che ho mandato all'hotel la scorsa primavera sul restyling della hall.`

L'agente cerca nel tuo archivio indicizzato e ti riporta il documento che intendevi, anche quando lo ricordi solo a metà.

*Suggerimento: L'indice si aggiorna man mano che aggiungi file, così l'archivio è sempre aggiornato.*

---

### Ricorda come ti piacciono le cose

![L'agente che applica le tue preferenze salvate](../../assets/examples/remember-preferences.png)
*L'agente che applica le tue preferenze salvate*

**Cosa chiedi:** `Fai una fattura — sai come mi piacciono.`

L'agente ricorda il tuo stile e le tue impostazioni da prima e le applica senza che tu debba ripeterli.

*Suggerimento: Puoi correggerlo in qualsiasi momento; aggiorna ciò che ricorda.*

---

### Non si perde nulla

![La cronologia delle versioni ti permette di tornare indietro in sicurezza](../../assets/examples/version-history.png)
*La cronologia delle versioni ti permette di tornare indietro in sicurezza*

**Cosa chiedi:** `Mostrami la versione precedente del contratto e ripristinala.`

Ogni versione creata dall'agente viene conservata. Puoi vedere la bozza precedente e riportarla indietro, così modificare è sempre sicuro.

*Suggerimento: È per questo che puoi lasciare che l'agente riscriva liberamente — la cronologia ti protegge.*

<!-- END agentbridge-examples -->
