# Codice sconto Farfetch, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Farfetch** da [shopilo.it](https://shopilo.it/negozi/farfetch.com). Restituisce **coupon Farfetch** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-farfetch](https://shopilo-it.github.io/codice-sconto-farfetch/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-farfetch
cd codice-sconto-farfetch
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Farfetch",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su moda di lusso",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/farfetch.com"
  }
]
```

## Coupon Farfetch disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su moda di lusso | [shopilo.it](https://shopilo.it/negozi/farfetch.com) |

Codici attivi: **[shopilo.it/negozi/farfetch.com](https://shopilo.it/negozi/farfetch.com)**

## Domande frequenti

### Come utilizzo un codice sconto Farfetch?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/farfetch.com), aggiungi i prodotti al carrello su Farfetch e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Farfetch?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Farfetch piu recenti?
La pagina [shopilo.it/negozi/farfetch.com](https://shopilo.it/negozi/farfetch.com) viene aggiornata quotidianamente con i codici sconto Farfetch, voucher Farfetch e coupon promozionali Farfetch piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Farfetch

Farfetch e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/farfetch.com) trovi i migliori codici sconto Farfetch, coupon Farfetch verificati e voucher Farfetch attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-farfetch
```

```javascript
const { fetchCoupons } = require('codice-sconto-farfetch');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
