# Architettura obiettivo candidata (TO-BE)

**Stato: TO-BE proposto, non approvato.** L'ipotesi favorisce semplicità d'uso nella didattica, continuità dei servizi amministrativi e riduzione delle duplicazioni.

## Separazione funzionale

| Popolazione | Identità/ambiente principale proposto | Posta | Dispositivi |
| --- | --- | --- | --- |
| Studenti | Google Workspace for Education | Gmail | ChromeOS Flex / Linux; Windows nei laboratori necessari |
| Docenti | Google Workspace for Education | Gmail | ChromeOS Flex nelle aule; dispositivi personali compatibili |
| Segreterie e dirigenza | Microsoft Entra / Microsoft 365 | Exchange Online | Windows |
| Supporto tecnico e casi misti | Modello di privilegi dedicato | Da definire caso per caso | Dipende dalla funzione |

Tutti potrebbero conservare l'attuale **dominio di posta istituzionale**. Ciò richiede verifica di dominio, licenze, instradamento, migrazione e policy.

## Schema logico

```text
     SIDI / Spaggiari (registrazioni amministrative)
                      |
             estrazioni autorizzate
                      |
      riconciliazione e controlli (da progettare)
                      |
               approvazioni / log
                 /          \
                /            \
     Google Workspace      Microsoft Entra
     didattica + Gmail     amministrazione + Exchange

     ClasseViva e sito istituzionale:
     canali delle circolari, indipendenti dalla posta
```

## Decisioni da non anticipare

- Non è ancora deciso che Google debba essere il sistema di ingresso MX: va studiato lo **split delivery** in entrambe le direzioni, con test.
- La migrazione Gmail richiede una politica di conservazione e un piano di ritorno; evitare inoltri individuali perpetui.
- ChromeOS Flex non equivale automaticamente a Chromebook gestito: verificare hardware, periferiche, costi di gestione e modalità d'esame.
- Laboratori Windows: valutare account temporanei/profili condivisi controllati, evitando credenziali permanenti comuni non tracciabili.
- Google Fundamentals e ChromeOS Education Upgrade hanno perimetri/licenze differenti: preventivo e verifica aggiornati necessari.
- SIDI e Spaggiari sono sistemi amministrativi: nessuna API o sincronizzazione specifica è stata finora validata.

## Criteri di scelta

Sicurezza e protezione dei dati; accessibilità e inclusione; qualità della posta; carico del team; continuità delle verifiche; compatibilità software; costo totale pluriennale; reversibilità; indipendenza da singole persone. Confrontare un progetto pilota con il miglioramento dell'attuale Microsoft 365 come scenario alternativo.

Vedi [ADR-0002](../decisioni/ADR-0002-architettura-ibrida-candidata.md) e [roadmap](roadmap.md).
