# Capitolo 28 — Risorse umane e persone

## In parole semplici

Le risorse umane sono il punto in cui un'azienda incontra le sue persone. Assumere, formare, aiutare i nuovi dipendenti a inserirsi, e capire perché le persone se ne vanno — queste cose plasmano tutta l'azienda. Sono anche piene di lavoro ripetitivo: leggere centinaia di CV, rispondere alle stesse domande di inserimento, ordinare la formazione per ruolo, e setacciare vecchi archivi per scoprire perché il personale si dimette. L'AI può prendersi la parte ripetitiva di ogni lavoro e lasciare la parte umana — giudizio, equità e attenzione — dove deve stare.

Pensa alle risorse umane come a un imbuto e a un giardino allo stesso tempo. L'imbuto è l'assunzione: molte persone entrano dall'alto, e tu le riduci a pochi profili adatti. Il giardino sono tutti quelli che hai già: li innaffi con la formazione, osservi i segnali di problemi, e cerchi di farli crescere. L'AI aiuta a entrambe le estremità. Nell'imbuto, smista e fa selezioni più in fretta di quanto una persona riesca a leggere. Nel giardino, individua schemi in mille piccoli segnali che nessun manager potrebbe tenere in testa.

Questo capitolo copre quattro attività: la selezione di CV e candidature, l'inserimento dei nuovi assunti, la formazione personalizzata e l'analisi del ricambio del personale. Ognuna è un posto dove una piccola azienda può risparmiare tempo e prendere decisioni migliori sulle persone.

Un'idea onesta prima di cominciare: le persone non sono fatture. Un numero sbagliato su una fattura costa denaro; una decisione sbagliata su una persona costa una vita, una carriera e la tua reputazione. Quindi l'AI nelle risorse umane è un *aiutante*, mai il *giudice*. Legge, smista, suggerisce e segnala. Una persona decide ancora chi ottiene il lavoro, chi ottiene la promozione, e perché qualcuno viene licenziato. E in Europa, l'assunzione e la gestione dei lavoratori sono considerati usi ad alto rischio dell'AI, con veri obblighi di legge. Il trattamento completo dell'AI Act europeo si trova nel [Capitolo 5 — Regole e responsabilità legale](ch05-rules-and-legal-responsibility.md); questo capitolo ti mostra cosa automatizzare e come, e dove la legge traccia una linea. Il metodo per giudicare se tutto questo conviene si trova nel [Capitolo 16 — Obiettivi, costi e ritorno sull'investimento](ch16-goals-costs-and-return-on-investment.md).

## Un po' di storia

**Anni '80–'90: la banca dati del personale.** Il primo grande cambiamento nel lavoro delle risorse umane fu la scheda del personale computerizzata. Invece di cartelline di carta in un armadio, i registri dei dipendenti vivevano in una banca dati. Stipendi, presenze e dettagli personali diventarono consultabili. Fu la prima volta che il software toccò il cuore delle risorse umane, e fissò il modello: conserva i dati, lascia l'umano al comando delle decisioni.

**Anni '90–2000: il sistema di tracciamento delle candidature.** Con il passaggio delle candidature online, le aziende adottarono il sistema di tracciamento delle candidature, o ATS — un software che raccoglie le candidature, le archivia e permette ai selezionatori di cercarle e ordinarle. Un selezionatore poteva ora vedere ogni candidato per un lavoro in un unico posto e filtrare per parole chiave. Questo portò ordine nel diluvio di candidature online, ma il filtro era semplice: abbinava parole, non persone.

**Anni 2000: l'e-learning e il sistema di gestione dell'apprendimento.** La formazione si spostò dall'aula allo schermo. Il sistema di gestione dell'apprendimento, o LMS, erogava corsi online e tracciava chi completava cosa. Questo rese la formazione scalabile, ma le prime versioni erano taglia unica: tutti guardavano lo stesso video, indipendentemente da ciò che già sapevano.

