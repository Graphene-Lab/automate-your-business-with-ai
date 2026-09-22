# Capitolo 20 — Implementare l'IA in modo sicuro

## In parole semplici

Quando porti l'IA nella tua azienda, stai lasciando che un nuovo lavoratore gestisca i tuoi dati. Come ogni lavoratore, anche quel nuovo lavoratore deve essere fidato, sorvegliato e delimitato. Questo capitolo riguarda il fare questo — come usare l'IA senza perdere i dati dei tuoi clienti, i tuoi conti o i tuoi segreti.

La sicurezza non è un prodotto che compri. È un insieme di abitudini che costruisci. L'obiettivo è semplice: **progetta le tue automazioni così che anche quando qualcosa va storto, i tuoi dati restino protetti.** Quell'idea ha un nome — **sicurezza by design** — e significa che pensi alla sicurezza all'inizio, non come ripensamento dopo una violazione.

Una buona analogia è una casa. Non lasci la porta d'ingresso spalancata perché "non è ancora successo niente di male". Chiudi le porte a chiave, limiti quali stanze possono entrare gli ospiti, metti una luce su un timer, e hai un piano se torni a casa e trovi una finestra aperta. La sicurezza dell'IA è lo stesso pensiero a strati: controlla chi entra, proteggi ciò che è dentro, sorveglia cosa succede, e sappi cosa fare se qualcosa si rompe.

Questo capitolo copre le abitudini centrali: progettare automazioni sicure, controllare chi può fare cosa, cifrare i dati così che siano illeggibili ai ladri, sorvegliare e registrare cosa fa l'IA, pianificare per il giorno in cui qualcosa va storto, e formare il tuo personale — perché il fattore umano è la prima linea di difesa.

Una verità onesta subito: nessun sistema è perfettamente sicuro. L'obiettivo non è la perfezione; è rendere la tua azienda un bersaglio difficile e mai un bersaglio facile. La maggior parte degli attacchi va al bersaglio facile. Una buona sicurezza semplice ti sposta da facile a difficile.

## Un po' di storia

**Anni 1970–1980: la sicurezza parte dal perimetro.** La prima sicurezza informatica si concentrava sul tenere fuori gli estranei — firewall, password, sale server chiuse a chiave. Il modello era un castello: mura forti, tutto dentro è sicuro. Questo funzionò finché le persone non ebbero bisogno di connettersi e condividere, il che incrinò le mura.

**Anni 1990: il perimetro si dissolve.** Internet e la posta elettronica significarono che i dati cominciarono a muoversi. Il modello del castello si ruppe. Virus e intrusioni arrivavano attraverso le stesse connessioni che rendevano possibile il business. La sicurezza doveva seguire i dati, non solo sorvegliare la porta.

**Anni 2000: "privilegio minimo" e difesa in profondità.** Il pensiero sulla sicurezza si spostò verso l'interno. Il principio del **privilegio minimo** — dai a ogni utente e programma solo l'accesso di cui ha assolutamente bisogno, niente di più — divenne centrale. Così come la **difesa in profondità**: molti strati sovrapposti, così se uno fallisce, un altro intercetta la minaccia.

**Anni 2010: "dai per scontato la violazione".** Gli esperti capirono che non puoi sempre tenere fuori gli attaccanti. La nuova mentalità era *dare per scontato* che un intruso possa già essere dentro, e concentrarsi sul limitare ciò a cui può arrivare e individuarlo in fretta. Registrazione, monitoraggio e risposta rapida divennero importanti quanto le mura.

**Anni 2020: l'IA aggiunge una nuova superficie di attacco.** L'IA porta nuovi modi di essere danneggiati — trucchi che ingannano l'IA stessa, avvelenamento dei dati, e il rischio di dare in pasto dati sensibili a strumenti che non controlli. (Queste minacce specifiche sono coperte nel [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md).) I vecchi principi — privilegio minimo, difesa in profondità, dai per scontato la violazione — si applicano ancora, ora applicati a un nuovo tipo di lavoratore.

