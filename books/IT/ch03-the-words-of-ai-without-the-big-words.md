# Capitolo 3 — Le parole dell'IA, senza le parole grosse

## In parole semplici

La maggior parte delle cattive decisioni sull'IA non dipende da una tecnologia scadente. Dipende da parole che nessuno si è fermato a definire.

Un fornitore dice: "la nostra piattaforma di IA si integra con i vostri sistemi tramite un'API low-code e usa un grande modello linguistico". Tutti annuiscono. Nessuno chiede cosa significhi davvero. Sei mesi dopo il progetto è fuori budget, i dati sono finiti da qualche parte inaspettata, e nessuno sa dire chi possiede cosa.

Le parole sono l'interfaccia. Se il tuo team non condivide lo stesso significato per "modello", "addestramento" e "integrazione", non puoi prendere buone decisioni su nessuna di esse. Non puoi confrontare due fornitori. Non puoi scrivere un contratto. Non puoi accorgerti quando qualcosa sta andando storto.

Questo capitolo è un glossario operativo, non un dizionario. Ogni parola riceve un significato semplice, un'analogia quotidiana e la domanda che dovresti fare quando la senti.

Una regola attraversa tutto. **Una spiegazione vera contiene sempre un verbo e un oggetto.** Non "è alimentato dall'IA", ma "legge le tue fatture e mette il totale nel tuo file contabile". Se qualcuno non riesce a darti un verbo e un oggetto, non ti ha detto niente.

### 3.1 Dati, informazione, conoscenza

Tre parole che le persone usano come se fossero la stessa cosa. Sono tre passi diversi, e la differenza conta quando pianifichi.

I **dati** sono fatti grezzi senza significato attaccato. Una colonna di numeri. Una cartella di PDF. Un elenco di date. I dati da soli non ti dicono nulla. Il numero 47 è un dato.

L'**informazione** è un dato con un contesto. "La fattura 47 era di 1.200 € ed è stata pagata in ritardo." Ora il numero significa qualcosa. L'informazione è un dato collocato da qualche parte.

La **conoscenza** è un'informazione più la comprensione di cosa farne. "Quando questo cliente paga in ritardo, di solito è perché il suo cliente paga in ritardo, quindi lo sollecitiamo con garbo e alla fine paga sempre." Questa è conoscenza. Vive nella testa di una persona, e ci sono voluti anni per costruirla.

Pensa a un archivio metallico. I dati sono il foglio. L'informazione è il foglio in una cartella etichettata. La conoscenza è sapere quali cartelle contano il lunedì mattina e quali possono aspettare fino a marzo.

**Perché ti riguarda.** L'IA lavora sui dati. Non acquisisce automaticamente la tua conoscenza. Puoi dare a un sistema diecimila fatture e imparerà degli schemi al loro interno. Non imparerà perché il tuo cliente più grande paga sempre in ritardo di proposito, perché quella è una conoscenza tenuta da una sola persona che non l'ha mai scritta.

Prima di ogni progetto IA, chiedi: **quanto di ciò che fa funzionare questo compito è scritto come dato, e quanto vive nella testa di qualcuno?** Il divario tra questi due numeri è la dimensione del tuo vero problema. Colmarlo è di solito più difficile, e più prezioso, della parte di IA.

**Chiedi al fornitore:** "Di quali dati avete bisogno da noi, in che forma, e di quanti?"

### 3.2 Algoritmo, modello, addestramento

**Algoritmo.** Una ricetta. Una serie ordinata e chiara di passi che risolve un problema. Fare il caffè è un algoritmo. La divisione in colonna è un algoritmo. Un algoritmo non ha bisogno di un computer; gli servono solo dei passi. La parola deriva dal nome del matematico del IX secolo al-Khwarizmi, il cui lavoro sul calcolo passo per passo fu tradotto in latino e alla fine ci diede la parola.

**Modello.** Nel linguaggio quotidiano sull'IA, un modello è ciò che ottieni alla fine dell'addestramento: un insieme di impostazioni imparate che puoi usare per rispondere a nuovi casi. Pensalo come un dipendente formato. Non devi riinsegnargli tutto ogni mattina. La conoscenza è dentro di lui.

