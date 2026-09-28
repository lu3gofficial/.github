# Standard repository LU3G

## Creazione

1. Repository privato nell'organizzazione LU3G.
2. Nome breve e stabile, senza riferimenti al server.
3. `main` e lo stato distribuibile; `staging` precede la produzione.
4. File runtime, dati e segreti non entrano mai nella cronologia Git.
5. Attivare secret scanning, push protection e Dependabot.

## Ruleset `main`

- pull request obbligatoria;
- almeno una approvazione quando il team avra piu revisori;
- conversazioni risolte e controlli CI superati;
- branch aggiornato prima del merge;
- force push e cancellazione vietati;
- bypass limitato al proprietario per sole emergenze documentate.

## Ambienti

### Staging

- dati sintetici o anonimizzati;
- deploy dopo CI;
- smoke test, ruoli, desktop e mobile prima del merge in `main`.

### Production

- approvazione manuale;
- backup e rollback disponibili;
- segreti separati da staging;
- deploy con chiave dedicata al singolo repository;
- readback degli hash e smoke test senza effetti commerciali.

## Permessi

- proprietari dell'organizzazione: minimo numero possibile;
- collaboratori: accesso al solo repository necessario;
- server: chiave di sola distribuzione, mai credenziali personali;
- automazioni: permessi GitHub minimi dichiarati nel workflow.

## Nuovo progetto

- [ ] `README`, `SECURITY`, `CONTRIBUTING` e `.gitignore`
- [ ] CI con test, build e controllo segreti
- [ ] Dependabot per gli ecosistemi usati
- [ ] ruleset di `main` e branch `staging`
- [ ] ambienti e approvazione produzione
- [ ] backup, rollback e runbook di deploy
- [ ] proprietario tecnico e dati esclusi documentati