L'arco: da un castello con una sola mura a molti strati che danno per scontato che la mura possa essere violata. La lezione non è mai cambiata: proteggi i dati stessi, non solo la porta.

## Curiosità

### 20.7 L'azienda che intercettò un attacco in un log che nessuno guardava

*L'azienda specifica in questa storia è illustrativa — un composito realistico, non una ditta nominata. Lo schema dietro di essa è reale e ben documentato.*

Immagina un'azienda di medie dimensioni che aveva un sistema di registrazione — un record di tutto ciò che accadeva sulla sua rete. I log giravano costantemente, registrando fedelmente ogni login, ogni file a cui si accedeva, ogni richiesta insolita. Per mesi, nessuno li leggeva. Erano lì, come una telecamera di sicurezza che nessuno guarda.

Poi un giorno un nuovo tecnico, facendo pulizia, diede un'occhiata ai log e vide qualcosa di strano: un programma contattava un indirizzo esterno a ore strane, prelevando dati lentamente e con costanza. Lo faceva da settimane. Nessuno se n'era accorto perché nessuno guardava. Quando finalmente guardarono, trovarono un intruso che era stato silenziosamente dentro molto più a lungo di quanto chiunque immaginasse.

La lezione scomoda non è che l'azienda fosse negligente. È che **l'evidenza era lì per tutto il tempo — ed è stata ignorata.** L'azienda aveva investito nella telecamera ma non nel guardarla.

Questo schema non è finzione. Il rapporto annuale *Cost of a Data Breach* dell'IBM ha scoperto, anno dopo anno, che le violazioni richiedono molto tempo per essere rilevate — nell'ordine dei **duecento giorni** in media nelle edizioni recenti — e che una larga quota viene notata per la prima volta da qualcuno fuori dall'azienda, non dal monitoraggio dell'azienda stessa. I log e i segnali spesso esistono. Ciò che manca è una persona che li guardi.

Per le tue automazioni di IA, la lezione è diretta: **un log che nessuno legge non è sicurezza.** Se raccogli registri di ciò che la tua IA fa, assegna qualcuno a guardare davvero, e imposta allarmi così che i segnali importanti trovino un umano invece di aspettare di essere scoperti.

## Un esempio di business reale

*Il seguente è un composito illustrativo di comuni schemi del mondo reale, non una singola azienda nominata.*

Un piccolo rivenditore online voleva che l'IA redigesse email di supporto ai clienti. Il modo facile e rischioso era dare all'IA pieno accesso all'intero database clienti — nomi, indirizzi, storico pagamenti — e lasciarlo leggere ciò di cui aveva bisogno. Il titolare si fermò e invece fece la cosa più sicura.

Derono all'IA accesso **in sola lettura** solo ai dettagli degli ordini di cui aveva bisogno per rispondere a una domanda di spedizione — non ai registri di pagamento, non alla scheda cliente completa. Lo configurarono così che l'IA potesse redigere ma un umano premesse invia. Attivarono un log che registrava ogni ordine che l'IA toccava. Dissero al team di supporto cosa l'IA poteva e non poteva vedere, e chiesero loro di segnalare qualsiasi cosa strana.

Dopo tre settimane, il log mostrò che all'IA era stato chiesto — da un cliente sveglio — di rivelare l'indirizzo di un altro cliente fingendo di essere quella persona. L'IA aveva rifiutato, perché non le era stato dato accesso a quei dati fin dall'inizio. Il tentativo fallì senza danni, e il log lo catturò così il team imparò che il trucco esisteva.

Se il titolare avesse preso la strada facile e dato all'IA l'intero database, lo stesso trucco avrebbe potuto funzionare. La progettazione sicura — minimo accesso, umano sull'invio, un log sorvegliato — trasformò una potenziale violazione in un non-evento. Ecco come appare la sicurezza by design nella pratica.

## Come fare

### 20.1 Principi di sicurezza by design: come progettare un'automazione che non espone dati

