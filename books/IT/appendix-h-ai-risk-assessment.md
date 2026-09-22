# Appendice H — Valutazione dei rischi dell'IA

Prima di lanciare un progetto IA, chiediti cosa potrebbe andare storto e quanto sarebbe grave. Questa tabella rende visibili i rischi così puoi ridurli, non ignorarli. Compilala con il tuo team. Fallo presto, e ripassala spesso.

## Come assegnare i punteggi

Valuta ogni rischio su due scale:

- **Probabilità** — Quanto è probabile? **Bassa / Media / Alta**
- **Impatto** — Quanto è grave se accade? **Basso / Medio / Alto**

Combinali in un **Livello di rischio**:

| | Impatto Basso | Impatto Medio | Impatto Alto |
|---|---|---|---|
| **Probabilità Alta** | Medio | Alto | **Critico** |
| **Probabilità Media** | Basso | Medio | Alto |
| **Probabilità Bassa** | Basso | Basso | Medio |

Tratta **Critico** e **Alto** come da sistemare obbligatoriamente prima del lancio.

## Modello vuoto

| Rischio | Cosa potrebbe andare storto | Probabilità | Impatto | Livello di rischio | Mitigazione | Responsabile |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Esempi compilati

| Rischio | Cosa potrebbe andare storto | Probabilità | Impatto | Livello di rischio | Mitigazione | Responsabile |
|---|---|---|---|---|---|---|
| Dati errati nell'IA | Il personale incolla dati personali dei clienti in uno strumento pubblico | Alta | Alto | **Critico** | Elenco solo strumenti approvati; bloccare gli strumenti pubblici sui dispositivi aziendali; formazione | Responsabile IT |
| Output errato usato | L'IA scrive una fattura con un importo sbagliato, inviata al cliente | Media | Alto | Alto | Revisione umana prima dell'invio; controllo automatico dei totali | Impiegata contabilità |
| Pregiudizio nelle decisioni | Uno strumento di assunzioni favorisce un gruppo per dati di addestramento sbilanciati | Media | Alto | Alto | Decide un umano; rivedi gli esiti per equità; evita assunzioni totalmente automatizzate | Responsabile HR |
| Fuga dal fornitore | Il fornitore subisce una violazione e i dati dei clienti sono esposti | Bassa | Alto | Medio | Checklist del fornitore; cifrare i dati; clausola contrattuale di avviso di violazione | Responsabile IT |
| Eccessivo affidamento | Il personale smette di controllare e si fida dell'IA ciecamente | Media | Media | Medio | Mantieni l'approvazione umana; audit a campione; formazione sui limiti | Responsabile di team |
| Prompt injection | Un documento nasconde istruzioni che ingannano l'IA | Media | Media | Medio | Tratta il testo esterno come non affidabile; limita cosa l'IA può farne | Responsabile IT |
| Lock-in | Impossibile lasciare il fornitore o esportare i dati | Bassa | Media | Medio | Clausola di esportazione dati nel contratto; tieni una copia | Titolare |
| Costi fuori controllo | L'uso cresce e la fattura schizza | Media | Media | Medio | Imposta avvisi d'uso; rivedi il piano ogni mese; metti un tetto al costo per compito | Titolare |
| Deriva del modello | Il fornitore cambia il modello e la qualità dell'output cala | Media | Media | Medio | Controlli a campione dell'output ogni settimana; tieni casi di test per confrontare | Responsabile di team |

## Guida alle colonne

- **Rischio** — Un nome corto per il rischio.
- **Cosa potrebbe andare storto** — Lo scenario concreto, non una vaga preoccupazione.
- **Probabilità / Impatto** — Basso / Medio / Alto.
- **Livello di rischio** — Dalla griglia qui sopra.
- **Mitigazione** — Cosa farai per abbassare la probabilità o l'impatto.
- **Responsabile** — L'unica persona che assicura che la mitigazione avvenga.

## Rischi IA comuni da considerare

Usa questo elenco per far scaturire le tue righe:

- [ ] Dati personali o sensibili trapelati a uno strumento esterno.
- [ ] Output errato a cui si crede senza revisione.
- [ ] Pregiudizio o iniquità nelle decisioni automatizzate.
- [ ] Violazione della sicurezza del fornitore.
- [ ] Prompt injection da documenti non affidabili.
- [ ] Shadow AI (personale che usa strumenti non approvati).
- [ ] Eccessivo affidamento e perdita di competenze.
- [ ] Costi fuori controllo al crescere dell'uso.
- [ ] Lock-in su un fornitore.
- [ ] Mancata conformità al GDPR o all'EU AI Act.
- [ ] Fiducia del cliente persa dopo un errore visibile.
- [ ] Cambiamenti silenziosi del modello e calo della qualità dell'output.

## Quando rilanciare questa valutazione

Ripassa la tabella quando accade una di queste cose:

- Aggiungi un nuovo strumento, una nuova fonte di dati o un nuovo processo.
- L'uso cresce molto, o lo strumento tocca più persone.
- Si verifica un incidente o un quasi-incidente.
- Una legge o un requisito del cliente cambia.
- Un fornitore cambia i suoi termini, il modello, o dove archivia i dati.

## Due modi per ridurre un rischio

Ogni mitigazione tira una di due leve:

- **Abbassa la probabilità** — rendi meno probabile l'evento negativo. Esempio: un elenco di soli strumenti approvati rende meno probabile una fuga di dati.
- **Abbassa l'impatto** — rendi più piccolo il danno se accade. Esempio: la revisione umana fa sì che una fattura errata venga presa prima che arrivi al cliente.

Un buon piano spesso tira entrambe le leve. Per ogni rischio chiediti: "Cosa rende questo meno probabile, e cosa limita il danno se accade comunque?"

Se un rischio resta **Critico** anche dopo la mitigazione, non lanciare. Rimuovi il passo rischioso o riprogetta il processo.

## Regole

- Ogni rischio Critico o Alto ha bisogno di una mitigazione **e** di un responsabile prima del lancio.
- Una mitigazione senza responsabile non è una mitigazione.
- Rilancia questa valutazione a ogni traguardo — i rischi cambiano.
- Se un rischio Critico non può essere ridotto, non lanciare. Dillo.
