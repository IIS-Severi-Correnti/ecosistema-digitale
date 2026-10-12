# Ecosistema digitale — IIS Severi-Correnti

Progetto collaborativo per **documentare, valutare e migliorare** architettura informatica, identità, piattaforme, dispositivi e processi dell'istituto.

> **Stato: proposta di lavoro del team digitale (12 ottobre 2026).** Questo repository non costituisce un atto di approvazione della scuola, non autorizza modifiche agli ambienti di produzione e non sostituisce le procedure istituzionali.

## Perché esiste

Rendere l'ecosistema scolastico comprensibile, sostenibile e documentato nel tempo. Il punto di partenza è un audit preliminare della directory Microsoft 365, ma il perimetro include l'infrastruttura digitale nel suo complesso.

## Come leggere i documenti

Ogni affermazione significativa va classificata come:
- **AS-IS verificato**: osservato o documentato, con fonte e data;
- **AS-IS riferito**: comunicato da soggetti coinvolti, da verificare tecnicamente;
- **TO-BE proposto**: opzione progettuale, non decisione approvata;
- **DA VALIDARE**: ipotesi, lacuna o requisito ancora aperto;
- **DECISO**: scelta approvata dall'autorità competente, con riferimento all'atto o all'esito formalizzato.

Gli [ADR](decisioni/README.md) registrano il ragionamento sulle scelte. Un ADR proposto non equivale a una delibera.

## Mappa del repository

| Area | Scopo |
| --- | --- |
| [architettura](architettura/stato-attuale.md) | Stato attuale, scenario obiettivo e roadmap |
| [audit](audit/audit-microsoft-2026.md) | Sintesi aggregata e limiti metodologici dell'audit Microsoft |
| [identita](identita/modello-dati-e-fonti.md) | Fonte amministrativa, dati minimi e ciclo di vita |
| [processi](processi/onboarding.md) | Ingressi, cambiamenti, uscite e manutenzione |
| [piattaforme](piattaforme/posta-ibrida.md) | Posta e ambienti applicativi |
| [dispositivi](dispositivi/strategia-postazioni.md) | Postazioni didattiche, uffici e laboratori |
| [governance](governance/ruoli-e-responsabilita.md) | Ruoli, autorizzazioni e controlli |
| [decisioni](decisioni/README.md) | Architecture Decision Records |
| [docs/questioni-aperte.md](docs/questioni-aperte.md) | Questioni da accertare con i referenti |

## Percorso iniziale

1. Validare la fotografia dell'AS-IS con team digitale, segreterie e responsabili.
2. Confrontare le anagrafiche amministrative autorizzate con gli account Microsoft.
3. Definire un processo di ciclo di vita ripetibile, senza cancellazioni automatiche.
4. Sperimentare Google Workspace e dispositivi alternativi in un perimetro pilota.
5. Misurare costi, sicurezza, usabilità e lavoro amministrativo; solo dopo decidere eventuali migrazioni.

Vedi la [roadmap](architettura/roadmap.md).

## Contribuire

Aprire una **Issue** per problemi o domande, una **Pull Request** per modifiche alla documentazione. Leggere [CONTRIBUTING.md](CONTRIBUTING.md), [AGENTS.md](AGENTS.md) e [SECURITY.md](SECURITY.md).

**Mai pubblicare** elenchi nominativi, CSV delle anagrafiche, password, token, indirizzi interni sensibili, esportazioni amministrative o rapporti riservati. La natura pubblica di questo repository non autorizza a pubblicare dati della scuola.

## Stato del progetto

Versione documentale iniziale **v0.1**, 12/10/2026. Contenuti predisposti per discussione e revisione; nessun intervento sulle piattaforme è implicito.

La licenza di riutilizzo dei contenuti non è stata ancora scelta dall'istituto: il repository pubblico è consultabile, ma il riuso resta da disciplinare.
