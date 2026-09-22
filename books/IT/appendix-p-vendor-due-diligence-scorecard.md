# Appendice P — Scorecard di due diligence sul fornitore di IA

Usala per confrontare i fornitori con numeri, non a intuito. Ogni criterio ha un **peso** (quanto conta per te). Valuta ogni fornitore da **1 a 5**. Il totale ponderato dà un numero con cui confrontare. Compila una scorecard per fornitore, poi mettile fianco a fianco.

## Come assegnare i punteggi

- **Peso** = quanto è importante il criterio. I pesi sommano a 100. Cambiali per adattare al tuo business.
- **Punteggio** = da 1 (scarso) a 5 (eccellente) per quanto bene il fornitore lo soddisfa.
- **Punteggio ponderato** = peso × (punteggio ÷ 5). Questo tiene il totale su 100.

> **Punteggio ponderato = Peso × (Punteggio ÷ 5)**
> **Totale = somma di tutti i punteggi ponderati (su 100)**

## Scorecard vuota

**Fornitore:** ______________________  **Data:** ____________  **Valutato da:** ____________

| Criterio | Peso | Punteggio (1–5) | Punteggio ponderato | Note |
|---|---|---|---|---|
| Sicurezza | 20 |  |  |  |
| Privacy e conformità | 20 |  |  |  |
| Trasparenza | 10 |  |  |  |
| Prezzi | 15 |  |  |  |
| Supporto | 15 |  |  |  |
| Uscita e lock-in | 15 |  |  |  |
| Referenze e reputazione | 5 |  |  |  |
| **Totale** | **100** |  |  |  |

## Cosa significa ogni criterio

- **Sicurezza** — MFA, controllo degli accessi, registri di audit, avviso di violazione, protezione dagli attacchi.
- **Privacy e conformità** — Adattamento al GDPR, dati non usati per addestrare modelli condivisi, posizione dei dati, DPA offerto.
- **Trasparenza** — Risposte chiare, onesto sui limiti, aperto su sub-responsabili e cambiamenti del modello.
- **Prezzi** — Chiaro, prevedibile mentre cresci, senza costi nascosti, prezzo di rinnovo equo.
- **Supporto** — Canali reali, tempi di risposta scritti, onboarding, promessa di disponibilità.
- **Uscita e lock-in** — Recesso facile, esportazione dati in un formato utilizzabile, contratto iniziale corto, mantieni la proprietà.
- **Referenze e reputazione** — Recensioni o referenze da aziende come la tua, operatività abbastanza lunga da essere responsabile.

## Esempio compilato

**Fornitore:** InvoiceFlow AI (esempio)  **Data:** 2026-09-15  **Valutato da:** Titolare

| Criterio | Peso | Punteggio (1–5) | Punteggio ponderato | Note |
|---|---|---|---|---|
| Sicurezza | 20 | 4 | 16 | MFA sì, registri di audit sì, avviso di violazione 72 ore. |
| Privacy e conformità | 20 | 3 | 12 | DPA offerto, ma dati archiviati fuori UE — serve una verifica. |
| Trasparenza | 10 | 4 | 8 | Documenti chiari, onesto sui limiti. |
| Prezzi | 15 | 3 | 9 | Chiaro ora, ma il rinnovo sale del 40%. |
| Supporto | 15 | 5 | 15 | Chat 24/7, risposta in 2 ore, buon onboarding. |
| Uscita e lock-in | 15 | 2 | 6 | Esportazione CSV sì, ma lock-in di 12 mesi con costo. |
| Referenze e reputazione | 5 | 4 | 4 | Buone recensioni da aziende simili. |
| **Totale** | **100** |  | **70** | Buon prodotto, debole su uscita e posizione dei dati. |

**Leggere l'esempio:** 70/100 è un fornitore discreto con due problemi reali — la posizione dei dati (privacy) e un lock-in costoso (uscita). Il titolare non dovrebbe firmare il contratto di 12 mesi così com'è. Sistema i termini di uscita e conferma la posizione dei dati, oppure guarda altrove.

## Come leggere il totale

| Totale | Significato |
|---|---|
| 85–100 | Candidato forte. Passa a un pilota. |
| 70–84 | Buono, ma sistema prima le voci con punteggio basso. |
| 55–69 | Debole. Chiedi di più o guarda altrove. |
| Sotto 55 | Rifiuta. Troppe lacune. |

## La regola di priorità

Un totale alto può nascondere un difetto fatale. **Ignora il totale e allontanati se uno di questi vale 1:**

- **Sicurezza = 1** — Non possono proteggere i tuoi dati.
- **Privacy e conformità = 1** — Useranno male o tratteranno male i tuoi dati.
- **Uscita e lock-in = 1** — Non puoi riavere i tuoi dati o andartene.

Questi non sono compromessi. Un prezzo ottimo non sistema un fornitore che non ti lascia andare o che fa trapelare i tuoi dati.

## Confrontare due fornitori fianco a fianco

Metti insieme i totali e i segnalatori di priorità:

| Criterio | Fornitore A | Fornitore B |
|---|---|---|
| Totale (su 100) | 70 | 66 |
| Qualche segnalatore di priorità (Sic/Priv/Usc = 1)? | No | Sì (Usc = 1) |
| Decisione | Pilota ad A | Rifiuta B — non si può uscire |

Qui il Fornitore A vince anche su un piccolo divario di totale, perché il Fornitore B fallisce la regola di priorità.

## Consigli

- **Fissa i pesi prima di valutare.** Decidi prima cosa conta, così il punteggio non viene piegato per adattarsi a un fornitore che ti piace.
- **Valuta con prove**, non con il fascino. Usa le risposte dell'Appendice K e la checklist dell'Appendice B.
- **Valuta ogni fornitore allo stesso modo.** La coerenza è ciò che rende i totali confrontabili.
- **Rivaluta dopo la prova.** L'uso reale spesso cambia i numeri.