La sicurezza by design significa che costruisci la sicurezza nell'automazione dal primo schizzo. Fai queste domande prima di costruire qualsiasi cosa:

- **Di quali dati ha davvero bisogno questa automazione?** Usa il meno possibile. Se le serve solo un numero d'ordine, non darle l'intera scheda cliente.
- **Qual è il peggio che potrebbe succedere se perde dati o viene ingannata?** Immagina il fallimento. Progetta così che il caso peggiore sia piccolo.
- **Dove vanno i dati?** Conosci ogni sistema che i dati toccano, soprattutto fuori dal tuo controllo. Non dare in pasto dati sensibili a uno strumento che non puoi giustificare.
- **Un umano può fermarla?** Costruisci un kill switch — un modo per spegnere l'automazione istantaneamente se si comporta male.
- **Fallisce in modo sicuro?** Se qualcosa si rompe, l'automazione dovrebbe fermarsi e proteggere, non aprirsi. Una porta che si chiude quando salta la corrente è "a prova di guasto".

Il principio centrale è il **privilegio minimo**: accesso minimo, portata minima, dati minimi. Un'automazione che non ha mai avuto accesso ai dati sensibili non può perderli, non importa quanto ingegnoso sia l'attacco. Progetta fuori l'accesso, e il rischio se ne va con esso.

### 20.2 Controllo degli accessi: chi può fare cosa

Il controllo degli accessi è semplicemente decidere chi è autorizzato a fare cosa, e farlo rispettare. È la serratura su ogni stanza, non solo sulla porta d'ingresso.

Tre regole semplici:

- **Dai a ogni persona e a ogni strumento solo l'accesso che il suo lavoro richiede.** Uno strumento di supporto che risponde a domande di spedizione ha bisogno di dati sugli ordini, non di dati sulle paghe. Un dipendente junior non dovrebbe avere lo stesso accesso del titolare.
- **Separa i compiti.** La persona che configura l'IA non dovrebbe essere l'unica che può approvare le sue azioni, né l'unica che può vedere i log. Distribuisci le chiavi così che nessun singolo account compromesso possa fare tutto.
- **Rivedi gli accessi quando le persone cambiano.** Quando il personale entra, si sposta o esce, aggiorna il loro accesso lo stesso giorno. Un vecchio accesso che persiste è uno dei modi più comuni in cui avvengono le violazioni.

Usa gli strumenti che i tuoi sistemi già hanno — ruoli utente, permessi e controlli di login. Attiva l'**autenticazione a due fattori** (un secondo passo oltre la password, come un codice sul telefono) ovunque puoi. Ferma la maggior parte degli attacchi con password rubate.

### 20.3 Cifratura: proteggere i dati in transito e a riposo

La **cifratura** significa mescolare i dati così che solo chi ha la chiave giusta possa leggerli. A un ladro, i dati cifrati sembrano un nonsenso. Protegge i dati in due stati:

- **In transito** — dati che si muovono tra luoghi, come un'email o un caricamento di file. La cifratura qui significa che un ladro che intercetta il filo vede spazzatura. Cerca "https" e connessioni sicure.
- **A riposo** — dati fermi, come file su un disco o record in un database. La cifratura qui significa che un ladro che ruba il disco rigido comunque non riesce a leggerlo.

Per una piccola impresa, i passi pratici sono semplici: usa strumenti che cifrano per impostazione predefinita (la maggior parte dei servizi affidabili lo fa), controlla che le connessioni siano sicure (https), e chiedi direttamente a qualsiasi fornitore: "I miei dati sono cifrati in transito e a riposo?" Un fornitore serio risponde sì e spiega come. Se non possono, è un avvertimento.

Una cautela: la cifratura protegge i dati dagli estranei. Non protegge da qualcuno che ha la chiave e la usa male. È per questo che il controllo degli accessi (20.2) e la cifratura funzionano insieme — la cifratura nasconde i dati, il controllo degli accessi limita chi tiene la chiave.

