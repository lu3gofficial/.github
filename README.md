# Standard GitHub LU3G

Questo repository e destinato a diventare il repository speciale `.github`
dell'organizzazione LU3G. Centralizza regole, template e controlli riutilizzabili
per i progetti aziendali senza contenere credenziali o dati di produzione.

## Principi

- repository privati per codice proprietario;
- un repository per prodotto o sito;
- pull request e CI prima del merge;
- ambienti `staging` e `production` separati;
- produzione approvata, tracciata e reversibile;
- database, upload, log, backup e segreti sempre fuori da Git.

La configurazione da applicare a ogni nuovo repository e descritta in
[`docs/REPOSITORY-STANDARD.md`](docs/REPOSITORY-STANDARD.md).