La parola è usata in due modi, e mescolarli crea confusione. Nel senso più antico, un modello è una descrizione scritta di come funziona qualcosa, come un modello finanziario in un foglio di calcolo. Nel senso moderno dell'IA, un modello è un file pieno di numeri che sono stati regolati finché le risposte non uscivano giuste. Quando oggi qualcuno dice "il modello", di solito intende la seconda cosa.

**Addestramento.** Il processo che porta dal nulla a un modello. Mostra esempi. Lascia che il sistema indovini. Confronta con la risposta giusta. Regola. Ripeti molte volte. Il Capitolo 2 ha spiegato il meccanismo. Qui conta il significato aziendale: **l'addestramento è un passo che paghi una volta sola, e la sua qualità fissa il limite massimo di tutto ciò che viene dopo.** Un modello addestrato su esempi scadenti non si aggiusta con un'interfaccia migliore. Si può solo riaddestrare, cioè pagare di nuovo.

Tre domande che chiariscono quasi ogni conversazione:

1. **Qual è l'input?** Cosa entra?
2. **Qual è l'output?** Cosa esce?
3. **Su cosa è stato addestrato?** Quali esempi, da quando, quanti?

Se un fornitore non sa rispondere alla terza domanda, non stai comprando un modello. Stai comprando una promessa.

### 3.3 IA generativa, LLM, prompt

**IA generativa** è un'IA che produce contenuti nuovi invece di limitarsi a ordinare o assegnare punteggi. Il Capitolo 2 l'ha definita. Ecco il vocabolario che la circonda.

**LLM — large language model (grande modello linguistico).** "Grande" significa che ha molte impostazioni regolabili, misurate in miliardi. Queste impostazioni si chiamano **parametri**. Un modello da 13 miliardi di parametri contiene 13.000.000.000 di numeri. "Linguistico" significa che è stato addestrato su testo. "Modello" significa che è il risultato utilizzabile dell'addestramento.

Quindi un LLM è un insieme molto grande di numeri, regolati leggendo un'enorme quantità di testo, finché non è diventato bravo a proseguire il testo. È tutta qui. Non è un database di fatti. È una macchina che prosegue il testo.

**Prompt.** Il testo che dai al modello. La tua domanda, la tua istruzione, la tua richiesta. Tutto qui è un prompt.

La parola conta più di quanto sembri, perché ciò che ricevi indietro dipende molto dal prompt. Un prompt vago dà una risposta vaga. Un prompt con contesto, un esempio e un formato chiaro ne dà una molto migliore. Imparare a scrivere buoni prompt è una vera abilità aziendale, e si impara bene in circa una settimana.

Un prompt è come un brief che dai a un copywriter freelance. Un brief cattivo — "scrivi qualcosa sul nostro prodotto" — produce qualcosa di inutile. Un brief buono — "scrivi 150 parole per piccoli negozianti, in inglese semplice, con questo tono, e lascia fuori i prezzi" — produce qualcosa che puoi usare. Lo scrittore è lo stesso. È cambiato solo il brief.

**Allucinazione.** Quando un modello afferma qualcosa di falso in modo sicuro. La parola è imperfetta, perché il modello non allucina in alcun senso medico. Sta proseguendo il testo in un modo che suona giusto, senza un archivio separato di fatti con cui confrontarsi. Ecco perché l'IA generativa ha bisogno di verifica per tutto ciò che conta.

**Finestra di contesto.** Quanta testo il modello può considerare in una volta. Pensala come una scrivania. Tutto ciò che vuoi che guardi deve starci sopra. Il testo che non entra semplicemente non c'è. Le scrivanie moderne sono grandi, ma non infinite, e una scrivania affollata funziona peggio di una ordinata.

**Chiedi al fornitore:** "Quale modello usate, chi lo ha creato, e dove finiscono il mio prompt e i miei dati quando li invio?"

### 3.4 RPA, no-code, low-code

Queste tre parole vengono vendute come se fossero IA. Di solito non lo sono.

**RPA — Robotic Process Automation (automazione robotica dei processi).** Software che copia ciò che una persona fa al computer: apri questo sistema, copia questo campo, incollalo in quell'altro sistema, clicca Salva. Funziona imitando le azioni di mouse e tastiera, oppure usando le stesse schermate che usa una persona. Il termine entrò in uso nei primi anni 2000.

