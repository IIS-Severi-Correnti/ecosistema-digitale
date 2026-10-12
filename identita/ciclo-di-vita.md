# Ciclo di vita delle identità (Joiner / Mover / Leaver)

**Stato: processo proposto da validare con segreterie, amministratori e responsabili.**

| Evento | Innesco autorevole | Azione tecnica proposta | Controllo |
| --- | --- | --- | --- |
| Nuova iscrizione | Iscrizione confermata | Preparare account e gruppo classe | Convalida dati e collisioni |
| Presa di servizio | Rapporto registrato | Preparare identità e ruolo autorizzato | Decorrenza e necessità operativa |
| Cambio classe/ruolo | Variazione convalidata | Aggiornare gruppi e privilegi | Rimuovere permessi non più dovuti |
| Proroga supplenza | Proroga registrata | Aggiornare scadenza prevista | Nessuna revoca prematura |
| Trasferimento/ritiro | Evento amministrativo confermato | Valutare sospensione e conservazione | Approvazione e comunicazioni |
| Diploma/cessazione | Conclusione effettiva | Disattivare secondo policy differenziata | Esami, recuperi, documenti, deleghe |
| Accesso esterno | Sponsorizzazione nominativa | Accesso limitato e a termine | Revisione periodica |

## Stati proposti

`DA_VERIFICARE → APPROVATO → ATTIVO → IN_REVISIONE → SOSPESO → ARCHIVIATO/ELIMINATO`

La scelta finale di conservazione e rimozione va determinata secondo gli obblighi applicabili e le caratteristiche dei servizi.

## Principi tecnici

- Modifiche **idempotenti**, verificabili e ripetibili.
- Dry-run con variazioni proposte prima delle modifiche.
- Soglie d'allarme per diminuzioni improvvise e cambi massivi.
- Log minimo con evento, operatore/processo, esito e timestamp; protezione dei log.
- Le eliminazioni definitive non sono una conseguenza automatica del semplice mancato riscontro.
- Prevedere override eccezionali documentati, con responsabile e data di revisione.
- Privilegi amministrativi separati dalle identità d'uso quotidiano.

Vedi [onboarding](../processi/onboarding.md), [offboarding](../processi/offboarding.md) e [manutenzione](../processi/manutenzione-annuale.md).
