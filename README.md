# Gruppi di servizio

Programma dei gruppi di servizio della congregazione, con stampa per gli anziani e per la bacheca.

- **Sito**: https://lucioros.github.io/gruppiservizio/

## Come sono protetti i dati

I dati dei proclamatori stanno in `dati.json`, **cifrati** (AES-GCM, chiave ricavata dalla password con PBKDF2).
Senza la password il file è illeggibile, anche se il repository è pubblico.
Il token di GitHub che serve per salvare è anch'esso cifrato nello stesso file.

## File

| File | Cosa contiene |
|---|---|
| `index.html` | L'applicazione |
| `dati.json` | Dati cifrati (non modificarlo a mano) |
| `jspdf.umd.min.js` | Libreria jsPDF (MIT) per creare i PDF |