La RPA non è IA. Non ha apprendimento e non fa ipotesi. Segue una sequenza registrata alla lettera. È affidabile e fragile allo stesso tempo. L'analogia è una macro in un foglio di calcolo: fa gli stessi passi ogni volta, velocemente, e si rompe se cambia la disposizione.

**Quando la RPA è giusta:** il compito è fisso, ad alto volume, e le schermate non cambiano. Copiare i dati di un ordine da un'email nel tuo sistema ordini cento volte al giorno è un classico lavoro da RPA. È economico e funziona.

**Quando la RPA è sbagliata:** tutto ciò che varia. Se l'input non è sempre nello stesso posto, la RPA si romperà, e lo farà spesso.

Uno schema comune e sensato: **l'IA legge e capisce l'input disordinato; la RPA fa la digitazione noiosa.** L'IA gestisce la variazione. La RPA gestisce la ripetizione.

**No-code.** Strumenti in cui costruisci un'automazione cliccando, trascinando e scegliendo da un menu, senza scrivere codice di programmazione. Buoni per flussi di lavoro semplici e chiari. Veloci da avviare.

**Low-code.** Simili, ma puoi scrivere un po' di codice quando il menu non offre ciò che ti serve. Più flessibili, un po' più tecnici.

Entrambi sono davvero utili, e entrambi hanno un costo nascosto: sono facili da iniziare e difficili da finire. Un flusso no-code che cresce fino a venti passi, tre sistemi e quattro persone che lo modificano diventa difficile da capire e pericoloso da cambiare. C'è uno schema noto in cui un'azienda costruisce decine di piccole automazioni no-code, nessuno riesce a mapparle tutte, e alla fine qualcuno deve ricostruire tutto.

**Chiedi al fornitore:** "Questo impara davvero qualcosa, o segue una sequenza fissa? Se una schermata cambia, cosa si rompe e chi lo aggiusta?"

### 3.5 Cloud, API, integrazione

**Cloud.** Il computer di qualcun altro. Questa è la definizione onesta. I tuoi file e i tuoi software girano su macchine in un grande centro dati che un'altra azienda possiede e mantiene, e tu paghi in base all'uso via internet.

Il cloud ha vantaggi reali: nessun hardware da comprare, capacità che puoi far crescere in pochi minuti, manutenzione automatica. Ha anche una conseguenza permanente: **i tuoi dati sono sulle macchine di qualcun altro, in un paese che potresti non aver scelto, sotto un contratto che probabilmente non hai letto.** Il [Capitolo 8](ch08-self-hosting-keep-your-data-under-control.md) tratta la gestione in proprio, e il [Capitolo 11](ch11-digital-sovereignty.md) tratta il controllo e la sovranità.

**API — application programming interface (interfaccia di programmazione delle applicazioni).** Un modo definito con cui un software chiede a un altro di fare qualcosa.

Pensa alla cucina di un ristorante. Non puoi entrare e cucinarti il pasto da solo. Vai a una finestra e ordini da un menu fisso. La cucina ti dice esattamente cosa puoi ordinare e come. Quella finestra è l'API: permette al mondo esterno di usare la cucina senza romperla.

In pratica, il tuo sito web chiede all'API della società di spedizioni "quanto costa spedire questo pacco a Madrid?" e riceve un numero in pochi secondi. Nessuno telefona a nessuno.

Due cose da sapere. Primo, se il prodotto di un fornitore non ha un'API, non puoi collegarvelo tu stesso, e dipendi da quel fornitore per sempre. Secondo, ogni chiamata API significa che i dati attraversano un confine. Ognuna è una piccola porta. Alcune porte sono chiuse e registrate. Altre no.

**Integrazione.** Collegare sistemi in modo che i dati si muovano tra loro senza che una persona li trasporti. È qui che la maggior parte dei progetti spende davvero tempo e denaro, e i fornitori raramente dicono quale livello intendono:

1. **File.** Esporta un foglio di calcolo, caricarlo da qualche parte. Semplice, lento, soggetto a errori.
2. **API.** Una connessione diretta. Veloce, affidabile, richiede lavoro di configurazione.
3. **Nativa.** Integrata nella stessa piattaforma. La migliore, ma ti blocca su quella piattaforma.