### 20.4 Monitoraggio e registrazione: sapere sempre cosa sta facendo l'IA

Un **log** è un record di ciò che è successo: chi ha fatto cosa, quando, su quali dati. Il **monitoraggio** è guardare quei log, dal vivo o regolarmente, per individuare guai.

Perché conta per l'IA: un'automazione di IA agisce sui tuoi dati tutto il giorno. Senza un log, non puoi dire cosa ha toccato, cosa ha cambiato, o se è stata ingannata. Con un log, hai un record che puoi controllare e una traccia che un attaccante non può nascondere.

Rendi la registrazione utile:

- **Registra le azioni importanti** — quali dati l'IA ha letto, cosa ha scritto, cosa ha inviato, e qualsiasi richiesta ha rifiutato.
- **Imposta allarmi** così che i segnali importanti trovino un umano. Non far fissare uno schermo a qualcuno; fai sì che il sistema urli quando succede qualcosa di insolito.
- **Guarda davvero.** Come mostra la storia di curiosità, un log che nessuno legge non è sicurezza. Assegna qualcuno a rivedere, anche brevemente, con un programma regolare.
- **Tieni i log al sicuro** così che un intruso non possa cancellarli.

Il monitoraggio trasforma un sistema silenzioso in uno visibile. Non puoi proteggere ciò che non puoi vedere.

### 20.5 Piani di risposta agli incidenti: cosa fare se qualcosa va storto

Prima o poi qualcosa andrà storto. La domanda non è "se" ma "quando", e quanto sei pronto. Un **piano di risposta agli incidenti** è un piano scritto per la giornata storta, fatto in una giornata calma così non stai improvvisando nel panico.

Un piano semplice ha cinque passi:

1. **Rileva.** Come saprai che qualcosa non va? (Un allarme, una segnalazione del personale, un reclamo di un cliente.)
2. **Contieni.** Come fermi il danno adesso? (Spegni l'automazione, taglia la connessione, blocca l'account.)
3. **Valuta.** Cosa è stato esposto o danneggiato? Controlla i log.
4. **Correggi e riprendi.** Ripara la causa e ripristina il normale funzionamento sicuro.
5. **Segnala e impara.** Dillo alle persone che devono saperlo — e sappi chi sei legalmente obbligato a informare. (Le leggi sulla privacy come il GDPR hanno doveri di segnalazione; vedi [Capitolo 10](ch10-privacy-and-gdpr.md).) Poi scrivi cosa è successo e come prevenirlo la prossima volta.

Scrivi il piano su una pagina. Nomina chi fa cosa. Tieni pronti i contatti di emergenza. Esegui una breve esercitazione una volta all'anno così tutti conoscono la loro parte. Un piano provato trasforma una crisi in un evento gestibile.

### 20.6 Formazione del personale: il fattore umano è la prima difesa

La serratura più forte può essere aperta da una sola persona negligente. Il tuo personale è insieme il tuo rischio più grande e la tua migliore difesa. La formazione li trasforma dal punto debole alla prima linea.

Cosa insegnare, in termini semplici:

- **Riconosci i trucchi.** Gli attaccanti ingannano le persone con email false, richieste urgenti e telefonate "sono dell'IT, dammi la password". Insegna al personale a individuarli e a dubitarne.
- **Tratta i dati con cura.** Chi può vedere cosa, e perché. Non condividere mai dati dei clienti fuori dai canali approvati.
- **Segnala, non nascondere.** Rendi sicuro e atteso segnalare un errore o una richiesta strana. Un dipendente che segnala un'email sospetta presto salva l'azienda. Uno che la nasconde lascia crescere un piccolo problema.
- **Conosci i limiti dell'IA.** Il personale dovrebbe sapere cosa l'IA può e non può vedere, e non chiederle mai di fare qualcosa fuori dai suoi confini sicuri.
- **Igiene di password e login.** Password forti, autenticazione a due fattori, nessuna condivisione di login.

