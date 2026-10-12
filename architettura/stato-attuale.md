# Stato attuale (AS-IS) — fotografia preliminare

**Data di riferimento: 12 ottobre 2026.** Le informazioni seguono due livelli: descrizioni riferite dal team e aggregati tratti da un audit preliminare; non costituiscono collaudo tecnico dell'infrastruttura.

## Servizi e utilizzi riferiti

| Ambito | Situazione riferita | Stato |
| --- | --- | --- |
| Identità e collaborazione | Microsoft 365 / Entra per docenti, studenti, amministrazione e dirigenza | AS-IS riferito |
| Postazioni d'istituto | Windows con accesso organizzativo e ambienti utente associati | AS-IS riferito; join Entra/AD locale da verificare |
| Posta istituzionale | Dominio comune `severi-correnti.edu.it`, attualmente in ambito Microsoft | AS-IS riferito |
| Nomenclatura email | Per gli studenti tipicamente `nome.cognome@`; per i docenti `cognome@` | AS-IS riferito; eccezioni/collisioni da verificare |
| Registro e circolari | ClasseViva (Spaggiari) e sito istituzionale come canali delle comunicazioni ufficiali | AS-IS riferito; verificare prassi e policy |
| Gestione amministrativa | Spaggiari e SIDI | AS-IS riferito; moduli, API, esportazioni e responsabilità da verificare |
| Dispositivi | Aule, laboratori, carrelli e postazioni amministrative | AS-IS riferito; inventario da consolidare |

## Prima criticità

La directory Microsoft appare sovradimensionata rispetto agli utenti correnti. L'[audit preliminare](../audit/audit-microsoft-2026.md) quantifica il fenomeno, ma **non** dispone del campo di ultimo accesso e non prova l'inattività dei singoli utenti.

## Elementi non ancora verificati

- Topologia di Entra ID, eventuale Active Directory locale, join e profili Windows.
- Tipi di account, licenze, domini verificati, alias, gruppi e deleghe.
- Numeri effettivi di studenti iscritti, docenti e personale in servizio.
- Flussi di comunicazione segreterie → docenti e gruppi istituzionali.
- Integrazioni effettivamente disponibili tra Spaggiari, SIDI e piattaforme cloud.
- Inventario dei computer e compatibilità con software specialistico e LIM.

Per assegnare lo stato **AS-IS verificato**, ogni punto richiede evidenza e data di riscontro, raccolte nei sistemi autorizzati.