**Chiedi al fornitore:** "A quali sistemi vi collegate oggi, con quale metodo, chi fa la configurazione, e cosa succede alla connessione se noi ce ne andiamo?"

## Un po' di storia

Le parole sono più antiche della tecnologia, e saperlo aiuta.

**Algoritmo** viene da al-Khwarizmi, un matematico persiano del IX secolo i cui libri descrivevano il calcolo passo per passo. La parola ha più di mille anni più del computer. **Dato** viene dal latino per "cose date" — fatti nel senso più semplice, molto prima che significasse qualcosa di memorizzato. **Rete neurale** viene dagli anni '40, dai primi tentativi di descrivere una cellula cerebrale come un minuscolo interruttore acceso/spento; la frase è rimasta anche se i sistemi moderni somigliano poco ai cervelli reali. **Machine learning** fu battezzato nel 1959 da Arthur Samuel, un ricercatore americano che lavorava a un programma di dama. **Large language model** entrò nell'uso comune intorno al 2018, quando apparvero modelli addestrati su testo su scala web. **Prompt** è preso in prestito dall'informatica più antica, dove indicava il punto in cui digiti; ora significa l'istruzione che dai a un modello, che è un compito molto più grande che digitare. **RPA** apparve nei primi anni 2000 per descrivere software che imita un umano davanti a uno schermo, e **low-code** e **no-code** entrarono nel vocabolario aziendale intorno al 2014.

La lezione nel vocabolario è semplice. Quasi nessuna di queste parole fu inventata da chi ha costruito la tecnologia. Furono prese in prestito, allungate, e poi vendute. Ecco perché sembrano vaghe. Sono vaghe. Il tuo compito è fissarne ciascuna con precisione prima di firmare qualsiasi cosa.

## Curiosità

### 3.6 Un modello addestrato solo su dati degli anni '30 ha scritto Python — come è possibile?

Nell'aprile 2026 un piccolo team di ricerca pubblicò un insolito modello linguistico. Si chiamava **talkie**, e tutto il suo senso stava in ciò che non sapeva.

Il team — Nick Levine, David Duvenaud dell'Università di Toronto, e Alec Radford — addestrò un modello da 13 miliardi di parametri su testo inglese pubblicato solo prima del 1931. Circa 260 miliardi di token. Un **token** è un piccolo frammento di testo, più o meno una parola o parte di una parola. Le fonti erano libri digitalizzati, giornali, periodici, riviste scientifiche, brevetti e giurisprudenza.

Nulla dal 1930 in poi entrò. Niente computer. Niente internet. E soprattutto, nessun linguaggio di programmazione, perché Python non fu creato fino alla fine degli anni '80.

Poi testarono se sapesse scrivere Python.

**Il risultato.** Sapeva, un po'. Il team diede al modello un test di programmazione standard chiamato HumanEval, con un colpo di scena: ogni problema veniva presentato con alcune funzioni di esempio casuali mostrate direttamente nella domanda. Il modello non aveva mai visto Python nell'addestramento. Ma poteva guardare gli esempi davanti a sé e copiare la struttura.

I risultati furono onesti e modesti. Il modello vintage otteneva un punteggio molto inferiore ai modelli moderni. Ogni risposta corretta che produceva era un semplice programma di una riga, come sommare due numeri, o una piccola modifica a uno degli esempi che gli venivano mostrati. Come lo mise il team, c'è ancora molta strada da fare prima che questa capacità sia notevole.

Ma un esempio era davvero sorprendente. Mostrata una funzione che codificava un cifrario a rotazione — un codice in cui ogni lettera si sposta di una quantità fissa — il modello produsse la funzione di decodifica cambiando un singolo carattere, trasformando un'addizione in una sottrazione. Non aveva mai visto Python. Non aveva mai visto un computer. Capì, dalla forma dell'esempio davanti a sé, che decodificare è l'opposto di codificare.

**Come è possibile?** La risposta è un comportamento chiamato **apprendimento nel contesto**: cogliere uno schema dagli esempi posti direttamente nella domanda, anziché dall'addestramento.