**Anni 2010: la people analytics.** Le aziende cominciarono ad analizzare i dati delle risorse umane come analizzavano quelli di vendita. Guardavano quali assunti restavano, quali team performavano, e quali segnali prevedevano che qualcuno se ne sarebbe andato. La people analytics trasformò le risorse umane da una funzione di carte a una funzione di dati. Ma servivano grandi insiemi di dati e analisti esperti, così per lo più solo le grandi aziende potevano farlo.

**Anni 2020: i grandi modelli linguistici leggono e scrivono delle persone.** I grandi modelli linguistici — AI addestrata su enormi quantità di testo — ora possono leggere un CV e una descrizione di lavoro e giudicare quanto corrispondono, redigere un piano di formazione personalizzato, e rispondere alla domanda HR di un dipendente con parole semplici. Questo è il passo più recente: un'AI che legge le parole che le persone scrivono e ragiona su di esse. È potente, e proprio perché è potente, è l'area dove la legge è più severa.

Il percorso: dalle cartelline di carta, alle banche dati consultabili, ai filtri per parole chiave, all'analisi, a un'AI che legge e ragiona sulle persone. Ogni passo ha tolto più lavoro ripetitivo dalle mani umane — e ogni passo ha alzato la posta per l'equità, perché le decisioni riguardano vite umane.

## Curiosità

### 28.5 La legge dice: avvisa i tuoi lavoratori prima che l'AI tocchi i loro posti di lavoro

Ecco un fatto che ogni datore di lavoro europeo dovrebbe sapere prima di accendere qualsiasi strumento HR che incide sul personale.

L'AI Act europeo ha una regola specifica sui lavoratori. In parole semplici: se usi un sistema AI ad alto rischio sul luogo di lavoro — uno che incide sulle decisioni sui tuoi dipendenti — devi informare i tuoi lavoratori e i loro rappresentanti *prima* di iniziare a usarlo. La legge lo afferma direttamente nell'articolo 26(7): "Prima di mettere in servizio o di utilizzare un sistema di IA ad alto rischio sul luogo di lavoro, i soggetti che distribuiscono che sono datori di lavoro informano i rappresentanti dei lavoratori e i lavoratori interessati che saranno soggetti all'uso del sistema di IA ad alto rischio."

Due cose contano qui. Prima, non è facoltativo. È un obbligo di legge, non una cortesia. Seconda, è *prima*, non dopo. Non puoi distribuire uno strumento di selezione AI e dirlo alla gente un mese dopo. Li avvisi prima.

Perché esiste questa regola? Perché le persone hanno diritto di sapere quando una macchina sta plasmando la loro vita lavorativa — che uno strumento stia leggendo la loro candidatura, classificando la loro performance, o decidendo i loro compiti. Il segretezza sull'AI al lavoro erode la fiducia e può nascondere ingiustizie. Dire le persone apertamente è il minimo che un datore di lavoro equo fa.

Un avvertimento collegato: lo stesso Act *vieta* il riconoscimento delle emozioni sul luogo di lavoro — usare l'AI per leggere i sentimenti di un lavoratore dal suo viso o dalla sua voce è proibito, tranne che per ragioni mediche o di sicurezza. Uno strumento che "rileva" se un operatore di call center è contento o stressato per punteggiarlo è decisamente vietato. L'elenco completo delle pratiche vietate e le date scaglionate sono nel [Capitolo 5](ch05-rules-and-legal-responsibility.md). Il punto qui è semplice: sii trasparente sull'AI che usi sulle persone, e non leggere mai di nascosto le loro emozioni.

## Un esempio di business reale

**Una media azienda che ha automatizzato assunzioni e inserimento — uno scenario illustrativo.**

Questo esempio è illustrativo. È un composito realistico, non un risultato aziendale riportato, costruito per mostrare come le quattro attività HR si incastrano e dove stanno l'umano e la legge.

