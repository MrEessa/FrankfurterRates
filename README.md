# Currency Watchlist

GBP, EUR, JPY, CHF, and AUD against USD - live rates with a 30-day change indicator. Plain HTML and vanilla JS. No framework, no build step. Open `index.html` and it works.

<img width="869" height="533" alt="{FBA0DE68-2F4A-403F-8AF6-A953C004CC12}" src="https://github.com/user-attachments/assets/b087b624-7339-47cc-b469-9a939aaa8781" />

## Stack

- HTML, CSS, vanilla JS
- [Frankfurter API](https://frankfurter.dev) - free, no API key
- `fetch` / `async/await` / `Promise.all` for parallel requests

## Run it

```bash
git clone https://github.com/your-username/currency-watchlist
cd currency-watchlist
open index.html
```

## Endpoints

| Endpoint | Purpose |
|---|---|
| `GET /latest` | Live rates |
| `GET /{date}` | Rates 30 days ago (for % change) |
| `GET /currencies` | Currency full names |

## Background

Learning project. I explored the API in Postman first, wrote an OpenAPI 3.0 spec for the three endpoints I needed, then built the UI against that contract. Slower than jumping straight into code, but I actually understood what I was consuming.