Mantieni la formazione breve, regolare e pratica — non una lezione una volta all'anno. Un promemoria mensile di cinque minuti e un canale di segnalazione chiaro fanno più di un lungo corso annuale che nessuno ricorda.

## Etica e responsabilità

La sicurezza è un dovere etico, non solo tecnico.

**Proteggi le persone di cui detieni i dati.** Clienti, dipendenti e partner ti hanno affidato le loro informazioni. Una violazione danneggia persone reali. Trattare quei dati in modo sicuro è una questione di onestà e cura.

**Segnala onestamente quando le cose vanno male.** Se devi avvisare clienti o regolatori, fallo tempestivamente e con verità. Insabbiare una violazione è peggio della violazione stessa, sia eticamente sia legalmente.

**Non usare la sicurezza come scusa per nascondere.** "Siamo sicuri" non dovrebbe mai significare "non potete verificare". Responsabilità e trasparenza stanno insieme.

**Bilancia sicurezza e usabilità.** Una sicurezza così pesante che nessuno può lavorare viene scavalcata, e una sicurezza scavalcata non è sicurezza affatto. Rendi il percorso sicuro quello facile.

**Forma con rispetto, non con colpa.** Quando qualcuno fa un errore, insegna, non punire. Una cultura della colpa nasconde gli errori; una cultura dell'apprendimento li fa emergere presto.

Proteggi i tuoi dati come vorresti che i tuoi fossero protetti.

## Errori da evitare

**Troppi accessi.** Dare all'IA o al personale più accesso del necessario. Usa il privilegio minimo.

**Nessun umano sull'invio.** Lasciare che l'IA agisca da sola su messaggi rivolti ai clienti. Tieni un controllo umano.

**Dare dati sensibili in pasto a strumenti non verificati.** Incollare dati dei clienti in uno strumento che non puoi giustificare. Sappi dove vanno i dati.

**Un log che nessuno legge.** Raccogliere registri e non guardare mai. Assegna qualcuno e imposta allarmi.

**Nessun piano per gli incidenti.** Improvvisare nella giornata storta. Scrivi il piano in una giornata calma.

**Condividere login.** Un account condiviso da molte persone distrugge la responsabilità. Dai a ognuno il proprio.

**Nessuna autenticazione a due fattori.** Lasciare gli account aperti a password rubate. Attiva la 2FA ovunque.

**Ignorare i cambi di personale.** Vecchi accessi che persistono dopo che qualcuno se ne va. Aggiorna gli accessi il giorno in cui i ruoli cambiano.

**Colpevolizzare invece di formare.** Punire gli errori così le persone li nascondono. Insegna e incoraggia la segnalazione.

**Dare per scontato che il fornitore sia sicuro.** Fidarsi senza chiedere. Chiedi ai fornitori di cifratura e accessi.

**La sicurezza come ripensamento.** Costruire l'automazione prima e pensare alla sicurezza dopo. Progetta la sicurezza dentro fin dall'inizio.

**Nessun kill switch.** Nessun modo per fermare l'automazione in fretta quando si comporta male. Costruisci l'interruttore di spegnimento.

## Esercizio pratico

### 20.8 Esercizio: scrivi il tuo piano di sicurezza per l'IA

Scrivi un piano di sicurezza di una pagina per un'automazione di IA che usi o prevedi di usare. Riempi ogni riga.

**1. L'automazione.** Nominala e quali dati tocca.

**2. Minimo accesso.** Elenca esattamente di quali dati ha bisogno. Taglia tutto il resto. Scrivi l'accesso che effettivamente concederai.

**3. Controllo umano.** Dov'è l'umano nel ciclo? Cosa può fare l'IA da sola, e cosa richiede l'approvazione di una persona?

**4. Ubicazione dei dati.** Dove vanno i dati? Elenca ogni sistema, soprattutto fuori dal tuo controllo. Nota quelli che non puoi giustificare e rimuovili.

**5. Cifratura.** I dati sono cifrati in transito e a riposo? Verifica con ogni fornitore e scrivi la risposta.

