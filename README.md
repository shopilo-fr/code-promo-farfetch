# Code promo Farfetch, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Farfetch** depuis [shopilo.fr](https://shopilo.fr/reductions/farfetch.com). Renvoie les **coupons Farfetch** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-farfetch](https://shopilo-fr.github.io/code-promo-farfetch/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-farfetch
cd code-promo-farfetch
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Farfetch",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur la mode de luxe",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/farfetch.com"
  }
]
```

## Coupons Farfetch disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur la mode de luxe | [shopilo.fr](https://shopilo.fr/reductions/farfetch.com) |

Codes actifs : **[shopilo.fr/reductions/farfetch.com](https://shopilo.fr/reductions/farfetch.com)**

## Questions frequentes

### Comment utiliser un code promo Farfetch ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/farfetch.com), ajoutez les produits a votre panier sur Farfetch et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Farfetch ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Farfetch les plus recents ?
La page [shopilo.fr/reductions/farfetch.com](https://shopilo.fr/reductions/farfetch.com) est mise a jour quotidiennement avec les codes promo Farfetch, bons de reduction Farfetch et coupons promotionnels Farfetch les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Farfetch

Farfetch est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/farfetch.com), retrouvez les meilleurs codes promo Farfetch, coupons Farfetch verifies et bons de reduction Farfetch actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-farfetch
```

```javascript
const { fetchCoupons } = require('code-promo-farfetch');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