Immagina un'azienda di 400 persone che assume circa 80 dipendenti l'anno, per lo più per pochi ruoli ricorrenti: vendite, supporto e back-office. Ogni posto vacante porta da 200 a 400 candidature. I due addetti alle risorse umane erano sommersi: leggere i CV prendeva giorni, le domande di inserimento si ripetevano tutto il giorno, e nessuno sapeva perché la gente se ne andava dopo un anno.

Hanno cambiato tre cose.

Primo, **la selezione dei CV con un controllo umano.** Hanno usato uno strumento AI per leggere ogni candidatura rispetto alla descrizione del lavoro e produrre una rosa ristretta con una breve motivazione per ogni corrispondenza. Gli addetti HR non hanno lasciato che lo strumento scartasse nessuno. Hanno rivisto la rosa, e ogni settimana campionavano anche un gruppo di candidature scartate per verificare che lo strumento non stesse ingiustamente scartando buoni candidati. Lo strumento ha ridotto i tempi di selezione da giorni a ore. La decisione è rimasta umana.

Secondo, **un assistente di inserimento.** Hanno costruito un chatbot addestrato sul loro manuale, sulle loro politiche e sulle loro FAQ. I nuovi assunti potevano chiedere: "Come faccio a richiedere un permesso?" o "Qual è la politica sulle spese?" e ottenere una risposta istantanea, di giorno o di notte. I due addetti HR hanno smesso di rispondere alle stesse dieci domande ogni giorno e hanno speso il tempo per i nuovi assunti che avevano davvero bisogno di un umano — i nervosi, quelli con situazioni insolite.

Terzo, **una revisione del ricambio.** Hanno raccolto due anni di registri HR in una semplice analisi: chi se n'è andato, da quale ruolo, dopo quanto tempo, e cosa diceva il loro ultimo questionario di coinvolgimento. Lo schema era chiaro — il personale di supporto se ne andava più spesso dopo 12-18 mesi, e i loro commenti di uscita si raggruppavano attorno alla retribuzione e alla mancanza di un percorso chiaro di crescita. Quell'unica costatazione ha dato loro una soluzione concreta: una revisione degli stipendi e un percorso di promozione definito per il supporto. Non serviva un'AI sofisticata per agire; serviva far emergere lo schema, cosa che l'analisi ha fatto.

Nota la forma. L'AI ha fatto la lettura, il rispondere e lo smistamento. Gli umani hanno preso le decisioni, l'attenzione e l'azione. E perché lo strumento di selezione incideva sull'assunzione — un uso ad alto rischio — l'azienda ha informato i suoi lavoratori e i loro rappresentanti prima di accenderlo, come la legge richiede. Questo è il modello da copiare.

## Come si fa

### 28.1 Selezione di CV e curricula

Selezionare CV (curricula) è il classico pozzo di tempo delle risorse umane. Un singolo posto vacante può portare centinaia di candidature, e leggerne una prende minuti. L'AI può leggerli tutti e produrre una rosa ristretta, così un umano rivede un mucchio gestibile invece di una montagna.

**Cosa fa l'AI.** Legge ogni CV e la descrizione del lavoro, poi ordina o smista le candidature per quanto corrispondono. Guarda competenze, esperienza e parole chiave. Gli strumenti moderni leggono il significato, non solo le parole, così "ho gestito un team di cinque" può corrispondere a "esperienza di leadership".

**L'avvertimento sull'alto rischio.** Nell'UE, usare l'AI per selezionare candidature di lavoro o filtrare candidati è un uso **ad alto rischio** secondo l'AI Act, perché incide sul sostentamento di una persona. Questo porta veri obblighi: trasparenza, supervisione umana e attenzione contro i pregiudizi. Leggi il [Capitolo 5](ch05-rules-and-legal-responsibility.md) prima di distribuire qualsiasi strumento di selezione. Non trattare un selettore di CV come "solo un software".