Ecco la versione semplice. Per leggere bene il testo, un modello deve diventare estremamente bravo a notare la struttura. Quale parola segue quale. Cosa si apre e cosa si chiude. Cos'è una definizione e cos'è un esempio. Cos'è una causa e cos'è un effetto. Impara tutto questo da comuni libri e giornali.

La struttura, a quanto pare, si trasferisce. Un modello che è diventato molto bravo a notare "questo blocco si apre qui, si chiude là, e questo valore confluisce in quell'altro" può applicare la stessa abilità a un blocco di Python che non ha mai visto. Non sta usando conoscenza di Python. Sta usando conoscenza della struttura su materiale Python.

Ecco perché poteva invertire la funzione del cifrario. Non stava programmando. Era seguire uno schema applicato a una materia che non esisteva nei suoi dati di addestramento.

**Perché i ricercatori l'hanno fatto.** La ragione è pratica e intelligente: un modello addestrato solo su testo pre-1931 non può aver memorizzato il test. I modelli moderni sono addestrati sul web moderno, che contiene le risposte alla maggior parte delle domande dei test pubblici. Questo si chiama **contaminazione dei dati**, e rende inaffidabili i benchmark moderni. Un modello può ottenere un buon punteggio perché ha visto la risposta prima, non perché sappia ragionare. Talkie è pulito per costruzione. Qualunque cosa faccia, l'ha davvero fatta.

**I limiti onesti.** Il team riportò anche che talkie si comportava peggio nel complesso rispetto al suo "gemello moderno" — un modello identico addestrato su dati web moderni — anche dopo aver corretto il fatto che le domande moderne confondono un modello degli anni '30. Attribuirono parte del divario al rumore dell'OCR: nel 1930 nulla era digitale, quindi ogni pagina doveva essere scansionata e trascritta, il che introduce errori che il testo nativo digitale non ha. Dissero che come sforzo di ricerca amatoriale non si aspettavano mai di colmare del tutto il divario. Stimarono però che il corpus storico potesse crescere ben oltre un trilione di token, abbastanza per un modello più o meno paragonabile al ChatGPT originale.

**La lezione aziendale.** Due cose.

Primo, questi modelli sono seguaci di strutture più che collezionisti di fatti. Questo spiega sia il loro potere sia la loro inaffidabilità. La struttura si trasferisce bene. La verità non arriva con essa.

Secondo, **la contaminazione dei dati è un problema reale nelle affermazioni dei fornitori.** Quando un fornitore dice "il nostro modello ottiene il 94% su questo benchmark", chiedi se il benchmark era nei dati di addestramento. Non è una piccola sottigliezza tecnica. È la differenza tra una capacità misurata e una risposta memorizzata. Chiedilo in ogni riunione con un fornitore.

## Un esempio aziendale reale

### Quando le parole sono il prodotto: "AI washing"

Nel settembre 2024 la Federal Trade Commission degli Stati Uniti annunciò un'operazione di controllo che chiamò **Operation AI Comply**. L'obiettivo erano aziende che facevano affermazioni esagerate o ingannevoli su ciò che i loro prodotti potevano fare con l'intelligenza artificiale. Il nome stesso della FTC per questa pratica è **AI washing**.

Lo schema descritto dai regolatori è semplice, e vale la pena riconoscerlo, perché è così che iniziano i cattivi acquisti di IA.

Un'azienda ha un prodotto ordinario. Forse uno strumento di pianificazione, o di automazione del marketing, o un chatbot costruito da un elenco fisso di risposte. L'azienda aggiunge "alimentato dall'IA" al marketing. Nulla nel prodotto cambia. Il prezzo sale. Le vendite salgono.

La posizione della FTC è che questo è un problema di tutela del consumatore, non tecnico. Se affermi una capacità che non hai, è un'affermazione ingannevole, e l'etichetta "IA" non ti protegge da essa.

**Perché questo è un esempio aziendale e non solo legale.** Perché la stessa trappola funziona in entrambe le direzioni. I fornitori usano le parole con leggerezza per vendere. Gli acquirenti usano le parole con leggerezza per giustificare un budget internamente. Un manager che non sa spiegare cosa fa la tecnologia scrive "automazione guidata dall'IA" in una proposta, ottiene l'approvazione del budget, e poi deve far funzionare qualcosa che nessuno ha definito.

