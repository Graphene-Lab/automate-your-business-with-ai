# Appendice D — Inventario dei dati

Non puoi proteggere dati che non riesci a trovare. Questo elenco classifica ogni elemento di dati importante che la tua azienda detiene, dove vive, e chi può raggiungerlo. Compilalo prima di collegare qualsiasi strumento di IA. Se un dato non è in questo elenco, non darlo in pasto all'IA.

## Come usarlo

1. Passa in rassegna i tuoi strumenti: email, unità disco, contabilità, CRM, sistemi HR, fogli di calcolo.
2. Aggiungi una riga per elemento di dati (un elenco clienti, un file delle paghe, una cartella di contratti).
3. Segna ogni elemento **Personale** (riguarda una persona) o **Sensibile** (categorie particolari — vedi sotto).
4. Controlla l'accesso: chi può aprirlo oggi, e chi *dovrebbe* poterlo fare.
5. Rivedilo prima di ogni progetto IA. Questo elenco ti dice cosa è sicuro usare e cosa no.

## Modello vuoto

| Elemento di dati | Dove è archiviato | Responsabile | Personale / Sensibile? | Chi può accedervi | Stato del backup | Conservazione |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Esempio compilato

| Elemento di dati | Dove è archiviato | Responsabile | Personale / Sensibile? | Chi può accedervi | Stato del backup | Conservazione |
|---|---|---|---|---|---|---|
| Elenco contatti clienti | CRM (cloud) | Responsabile vendite | Personale (nomi, email, telefoni) | Team vendite (modifica), Finanza (sola lettura) | Quotidiano, fuori sede | Tieni finché attivo + 3 anni |
| File delle paghe | Unità condivisa, cartella "HR" | Responsabile HR | Sensibile (stipendio, documento d'identità, banca) | Solo HR | Settimanale, fuori sede | 10 anni (per legge) |
| Contratti dei fornitori | Armadio di carta + cartella scansionata | Titolare | Nessuno (riservato aziendale) | Titolare, Finanza | Parziale (solo scansioni) | Vita del contratto + 6 anni |

## Dove cercare i dati

Passa in rassegna ciascuno di questi. I dati si nascondono in bella vista:

- [ ] Caselle email condivise e caselle personali.
- [ ] Unità condivise e cartelle di rete.
- [ ] Strumenti cloud: CRM, contabilità, HR, strumenti di progetto.
- [ ] Fogli di calcolo e allegati (spesso la cosa più disordinata).
- [ ] File di carta, armadi e copie scansionate.
- [ ] Backup ed esportazioni vecchie.
- [ ] Strumenti di chat e storico dei messaggi.
- [ ] Telefoni e laptop del personale.
- [ ] Strumenti di terze parti a cui il personale si è iscritto per conto proprio (copie ombra).

## Cosa conta come "Sensibile"

Sotto il GDPR, queste categorie particolari richiedono una cura extra. Segnale chiaramente:

- Dati sanitari
- Origine razziale o etnica
- Opinioni politiche
- Credenze religiose o filosofiche
- Iscrizione a sindacati
- Dati genetici e biometrici (per identificazione)
- Vita sessuale o orientamento sessuale

Tratta come sensibile anche se non di "categoria speciale": dati bancari, numeri di documento d'identità, password, dati dei bambini e tutto ciò che potrebbe danneggiare una persona se trapelasse.

## Guida alle colonne

- **Elemento di dati** — Un nome semplice per la cosa (non il nome del file).
- **Dove è archiviato** — Sistema e posizione: strumento cloud, percorso su unità, armadio di carta.
- **Responsabile** — Una persona responsabile.
- **Personale / Sensibile?** — Personale, Sensibile, o Nessuno.
- **Chi può accedervi** — Ruoli o persone, e se possono leggere o modificare.
- **Stato del backup** — Quanto spesso viene fatto il backup, e dove. Segna se **non** c'è backup.
- **Conservazione** — Per quanto lo conservi, e perché (regola di legge o esigenza di business).

## Campanelli d'allarme da sistemare subito

- [ ] Dati sensibili senza un responsabile.
- [ ] Dati sensibili che chiunque in azienda può aprire.
- [ ] Dati importanti senza backup.
- [ ] Dati conservati "per sempre" senza motivo.
- [ ] Dati personali in uno strumento che non controlli (shadow AI, email personale).
- [ ] Gli stessi dati in molti posti senza una copia principale.

## Regole pratiche di conservazione

- Conserva i dati solo finché ti servono. Più a lungo non è più sicuro — è più rischio.
- Controlla i minimi di legge: i registri fiscali e delle paghe hanno spesso anni fissi. Chiedi al tuo commercialista.
- Per i dati dei clienti, conservali finché il rapporto è attivo, poi un periodo breve e dichiarato.
- Cancella o anonimizza i dati che non ti servono più. Non lasciarli accumulare.
- Scrivi il motivo di ogni periodo di conservazione, così nessuno deve indovinare dopo.

## Tenere l'inventario aggiornato

- Rivedilo ogni 6 mesi, e prima di ogni nuovo progetto IA.
- Aggiungi una riga il giorno in cui appare un nuovo strumento o una nuova fonte di dati.
- Nomina un responsabile per elemento; i responsabili lo tengono onesto.
- Trattalo come un documento vivo, non una faccena una tantum.

## Regola per i progetti IA

Prima che qualsiasi dato entri in uno strumento di IA, controlla questo inventario. Se un elemento è **Sensibile**, ti serve un motivo chiaro, uno strumento sicuro e spesso una DPIA. In caso di dubbio, lascialo fuori.