**Il pregiudizio è il pericolo centrale.** Un'AI addestrata sulle assunzioni passate impara gli schemi delle assunzioni passate — inclusa ogni ingiustizia passata. Se la tua azienda storicamente ha assunto soprattutto uomini per un ruolo, lo strumento potrebbe imparare a penalizzare le donne. Se ha imparato a favorire un'università, potrebbe scartare candidati ugualmente bravi di altrove. Non è ipotetico; è successo in sistemi reali. Difenditi: rivedi la rosa e il mucchio degli scartati per cercare schemi, testa lo strumento su esempi diversi, e non lasciarlo mai scartare in automatico.

**Mantieni la decisione umana.** Usa l'AI per fare selezioni e per spiegare *perché* ha abbinato. Una persona prende la decisione. Una rosa con motivazioni è molto meglio di una semplice classifica, perché permette al revisore di vedere la logica dello strumento e cogliere un abbinamento sbagliato.

**Informa candidati e lavoratori.** Sii trasparente sul fatto che l'AI assiste nella selezione, e informa i tuoi lavoratori e i loro rappresentanti prima di accenderlo, come la legge richiede. I dati dei candidati sono dati personali; trattali secondo le regole sulla privacy nel [Capitolo 10 — Privacy e GDPR](ch10-privacy-and-gdpr.md).

### 28.2 Inserimento

L'inserimento è la prima vera esperienza che un nuovo assunto ha della tua azienda. Un buon inserimento fa sentire una persona accolta, chiara e pronta. Uno cattivo la lascia confusa e ansiosa. L'AI aiuta rispondendo all'istante alle infinite domande di routine, così la parte umana dell'inserimento — l'accoglienza, le presentazioni, la rassicurazione — riceve più tempo, non meno.

**L'assistente di inserimento.** Un chatbot addestrato sul tuo manuale, sulle tue politiche e sulle domande comuni può rispondere a un nuovo assunto alle 9 di sera della vigilia del primo giorno: "A che ora devo arrivare?", "Cosa porto?", "Come funziona lo stipendio?". Questo elimina le piccole confusioni che rendono stressante il primo giorno.

**Una lista di controllo guidata.** L'AI può generare un piano di inserimento personalizzato per ogni ruolo: gli account da aprire, i sistemi a cui accedere, le persone da incontrare, la formazione da finire. Invece di una lista generica unica, ogni nuovo assunto riceve un percorso adatto al suo lavoro. Lo strumento traccia l'avanzamento e sollecita ciò che manca.

**Redigi i materiali di benvenuto.** L'AI può redigere l'email di benvenuto, la presentazione al team e il programma della prima settimana, così il manager parte da una buona bozza invece che da una pagina bianca. Il manager la personalizza. Il tocco umano resta, ma il lavoro noioso si riduce.

**Cosa l'AI non può sostituire.** Il caffè di benvenuto, il mentore, il manager che si fa vivo al terzo giorno. L'inserimento è emotivo quanto pratico. Usa l'AI per le informazioni e la lista di controllo; tieni una persona per l'accoglienza. Un nuovo assunto che parla solo con un bot si sente un numero.

**Misura i primi 90 giorni.** Traccia quanto tempo impiega un nuovo assunto a diventare produttivo e come si sente a 30, 60 e 90 giorni. Se l'inserimento con l'AI funziona, il tempo di rodaggio cala e la soddisfazione iniziale sale. Se non funziona, il bot non è la risposta — lo è il processo.

### 28.3 Formazione personalizzata

La vecchia formazione era taglia unica: tutti guardavano lo stesso corso. La formazione personalizzata usa l'AI per adattare l'apprendimento a ciò che ogni persona già sa e a ciò di cui il suo ruolo ha bisogno. È la differenza tra una lezione frontale fissa e un tutor che sa dove sei bloccato.

**Adatta alla persona.** L'AI può dare un breve quiz iniziale, vedere cosa una persona già sa, e saltare ciò che ha già padroneggiato. Dedica tempo solo alle lacune. Questo rispetta il tempo di chi impara e rende la formazione più veloce e più pertinente.

