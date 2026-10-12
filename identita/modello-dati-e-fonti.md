# Modello minimo di identità e fonti

**Stato: proposta.** Il sistema amministrativo resta il riferimento per l'idoneità all'accesso; le piattaforme digitali sono destinatarie, non la fonte decisionale.

## Ruoli delle fonti

- **SIDI:** riferimento istituzionale per le informazioni ministeriali pertinenti.
- **Spaggiari:** ambiente operativo amministrativo da verificare come possibile fonte delle estrazioni necessarie.
- **Segreteria competente:** valida eventi, correzioni e discordie fra registri.
- **Google Workspace / Microsoft Entra:** rappresentano identità digitali, gruppi e abilitazioni.
- **Registro tecnico di riconciliazione (eventuale):** traccia collegamenti e stati minimi, non duplica inutilmente le anagrafiche.

**DA VALIDARE:** quali moduli Spaggiari siano attivi, le esportazioni disponibili, i diritti di accesso, formati e frequenza. Non presumere API SIDI/Spaggiari.

## Campi logici minimi (proposta, non esportazione reale)

| Campo | Scopo |
| --- | --- |
| `person_id` opaco e stabile | Legare cambi di classe, nome o email alla stessa persona |
| `tipo` | Studente, docente, ATA, esterno autorizzato |
| `stato_amministrativo` | Iscritto/in servizio, prossimo ingresso, cessato, da verificare |
| `decorrenza`, `fine_prevista` | Validità del rapporto, quando applicabile |
| `classe_ufficio` | Solo per assegnazioni necessarie |
| `mail_istituzionale` | Indirizzo comunicato all'utente, non chiave primaria |
| `provider_target` | Google, Microsoft o combinazione giustificata |
| `stato_sync`, `ultimo_esito` | Verifica e tracciabilità |

Non pubblicare il dataset reale. Non usare automaticamente codice fiscale, nome e cognome come chiave pubblica/tecnica se esiste un'alternativa meno invasiva.

## Regole di riconciliazione

- Prevedere omonimie, variazioni anagrafiche, rinnovi e casi di doppio ruolo.
- Se manca un identificatore o le fonti discordano: **eccezione**, non cancellazione.
- Ogni modifica proposta deve essere riproducibile e registrata.
- In caso di CSV vuoto, parziale o statisticamente anomalo: **stop e segnalazione**.
- Proteggere le esportazioni in un ambiente istituzionale autorizzato con accesso minimo e tempi di conservazione definiti.

## Prossime prove

Campioni **sintetici** per simulare ingressi, duplicati, rinnovi contratti, classi cambiate, trasferimenti, file corrotti e utenti assenti per errore.
