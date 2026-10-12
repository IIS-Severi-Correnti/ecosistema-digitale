# Audit preliminare Microsoft 365 — sintesi aggregata

**Fonte:** analisi documentale di esportazione utenti dell'11 ottobre 2026, condivisa per la progettazione; il CSV nominativo e il rapporto originale non sono pubblicati qui. **Stato: osservazione preliminare da validare.**

## Dati aggregati riportati

| Voce | Quantità |
| --- | ---: |
| Account totali | 6.954 |
| Classificati come studenti | 3.324 |
| Classificati come genitori | 2.323 |
| Classificati come docenti | 232 |
| Account Guest esterni | 288 |
| Account classificati come risorse | 69 |
| Account senza licenza (indicatore trasversale) | 2.620 |
| Studenti associati ad annualità precedenti (sottoinsieme potenziale) | almeno 1.515 |

### Attenzione all'interpretazione

- L'esportazione **non contiene l'ultimo accesso**: non si può inferire la reale inattività.
- La classificazione deriva dagli attributi disponibili; può contenere errori e categorie sovrapposte.
- Gli account senza licenza e gli studenti di annualità precedenti **non** sono categorie additive.
- I 6.954 non sono il numero degli utenti che hanno diritto attuale a un account.
- L'eventuale differenza aritmetica tra somme delle categorie e totale non prova l'esistenza di una precisa classe residuale, se non si dimostra la mutua esclusività.
- I 1.515 studenti storici non possono essere automaticamente considerati ex studenti.

## Verifiche necessarie prima di agire

1. Confrontare dati di segreteria autorizzati con identità Microsoft mediante ID affidabile.
2. Validare ruolo, appartenenza, data di servizio/iscrizione, eccezioni e necessità dell'account.
3. Esaminare accessi riusciti dove tecnicamente e giuridicamente consentito; verificare gruppi, posta, OneDrive, condivisioni e dipendenze.
4. Distinguere **blocco accesso**, **rimozione licenza** ed **eliminazione**, con conseguenze e tempi di recupero diversi.
5. Definire per ogni tipologia: responsabile, autorizzazione, conservazione dati, eccezioni e procedura di ripristino.

**Nessun elenco nominativo o dato tecnico sensibile deve essere ricostruito, caricato o pubblicato in questo repository.**

## Esito attuale

L'audit giustifica un progetto di riconciliazione e governance delle identità. **Non autorizza un'operazione massiva di cancellazione.**