**6. Controllo degli accessi.** Chi può fare cosa? Elenca i ruoli. Nota dove attiverai l'autenticazione a due fattori.

**7. Registrazione.** Cosa registrerai? Chi guarderà, e quanto spesso? Cosa farà scattare un allarme?

**8. Kill switch.** Come la spegni istantaneamente? Scrivi i passi esatti.

**9. Piano per gli incidenti.** Scrivi i cinque passi — rileva, contiene, valuta, correggi, segnala — con i nomi di chi fa ciascuno. Nota ogni dovere legale di segnalazione (vedi [Capitolo 10](ch10-privacy-and-gdpr.md)).

**10. Formazione del personale.** Cosa insegnerai al team su questa automazione, e come segnaleranno un problema?

Mettilo su una pagina. Condividilo con le persone coinvolte. Tienilo dove puoi trovarlo nella giornata storta. Un piano scritto in una giornata calma vale dieci volte un piano inventi in una crisi.

## Checklist

### 20.9 Checklist: le 15 domande di sicurezza

Prima di lasciare che un'automazione di IA tocchi dati reali, rispondi a queste quindici domande. Ognuna deve essere un chiaro "sì".

- [ ] **1. Minimo accesso:** L'automazione ha solo i dati di cui ha davvero bisogno, e niente di più?
- [ ] **2. Umano sull'invio:** C'è un umano che controlla tutto ciò che raggiunge un cliente?
- [ ] **3. Ubicazione dei dati:** Conosco ogni sistema che i dati toccano, incluso fuori dal mio controllo?
- [ ] **4. Strumenti verificati:** Ho rifiutato di dare in pasto dati sensibili a qualsiasi strumento che non posso giustificare?
- [ ] **5. Cifrato in transito:** I dati sono cifrati mentre si muovono tra sistemi?
- [ ] **6. Cifrato a riposo:** I dati sono cifrati mentre sono archiviati?
- [ ] **7. Login individuali:** Ogni persona ha il proprio login, senza condivisioni?
- [ ] **8. Autenticazione a due fattori:** La 2FA è attivata per gli account importanti?
- [ ] **9. Compiti separati:** Configurazione, approvazione e revisione dei log sono divisi tra persone?
- [ ] **10. Revisione degli accessi:** Aggiorno gli accessi il giorno in cui il personale entra, si sposta o esce?
- [ ] **11. Registrazione:** Sto registrando ciò che l'IA legge, scrive, invia e rifiuta?
- [ ] **12. Log sorvegliati:** Qualcuno sta davvero rivedendo i log, con allarmi per i segnali importanti?
- [ ] **13. Kill switch:** Posso spegnere l'automazione istantaneamente, e so come?
- [ ] **14. Piano per gli incidenti:** Ho un piano scritto e nominato per rilevare, contenere, valutare, correggere e segnalare?
- [ ] **15. Personale formato:** Il team è stato addestrato a individuare i trucchi e segnalare i problemi in sicurezza?

Se una risposta è "no", l'automazione non è pronta. Correggila prima di andare in produzione. La sicurezza non è un prodotto che compri una volta; è quindici domande a cui continui a rispondere sì.

## Punti chiave

- La sicurezza by design significa costruire la sicurezza dentro fin dall'inizio — minimo accesso, un umano sull'invio e un kill switch — così il caso peggiore resta piccolo.
- Un log che nessuno legge non è sicurezza: raccogli registri, imposta allarmi e assegna qualcuno a guardare davvero.
- La cifratura nasconde i dati agli estranei (in transito e a riposo), mentre il controllo degli accessi limita chi tiene la chiave — ti servono entrambi che lavorano insieme.
- Scrivi il tuo piano di risposta agli incidenti in una giornata calma: rileva, contiene, valuta, correggi, segnala, impara — con nomi attaccati a ogni passo.
- Il fattore umano è la prima difesa: forma il personale a individuare i trucchi e segnalare in sicurezza, e rendi il percorso sicuro quello facile.
