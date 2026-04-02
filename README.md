# Cod reducere Kfea — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Kfea** de pe [shopilo.ro](https://shopilo.ro/magazin/kfea.ro). Returneaza **cupoane Kfea** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-kfea](https://shopilo-ro.github.io/cod-reducere-kfea/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-kfea
cd cod-reducere-kfea
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Kfea",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% reducere la mobila si decoratiuni",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/kfea.ro"
  }
]
```

## Cupoane Kfea disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 15% | 15% reducere la mobila si decoratiuni | [shopilo.ro](https://shopilo.ro/magazin/kfea.ro) |

Codurile active: **[shopilo.ro/magazin/kfea.ro](https://shopilo.ro/magazin/kfea.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Kfea?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/kfea.ro), adauga produsele in cos pe Kfea, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Kfea?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Kfea?
Pagina [shopilo.ro/magazin/kfea.ro](https://shopilo.ro/magazin/kfea.ro) este actualizata zilnic cu cele mai noi cod reducere Kfea, voucher Kfea si cupon promotional Kfea.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Kfea

Kfea este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/kfea.ro) cele mai bune cod reducere Kfea, cupoane Kfea verificate si voucher Kfea active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-kfea
```

```javascript
const { fetchCoupons } = require('cod-reducere-kfea');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
