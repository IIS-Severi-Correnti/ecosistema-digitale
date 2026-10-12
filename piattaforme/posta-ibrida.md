# Posta ibrida Gmail / Exchange Online

**Stato: TO-BE proposto, non implementato.**

## Esigenza

Docenti e studenti lavorerebbero in Gmail, integrato con Classroom e Drive; uffici e dirigenza conserverebbero Exchange/Outlook. Gli indirizzi istituzionali del dominio `severi-correnti.edu.it` dovrebbero restare invariati.

Le comunicazioni ufficiali tramite circolari sul sito e su ClasseViva sono **riferite** come processo già distinto dalla posta.

## Modello candidato

Instradamento per **destinatario effettivo** (split delivery), non per formato del nome email. Valutare con test un sistema MX di ingresso e la distribuzione all'altro provider. Progettare anche il flusso interno Exchange → Gmail per destinatari dello stesso dominio.

## Requisiti da validare

- Titolarità e configurazione DNS/MX e verifica dominio su entrambi i tenant.
- Directory destinatari, alias e caselle condivise; gestione degli indirizzi già esistenti.
- Routing reciproco senza loop né perdita di messaggi.
- SPF, DKIM e DMARC allineati alle sorgenti di invio autorizzate.
- Limiti e policy dei due provider, antispam e tracciabilità.
- Trattamento di allegati, liste, inoltri, calendari e notifiche.
- Migrazione e conservazione delle vecchie caselle; continuità e rollback.
- Test con messaggi interni/esterni, utenti inesistenti, risposte, bounce e distribuzioni.
- Valutazione protezione dati, licenze e responsabilità dei fornitori.

## Perché non inoltri individuali permanenti

Genererebbero due caselle da mantenere, possibilità di divergenza e dipendenze dalle policy di inoltro. Preferire il routing di dominio, **se validato**.

## Ordine raccomandato

Prototipo con account di test → misure di recapitabilità → approvazione → migrazione per piccoli gruppi → dismissione controllata delle caselle ridondanti.

Riferimenti da controllare in progettazione: documentazione ufficiale Google Workspace su *Split Delivery* e Microsoft Exchange Online su *Accepted Domains / Internal Relay*.