L'operazione del regolatore ti è utile come checklist al contrario. Prima di comprare, chiedi:

1. **Quale affermazione specifica viene fatta?** Scrivila in una frase con un verbo e un oggetto.
2. **Come sapremmo se quell'affermazione fosse falsa?** Se nessuno sa indicare un test, l'affermazione è decorazione.
3. **L'affermazione è nel contratto?** Il linguaggio del marketing non è un impegno. Se una capacità conta, dovrebbe essere scritta con un numero e una data.
4. **Chi è responsabile se non funziona?** Nomina una persona, non un'azienda.

Un fornitore onesto risponde a tutte e quattro con sicurezza. Un fornitore che fa washing diventa vago. La vaghezza in risposta a domande specifiche è di per sé la risposta.

## Come si fa

### Il test delle parole semplici

Usalo ogni volta che un termine tecnico appare in una riunione.

**Passo 1: Fermati sulla parola.** Non lasciarla passare perché suona importante.

**Passo 2: Chiedi una frase con un verbo e un oggetto.** Non "usa un grande modello linguistico", ma "legge le nostre email di assistenza e prepara una bozza di risposta". Se chi parla non riesce a produrne una, la parola non ha ancora contenuto.

**Passo 3: Chiedi cosa entra e cosa esce.** Ogni sistema reale ha un input e un output. Scrivi entrambi.

**Passo 4: Chiedi cosa lo rompe.** Ogni tecnologia ha una modalità di guasto. Un fornitore onesto nomina la sua.

**Passo 5: Scrivi la tua definizione su una riga e rileggila.** Se un collega intelligente non la capisse, la definizione non è finita.

### La tua tabella di traduzione operativa

| Parola che senti | Significato semplice | Cosa chiedere |
|---|---|---|
| Alimentato dall'IA | Usa qualche componente imparato, magari minuscolo | Quale parte, esattamente? |
| Modello | Un file di impostazioni imparate che risponde a nuovi casi | Addestrato su cosa, quando, quanto? |
| Addestramento | Regolare le impostazioni contro esempi finché le risposte corrispondono | Chi l'ha fatto, e chi l'ha verificato? |
| LLM | Un sistema di continuazione di testo molto grande | Quale, fatto da chi, in esecuzione dove? |
| Prompt | L'istruzione che dai al modello | Possiamo scrivere e riutilizzare i nostri? |
| Allucinazione | Un'affermazione sicura che è falsa | Come la rilevate e correggete? |
| RPA | Software che imita una persona che clicca sugli schermi | Cosa si rompe quando lo schermo cambia? |
| No-code | Costruire cliccando, senza programmare | Cosa non può fare? |
| Low-code | Soprattutto cliccare, un po' di programmazione consentita | Chi lo mantiene qui? |
| Cloud | Gira sui computer di qualcun altro | Quale paese, quale contratto, quali dati escono? |
| API | Una finestra definita perché un sistema usi un altro | Esiste? Possiamo usarla noi stessi? |
| Integrazione | I dati si muovono tra sistemi senza una persona | Quale metodo, chi lo configura, e se noi ce ne andiamo? |
| Token | Un piccolo frammento di testo | Quanti per un uso tipico, e quanto costano? |
| Finestra di contesto | Quanta testo il modello può guardare in una volta | Cosa succede quando il nostro documento è troppo grande? |

### Costruisci un glossario condiviso per la tua azienda

Fallo una volta e tienilo vivo.

1. Avvia una singola pagina. Ogni termine che emerge in una discussione sull'IA ci finisce.
2. Ogni voce riceve tre righe: il significato semplice, cosa significa *nella nostra azienda*, e una domanda a cui ancora non sappiamo rispondere.
3. Una persona con un nome possiede la pagina. Non un comitato.
4. Prima di ogni riunione con un fornitore, leggi la pagina. Durante la riunione, aggiungici.
5. Ritira le voci che non usi mai. Tienilo sotto le due pagine.

