# Pubblicazione della pagina illustrativa

Questa cartella contiene una **pagina statica, responsiva, senza dipendenze esterne** (HTML/CSS/JavaScript) con l'infografica dell'architettura candidata.

- `docs/index.html`: contenuto pubblico.
- `docs/assets/styles.css`: presentazione, layout responsive e stampa.
- `docs/assets/site.js`: pulsante di stampa.
- `docs/assets/sc-logo.png`: logo Severi-Correnti e favicon, derivato dall'immagine fornita per il progetto.
- `docs/assets/google-logo.jpg`: logo Google, derivato dall'immagine fornita per il progetto.
- `docs/assets/microsoft-logo.png`: logo Microsoft, derivato dall'immagine fornita per il progetto.
- `docs/assets/favicon.svg`: vecchia favicon non più utilizzata.

## Attivazione iniziale GitHub Pages (una tantum)

Un amministratore del repository deve aprire **Settings → Pages** e impostare:
1. **Source:** Deploy from a branch.
2. **Branch:** `main`.
3. **Folder:** `/docs`.
4. Premere **Save**.

L'indirizzo previsto è: <https://iis-severi-correnti.github.io/ecosistema-digitale/>.

La pubblicazione potrebbe richiedere qualche minuto. Da quel momento, i commit su `main` che modificano la cartella `docs/` aggiorneranno la pagina attraverso GitHub Pages.

## Aggiornamento dei contenuti

- La pagina illustra **TO-BE proposto**, non un'architettura approvata.
- Aggiornare insieme gli ADR e la documentazione corrispondente.
- Non aggiungere dati personali, infrastruttura sensibile o identificativi di account.
- Verificare su telefono e desktop, con tastiera e in stampa.
- La cartella `docs/` contiene anche altre note Markdown: la presenza di `.nojekyll` fa pubblicare i file statici senza una build Jekyll.

La modalità di pubblicazione tramite branch è descritta dalla [documentazione ufficiale GitHub](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Identità visuale

La pagina adotta la palette del logo scolastico: **arancione #F75F00** e **grigio #666666**, con sfondi bianchi e neutri. I loghi di Google e Microsoft sono riprodotti dai file forniti per il progetto, ottimizzati per la visualizzazione web e mantenuti cromaticamente distinti. Non sono inseriti servizi di font, immagini o analytics esterni.
