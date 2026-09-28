# Sicurezza LU3G

Non aprire issue pubbliche per vulnerabilita o possibili fughe di dati.
Invia una segnalazione privata a `giordano.vinci@lu3g.it` con impatto,
componente e riproduzione minima priva di dati reali.

## Requisiti minimi

- autenticazione a due fattori per i membri dell'organizzazione;
- segreti conservati negli ambienti GitHub o nel vault del server;
- chiavi di deploy dedicate, revocabili e con privilegi minimi;
- protezione di `main` e divieto di force push;
- backup e prove di ripristino indipendenti da GitHub;
- revisione delle dipendenze e secret scanning per ogni repository.