**Adatta al ruolo.** Un assunto nel supporto ha bisogno di una formazione diversa da un assunto nelle vendite, anche nella stessa azienda. L'AI può assemblare un percorso di apprendimento dalla tua biblioteca di contenuti che si adatta al ruolo, al livello e al ritmo della persona.

**Redigi i contenuti.** L'AI può trasformare i tuoi documenti esistenti — una politica, una guida prodotto, una riunione registrata — in un breve modulo di formazione con domande per verificare la comprensione. Questo trasforma conoscenza che già esiste in formazione che la gente può davvero usare, senza che uno specialista costruisca ogni corso.

**Rispondi alle domande mentre si impara.** Chi impara può chiedere all'AI un punto difficile e ottenere una spiegazione con parole semplici, come un tutor. È qui che i grandi modelli linguistici eccellono: spiegano, riformulano e fanno esempi su richiesta.

**Tienilo onesto e verificato.** La formazione generata dall'AI deve essere rivista da un esperto umano prima di essere diffusa. Un modulo di formazione sicuro ma sbagliato diffonde errori in fretta. Verifica i fatti, verifica il tono, e tieni una persona disponibile per le domande che contano. La formazione plasma come le persone lavorano; deve essere giusta.

### 28.4 Analisi del ricambio del personale

Il ricambio significa persone che lasciano la tua azienda. Un ricambio alto è costoso — perdi competenze, riassumi, ri-formi. L'analisi del ricambio usa l'AI per guardare i tuoi dati HR e scoprire *perché* le persone se ne vanno, così puoi risolvere la causa invece di indovinare.

**Cosa guarda l'AI.** Combina i registri: chi se n'è andato, da quale ruolo, dopo quanto tempo, la sua retribuzione, il suo manager, l'ultimo questionario di coinvolgimento, se è stato promosso, quanto spesso era in ritardo. Da solo, ogni fatto è piccolo. Insieme, formano uno schema.

**Lo schema è il valore.** L'AI può far emergere qualcosa come: "Le persone nel ruolo X che non sono state promosse in 18 mesi se ne vanno a tre volte il tasso normale." Questa è una costatazione su cui puoi agire. Nessun manager potrebbe tenere mille registri in testa e vederlo; l'analisi sì.

**Prevedi il rischio, non la persona.** Alcuni strumenti segnalano quali dipendenti attuali mostrano schemi simili a quelli che se ne sono andati. Usa questo per *iniziare una conversazione* — un controllo, un piano di sviluppo — mai per segnare in silenzio qualcuno come "probabile che se ne vada" e trattarlo diversamente. Una previsione è una ragione per prendersi cura, non una ragione per agire contro qualcuno.

**Osserva i piccoli segnali.** Questionari di coinvolgimento, un calo nella performance, una promozione saltata, un cambio di manager — sono questi i piccoli segnali che spesso precedono una dimissione. L'AI è brava a notarli su molte persone insieme. Il compito umano è rispondere con una conversazione vera.

**La privacy prima di tutto.** L'analisi del ricambio usa dati personali sensibili. Trattala secondo le regole sulla privacy nel [Capitolo 10](ch10-privacy-and-gdpr.md), tienila al sicuro, e usala per migliorare le condizioni per il gruppo, non per spiare i singoli. L'obiettivo è un posto di lavoro migliore, non un sistema di sorveglianza.

## Etica e responsabilità

Le risorse umane sono il posto più sensibile dove usare l'AI, perché il risultato è una decisione su una vita umana. L'asticella etica qui è più alta che in qualsiasi altro punto di questo libro.

**Una persona decide delle persone.** L'AI legge, smista e suggerisce. Un umano prende ogni decisione di assunzione, promozione e licenziamento. Non lasciare mai che uno strumento scarti in automatico un candidato o licenzi in automatico un lavoratore. L'umano deve possedere il risultato e poterlo spiegare.

**Combatti attivamente il pregiudizio.** L'AI delle risorse umane eredita i pregiudizi nei suoi dati di addestramento. Rivedi i risultati tra i gruppi — genere, età, provenienza — e cerca schemi ingiusti. Testa lo strumento prima di fidartene, e continua a testarlo dopo. L'equità non è un'impostazione che attivi una volta; è un'abitudine che verifichi.