Un glossario condiviso è una piccola cosa con un effetto enorme. Trasforma "abbiamo comprato l'IA" in "usiamo un modello di testo per preparare bozze di risposta e uno strumento a regole per archiviarle, e una persona controlla entrambi".

## Etica e responsabilità

### 3.7 Privacy, sicurezza, bias — la versione breve

Tre parole che sentirai costantemente. Ecco l'introduzione semplice. Il trattamento completo vive altrove, e dovresti leggere quei capitoli prima di distribuire qualsiasi cosa che tocchi i dati dei clienti.

La **privacy** riguarda chi è autorizzato a vedere e usare le informazioni personali. La domanda pratica per ogni strumento IA è semplice: *quando incollo qualcosa, dove va, chi può leggerlo, e cosa ne conservano?* Non inserire mai i dati personali di un cliente in uno strumento che non hai verificato. Il [Capitolo 10](ch10-privacy-and-gdpr.md) tratta la privacy e il GDPR come si deve.

La **sicurezza** riguarda la protezione dei sistemi da attacchi, abusi e incidenti. L'IA aggiunge nuovi modi per essere attaccati, incluso ingannare un modello con input formulati con cura e avvelenare i dati da cui impara. Il [Capitolo 6](ch06-cybersecurity-in-the-ai-era.md) tratta questo per intero.

Il **bias** (pregiudizio) è quando un sistema tratta alcune persone peggio di altre in modo sistematico, perché gli esempi da cui ha imparato erano squilibrati. Se le passate decisioni di assunzione favorivano un gruppo, un modello addestrato su di esse imparerà a favorire quel gruppo. Il bias non è un fallimento morale della macchina. È uno specchio tenuto davanti agli esempi. Il [Capitolo 4](ch04-ethical-ai-doing-the-right-thing.md) tratta bias, trasparenza, spiegabilità e responsabilità umana come parte del quadro etico completo.

L'unica cosa da portare via da questa sezione: **non puoi gestire un rischio che non sai nominare.** Imparare le parole non è accademico. È il primo requisito per fare le domande giuste.

## Errori da evitare

**Errore 1: Accettare "IA" come una funzionalità.** Non è una funzionalità. È una categoria che contiene decine di tecnologie molto diverse. Chiedi quale.

**Errore 2: Pensare che no-code significhi non pensare.** Il no-code elimina la programmazione. Non elimina il design, la manutenzione, o il rischio di un groviglio inestricabile di automazioni.

**Errore 3: Confondere la RPA con l'IA.** Se segue una sequenza registrata, non sta imparando nulla. Può essere esattamente ciò che vuoi, o esattamente ciò che fallirà.

**Errore 4: Pensare che un'API significhi che sei integrato.** Un'API è una possibilità, non una connessione. Qualcuno deve comunque costruire e mantenere la connessione.

**Errore 5: Non chiedere dove si trova davvero il cloud.** "Il cloud" è un centro dati, in un paese, sotto un contratto. Chiedi quale.

**Errore 6: Lasciare che un fornitore definisca i tuoi termini.** Se il vocabolario del fornitore è l'unico vocabolario nella stanza, il fornitore controlla la riunione.

**Errore 7: Saltare il test delle parole semplici perché sembra lento.** Cinque minuti di "cosa significa davvero?" costano meno di sei mesi di un progetto che nessuno sa descrivere.

**Errore 8: Credere a un benchmark senza chiedere della contaminazione.** L'esperimento Talkie esiste proprio perché i risultati dei test moderni possono essere gonfiati da risposte già presenti nei dati di addestramento.

## Esercizio pratico

### 3.8 Traduci una frase tecnica in parole semplici

Questa è l'abilità più utile di tutto il capitolo. Esercitati su queste sei frasi. Scrivi la tua risposta prima di leggere la risposta modello.

**Frase 1:** "La nostra piattaforma sfrutta un grande modello linguistico per offrire elaborazione intelligente dei documenti su larga scala."

*Risposta modello:* "Legge documenti e ne estrae le informazioni. Usa un grosso sistema di testo per farlo. Gestisce molti documenti alla volta."

**Frase 2:** "La soluzione è un bot RPA low-code con integrazione API basata su cloud."

*Risposta modello:* "Un robot che copia dati da uno schermo all'altro. Puoi configurarlo soprattutto cliccando. Parla con altri sistemi su internet attraverso una connessione definita. Gira sui computer del fornitore."

