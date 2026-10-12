# ADR-0002 — Google per la didattica e Microsoft per l'amministrazione

- **Data:** 2026-10-12
- **Stato:** proposto; non approvato
- **Ambito:** identità, posta e dispositivi

## Problema

Ridurre la complessità degli account e semplificare l'esperienza didattica, senza compromettere processi amministrativi e software specialistico.

## Opzioni da confrontare

1. Razionalizzare Microsoft 365 mantenendo un ecosistema prevalentemente unico.
2. Google Workspace per didattica + Microsoft 365 per amministrazione (**candidata**).
3. Convivenza estesa di entrambi i sistemi per tutti gli utenti.
4. Ulteriori combinazioni open source dove giustificate dai requisiti.

## Ipotesi candidata

Google Workspace (Gmail, Drive, Classroom) per studenti e docenti; Microsoft Entra/Exchange per segreterie e dirigenza; mantenimento di ClasseViva e sito per le circolari; ChromeOS Flex/Linux dove compatibili e Windows per amministrazione/laboratori specialistici; email sotto il dominio istituzionale con instradamento corretto.

## Motivazioni e rischi

**Benefici attesi:** ambiente didattico coerente, minore duplicazione delle caselle, processi amministrativi preservati, dispositivi potenzialmente più semplici.

**Rischi/limiti:** doppia governance, routing posta complesso, costi gestione ChromeOS, compatibilità LIM/CAD, sincronizzazione anagrafiche da verificare, conservazione e GDPR, formazione, continuità operativa.

## Condizioni per una decisione

Audit validato; requisiti delle segreterie; test email; prova dispositivi; costi complessivi; valutazioni legali/privacy; piano formazione e rollback; approvazione dei responsabili competenti.

**Nessuna migrazione o acquisto discende da questo ADR.**