**Sii trasparente con i lavoratori.** Informa i tuoi lavoratori e i loro rappresentanti prima che qualsiasi AI ad alto rischio tocchi i loro posti di lavoro, come la legge richiede. Il segreto sull'AI al lavoro rompe la fiducia e nasconde le ingiustizie. La trasparenza è sia la legge sia la cosa giusta.

**Non leggere mai le emozioni sul lavoro.** Il riconoscimento delle emozioni sul luogo di lavoro è vietato dall'AI Act europeo. Non comprare né usare uno strumento che punteggia il personale leggendo i loro volti o le loro voci. È vietato, ed è sbagliato.

**Proteggi i dati personali.** I dati delle risorse umane sono tra i più sensibili che un'azienda possiede — retribuzione, note sanitarie, performance, circostanze personali. Custodiscili, limita chi li vede, e segui il [Capitolo 10](ch10-privacy-and-gdpr.md). Non immettere dati dei dipendenti in strumenti AI pubblici senza verificare le implicazioni di sicurezza (vedi [Capitolo 6 — Cybersecurity nell'era dell'AI](ch06-cybersecurity-in-the-ai-era.md)).

**Usa i dati per aiutare, non per punire.** Le previsioni sul ricambio e i dati di coinvolgimento dovrebbero renderti un datore di lavoro migliore — stipendi migliori, percorsi di crescita migliori, condizioni migliori. Non dovrebbero mai diventare uno strumento per sorvegliare, classificare o punire i singoli. Misura il luogo di lavoro, non la persona come bersaglio.

**Mantieni l'umano nell'accoglienza.** Nell'inserimento e nell'HR quotidiano, l'AI gestisce le informazioni; gli umani gestiscono l'attenzione. Un'azienda che esternalizza tutto il contatto umano a un bot perde la fiducia che fa funzionare un luogo di lavoro.

## Errori da evitare

**Lasciare che l'AI scarti candidati.** Il peggior errore HR. Uno strumento che scarta in automatico nasconde pregiudizi e uccide buone assunzioni. Mantieni sempre una decisione umana.

**Ignorare il pregiudizio.** Non verificare se lo strumento tratta i gruppi in modo ingiusto. Il pregiudizio di assunzione passato diventa pregiudizio di assunzione futuro se non guardi. Testa e rivedi.

**Accendere uno strumento ad alto rischio di nascosto.** Non informare i lavoratori e i loro rappresentanti prima di usare un'AI che li riguarda. Questo rompe la legge e la fiducia.

**Comprare uno strumento di riconoscimento delle emozioni.** È vietato sul luogo di lavoro. Un'offerta di un venditore per il "rilevamento dell'umore" sul personale è una trappola.

**Trattare una previsione come un verdetto.** Agire contro un dipendente perché un modello lo ha segnalato come "probabile che se ne vada". Una previsione è una ragione per parlare, non per punire.

**Sorvegliare il personale.** Usare i dati HR per osservare e classificare i singoli invece di migliorare le condizioni per il gruppo. Questo avvelena la fiducia.

**Un inserimento solo bot.** Un nuovo assunto che non parla mai con un umano si sente un numero. Mantieni l'accoglienza umana.

**Formazione AI non revisionata.** Pubblicare formazione generata dall'AI che è sicura ma sbagliata. Un esperto umano deve controllarla.

**Automatizzare un cattivo processo HR.** Se la tua assunzione o il tuo inserimento sono rotti, l'AI crea un processo rotto più veloce. Prima sistema il processo.

**Far trapelare dati dei dipendenti.** Mettere dati HR sensibili in strumenti AI non sicuri. Prima verifica sicurezza e privacy.

**Nessuna linea di base.** Non misurare il tempo di assunzione, il tempo di rodaggio o il ricambio prima, così non puoi dimostrare il miglioramento. Misura prima (vedi [Capitolo 22 — Misurare i risultati e il ROI](ch22-measuring-results-and-roi.md)).