**Frase 3:** "Usiamo la generazione aumentata dal recupero per fondare il modello sulla vostra base di conoscenza."

*Risposta modello:* "Prima di rispondere, cerca le pagine rilevanti nei vostri documenti e le usa come base. Questo riduce le risposte inventate. Funziona solo se i vostri documenti sono buoni e aggiornati."

**Frase 4:** "Il modello è messo a punto sui vostri dati di settore."

*Risposta modello:* "Hanno preso un modello generale esistente e lo hanno addestrato ulteriormente sui vostri esempi, così si adatta meglio al vostro business. Per questo pagate. Significa anche che i vostri dati sono stati inviati a chi ha fatto l'addestramento."

**Frase 5:** "La nostra IA fornisce un processo decisionale spiegabile e trasparente."

*Risposta modello:* "Affermano che puoi vedere perché ha deciso ciò che ha deciso. Chiedi loro di mostrartelo, su un caso reale, adesso. Se non possono, l'affermazione è decorazione."

**Frase 6:** "È un sistema multi-agente con orchestrazione."

*Risposta modello:* "Diverse componenti di IA lavorano su un compito in sequenza o in parallelo, e qualcosa le coordina. Chiedi: quante componenti, cosa fa ciascuna, e cosa succede se una fallisce?"

**Ora fai il tuo.** Trova una frase da un'email di un fornitore che hai ricevuto nell'ultimo mese. Tradurla con lo stesso metodo: verbo e oggetto, input, output, cosa si rompe. Manda la tua traduzione indietro al fornitore e chiedi se è corretta. La loro reazione ti dirà moltissimo.

## Checklist

### 3.9 Il tuo glossario minimo

- [ ] So spiegare dati, informazione e conoscenza, e so quanta della conoscenza della mia azienda è scritta.
- [ ] So definire algoritmo come "una ricetta": una serie ordinata di passi.
- [ ] So definire modello come "la cosa addestrata che usi per rispondere a nuovi casi".
- [ ] So definire addestramento come "regolare le impostazioni contro esempi finché le corrispondono".
- [ ] So che un LLM è un sistema di continuazione di testo, non un database di fatti.
- [ ] So che un prompt è l'istruzione che do al modello, e che la sua qualità cambia il risultato.
- [ ] So cos'è un token e più o meno quanto costano i token per un uso tipico.
- [ ] So cos'è una finestra di contesto e cosa succede quando un documento è troppo grande per essa.
- [ ] So che "allucinazione" significa un'affermazione falsa detta con sicurezza, e che serve verifica.
- [ ] So distinguere la RPA dall'IA, e so che la RPA è economica e fragile.
- [ ] So che no-code e low-code eliminano la programmazione, non il design o la manutenzione.
- [ ] So che "il cloud" significa i computer di qualcun altro, in un paese specifico, sotto un contratto specifico.
- [ ] So che un'API è una finestra definita perché un sistema usi un altro, e chiedo sempre se ne esiste una.
- [ ] So i tre livelli di integrazione: file, API, nativa.
- [ ] Uso il test delle parole semplici: un verbo, un oggetto, un input, un output, e cosa si rompe.
- [ ] Ho iniziato un glossario condiviso di una pagina con un proprietario nominato.
- [ ] So che privacy, sicurezza e bias hanno ciascuno un capitolo completo, e li ho letti o li leggerò.

## Punti chiave

- La maggior parte delle cattive decisioni sull'IA viene da parole non definite, non da una tecnologia scadente.
- Una spiegazione vera contiene sempre un verbo e un oggetto; se non riesci a nominarne uno, non ti è stato detto nulla.
- I modelli sono seguaci di strutture, non custodi di fatti, ed è per questo che trasferiscono abilità tra materie e che affermano falsità con sicurezza.
- L'esperimento Talkie mostra che un modello senza conoscenza dei computer può comunque scrivere un po' di Python, ed esiste perché i risultati dei benchmark moderni possono essere gonfiati da dati contaminati.
- Fissa ogni termine con precisione prima di firmare: cosa entra, cosa esce, cosa lo rompe, e chi lo possiede.
