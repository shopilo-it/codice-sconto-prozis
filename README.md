# Codice sconto Prozis, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Prozis** da [shopilo.it](https://shopilo.it/negozi/prozis.com). Restituisce **coupon Prozis** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-prozis](https://shopilo-it.github.io/codice-sconto-prozis/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-prozis
cd codice-sconto-prozis
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Prozis",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su nutrizione sportiva",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/prozis.com"
  }
]
```

## Coupon Prozis disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su nutrizione sportiva | [shopilo.it](https://shopilo.it/negozi/prozis.com) |

Codici attivi: **[shopilo.it/negozi/prozis.com](https://shopilo.it/negozi/prozis.com)**

## Domande frequenti

### Come utilizzo un codice sconto Prozis?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/prozis.com), aggiungi i prodotti al carrello su Prozis e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Prozis?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Prozis piu recenti?
La pagina [shopilo.it/negozi/prozis.com](https://shopilo.it/negozi/prozis.com) viene aggiornata quotidianamente con i codici sconto Prozis, voucher Prozis e coupon promozionali Prozis piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Prozis

Prozis e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/prozis.com) trovi i migliori codici sconto Prozis, coupon Prozis verificati e voucher Prozis attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-prozis
```

```javascript
const { fetchCoupons } = require('codice-sconto-prozis');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