**Dimenticare che la legge è il pavimento.** Conformarsi all'AI Act non rende equo uno strumento di assunzione. L'etica sta sopra la conformità, e la responsabilità è tua (vedi [Capitolo 4 — Etica dell'AI: fare la cosa giusta](ch04-ethical-ai-doing-the-right-thing.md)).

## Esercizio pratico

### 28.7 Esercizio: pianifica un'automazione HR in modo responsabile

Scegli un'attività HR e pianifica la sua assistenza con l'AI dall'inizio alla fine, con l'umano e la legge integrati.

**Passo 1 — Scegli l'attività.** Scegline una: selezione CV, inserimento, formazione o analisi del ricambio. Fanne una, non tutte.

**Passo 2 — Definisci l'obiettivo e la metrica.** Tempo di assunzione più veloce? Rodaggio del nuovo assunto più rapido? Meno ricambio? Scegli un numero da misurare.

**Passo 3 — Misura la linea di base.** Qual è quel numero adesso? Quanto tempo prende la selezione? Quanto tempo per il rodaggio? Qual è il tuo tasso di ricambio? Scrivilo.

**Passo 4 — Classifica il rischio.** È un uso ad alto rischio secondo l'AI Act? La selezione e la gestione dei lavoratori lo sono. Se sì, hai obblighi di legge: trasparenza, supervisione umana, attenzione al pregiudizio. Annotali (vedi [Capitolo 5](ch05-rules-and-legal-responsibility.md)).

**Passo 5 — Marca ogni passo.** Per ogni passo, marcalo: **l'AI lo fa** (leggere, smistare, redigere, far emergere), **l'umano lo revisiona** (controllare la rosa, rivedere la formazione), oppure **l'umano lo decide** (l'assunzione, la promozione, la soluzione). Ogni decisione su una persona deve essere umana.

**Passo 6 — Costruisci il controllo del pregiudizio.** Decidi come verificherai gli schemi ingiusti tra i gruppi, e quanto spesso rivedrai il mucchio degli scartati e i risultati.

**Passo 7 — Pianifica l'avviso ai lavoratori.** Scrivi come e quando informerai i lavoratori e i loro rappresentanti prima di accendere lo strumento, come la legge richiede.

**Passo 8 — Lancia in piccolo e misura.** Prima fallo girare su un ruolo o un team. Confronta la metrica con la linea di base. Scala solo ciò che dimostra di aiutare e di trattare le persone equamente.

Fai bene un'attività. Il controllo del pregiudizio e l'avviso ai lavoratori che costruisci ai passi 6 e 7 sono preziosi di per sé — ti costringono a vedere i tuoi schemi di assunzione, utile anche al di là dello strumento.

## Lista di controllo

### 28.8 Lista di controllo per risorse umane e persone

Prima di usare l'AI sulle persone, verifica queste cose.

- [ ] **Hai misurato la linea di base** — tempo di assunzione, tempo di rodaggio, tasso di ricambio.
- [ ] **Un umano prende ogni decisione su una persona** — nessun scarto automatico, nessun licenziamento automatico.
- [ ] **Hai classificato il rischio** — la selezione e la gestione dei lavoratori sono ad alto rischio secondo l'AI Act.
- [ ] **Hai avvisato i lavoratori e i loro rappresentanti prima di accendere** qualsiasi AI ad alto rischio che li riguarda (art. 26(7)).
- [ ] **Testi il pregiudizio** tra genere, età e provenienza, e rivedi il mucchio degli scartati.
- [ ] **Non usi mai il riconoscimento delle emozioni** sui lavoratori — è vietato.
- [ ] **Lo strumento spiega le sue corrispondenze** così un revisore può vedere la logica.
- [ ] **L'inserimento mantiene un'accoglienza umana** — il bot risponde, una persona accoglie.
- [ ] **La formazione generata dall'AI è revisionata da un esperto umano** prima di essere diffusa.
- [ ] **Le previsioni sul ricambio iniziano una conversazione**, non una punizione.
- [ ] **I dati HR sono tenuti al sicuro** e seguono le regole sulla privacy (vedi [Capitolo 10](ch10-privacy-and-gdpr.md)).
- [ ] **Usi i dati per migliorare le condizioni per il gruppo**, non per sorvegliare i singoli.
- [ ] **Sistemi il processo HR prima di automatizzarlo.**
- [ ] **Tratti la conformità come il pavimento** e la tua equità come lo standard sopra di essa.

Se una casella è vuota, una persona potrebbe sentirlo — e la legge potrebbe raggiungerla. Riempi ogni casella prima di lasciare che l'AI si avvicini alle tue persone.

## Punti chiave

- L'AI nelle risorse umane prende il lavoro ripetitivo — leggere CV, rispondere alle domande di inserimento, ordinare la formazione, far emergere gli schemi del ricambio — e lascia il decidere, l'attenzione e l'agire agli umani.
- L'assunzione e la gestione dei lavoratori sono usi ad alto rischio secondo l'AI Act europeo: una persona deve decidere, devi difenderti dal pregiudizio, e devi informare i lavoratori e i loro rappresentanti prima di accendere qualsiasi AI ad alto rischio che li riguarda.
- Il riconoscimento delle emozioni sul luogo di lavoro è vietato; non comprare né usare uno strumento che punteggia il personale leggendo i loro sentimenti.
- Usa i dati HR per rendere il luogo di lavoro migliore per il gruppo, mai per sorvegliare o punire i singoli, e mantieni l'accoglienza umana nell'inserimento.
- Misura la linea di base, mantieni un umano in ogni decisione sulle persone, e tratta la legge come il pavimento e l'equità come lo standard sopra di essa.

<!-- BEGIN agentbridge-examples -->

## Provalo con AgentBridge

Ecco come appare lo stesso lavoro con AgentBridge. Ogni riquadro mostra il risultato finito e l'unica riga che digiti per ottenerlo.

### Un semplice manuale del personale

![Un manuale del personale amichevole, pronto da condividere](../../assets/examples/employee-handbook.png)
*Un manuale del personale amichevole, pronto da condividere*

**Cosa chiedi:** `Scrivi un breve manuale del dipendente che copra orario di lavoro, ferie, regole sul lavoro da remoto e a chi chiedere aiuto.`

L'agente scrive un manuale chiaro e amichevole con parole semplici, con ogni argomento su una pagina a sé. Aggiornalo quando vuoi chiedendo — 'aggiungi una riga sulla nuova regola del parcheggio'.

*Suggerimento: Tienilo nella tua area documenti così l'agente potrà rispondere alle domande attingendovi più tardi.*

---

### Un foglio presenze settimanale

![Un foglio presenze settimanale con totali per persona](../../assets/examples/timesheet.png)
*Un foglio presenze settimanale con totali per persona*

**Cosa chiedi:** `Crea un foglio presenze settimanale con persone, progetti, ore al giorno e un totale per persona.`

L'agente costruisce la griglia del foglio presenze con colonne giornaliere e totali automatici. Compilalo o allega le tue ore approssimative e lascia che le ordini lui.

*Suggerimento: Moltiplica le ore per ciascuna tariffa e hai anche una scheda di fatturazione — devi solo chiedere.*

---

### Forma il tuo team in fretta

![Una diapositiva di formazione passo per passo](../../assets/examples/training-deck.png)
*Una diapositiva di formazione passo per passo*

**Cosa chiedi:** `Fai una presentazione di formazione su come gestire un rimborso a un cliente, passo per passo.`

L'agente trasforma il processo in diapositive chiare, un passo ciascuna, facili da seguire. Usalo per l'inserimento e i ripassi.

*Suggerimento: Aggiungi una diapositiva finale con 'a chi chiedere' così le persone sanno dove trovare aiuto.*

<!-- END agentbridge-examples -->
