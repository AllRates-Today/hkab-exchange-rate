# Hong Kong Association of Banks Exchange Rates API — hkab-exchange-rate

[![npm version](https://img.shields.io/npm/v/hkab-exchange-rate.svg)](https://www.npmjs.com/package/hkab-exchange-rate)
[![license](https://img.shields.io/npm/l/hkab-exchange-rate.svg)](https://github.com/AllRates-Today/hkab-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/hkab-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![USD/HKD today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fhkab%3Fsource%3DUSD%26target%3DHKD&query=%24.rate&label=USD%2FHKD%20published%20by%20Hong%20Kong%20Association%20of%20Banks&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/hkab/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fhkab%3Fsource%3DUSD%26target%3DHKD&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/hkab/)

**Official Hong Kong Association of Banks (Hong Kong) daily exchange rates for Node.js and TypeScript. The published bank association rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers Hong Kong Association of Banks itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official published rates** — Hong Kong Association of Banks's own table, with the publisher's own `rate_date` on every response
- 📅 **History from 2026** — this source publishes only its current table, so the archive builds forward from the day we started collecting
- 🔀 **Published vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number Hong Kong Association of Banks itself published, fixed once printed and carrying the bank association's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest published table

[![Latest Hong Kong Association of Banks table](https://allratestoday.com/api/open/central-bank/hkab/table.svg)](https://allratestoday.com/central-bank-rates-api/hkab/)

The image is rendered live from the keyless endpoint, so it follows the bank association's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the bank association publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-11-11 by Hong Kong Association of Banks — 66 rates, first 60 shown. Updated 2026-11-11.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| AUD | HKD | middle | 5.38775 |
| AUD | HKD | sell | 5.468 |
| AUD | HKD | tt_buy | 5.3075 |
| BND | HKD | middle | 6.12025 |
| BND | HKD | sell | 6.185 |
| BND | HKD | tt_buy | 6.0555 |
| CAD | HKD | middle | 5.52875 |
| CAD | HKD | sell | 5.61 |
| CAD | HKD | tt_buy | 5.4475 |
| CHF | HKD | middle | 9.50875 |
| CHF | HKD | sell | 9.5915 |
| CHF | HKD | tt_buy | 9.426 |
| CNY | HKD | middle | 1.176 |
| CNY | HKD | sell | 1.1885 |
| CNY | HKD | tt_buy | 1.1635 |
| DKK | HKD | middle | 1.17225 |
| DKK | HKD | sell | 1.187 |
| DKK | HKD | tt_buy | 1.1575 |
| EUR | HKD | middle | 8.76275 |
| EUR | HKD | sell | 8.8705 |
| EUR | HKD | tt_buy | 8.655 |
| GBP | HKD | middle | 10.47 |
| GBP | HKD | sell | 10.55 |
| GBP | HKD | tt_buy | 10.39 |
| INR | HKD | middle | 0.08375 |
| INR | HKD | sell | 0.0905 |
| INR | HKD | tt_buy | 0.077 |
| JPY | HKD | middle | 0.0494275 |
| JPY | HKD | sell | 0.05043 |
| JPY | HKD | tt_buy | 0.048425 |
| KRW | HKD | middle | 0.0058425 |
| KRW | HKD | sell | 0.006095 |
| KRW | HKD | tt_buy | 0.00559 |
| MYR | HKD | middle | 1.93425 |
| MYR | HKD | sell | 1.9605 |
| MYR | HKD | tt_buy | 1.908 |
| NOK | HKD | middle | 0.82525 |
| NOK | HKD | sell | 0.839 |
| NOK | HKD | tt_buy | 0.8115 |
| NZD | HKD | middle | 4.39675 |
| NZD | HKD | sell | 4.46 |
| NZD | HKD | tt_buy | 4.3335 |
| PHP | HKD | middle | 0.12475 |
| PHP | HKD | sell | 0.129 |
| PHP | HKD | tt_buy | 0.1205 |
| PKR | HKD | middle | 0.02825 |
| PKR | HKD | sell | 0.031 |
| PKR | HKD | tt_buy | 0.0255 |
| SEK | HKD | middle | 0.79525 |
| SEK | HKD | sell | 0.808 |
| SEK | HKD | tt_buy | 0.7825 |
| SGD | HKD | middle | 6.12025 |
| SGD | HKD | sell | 6.1825 |
| SGD | HKD | tt_buy | 6.058 |
| THB | HKD | middle | 0.2335 |
| THB | HKD | sell | 0.237 |
| THB | HKD | tt_buy | 0.23 |
| TWD | HKD | middle | 0.23775 |
| TWD | HKD | sell | 0.2415 |
| TWD | HKD | tt_buy | 0.234 |

</details>

[Full table on the Hong Kong Association of Banks rates page](https://allratestoday.com/central-bank-rates-api/hkab/) · Source: [Official rates published by HKAB, served by AllRatesToday](https://allratestoday.com/central-bank-rates-api/hkab/). Rates are as printed by the bank association; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install hkab-exchange-rate
```

```bash
yarn add hkab-exchange-rate
```

```bash
pnpm add hkab-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/hkab-exchange-rate`](https://www.npmjs.com/package/@allratestoday/hkab-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'hkab-exchange-rate';

const pair = await getRate('USD', 'HKD', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official Hong Kong Association of Banks rate, on the bank association's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest published table
- [Full published table](#full-published-table) — everything the bank association printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the bank association does not print directly are resolved from its table and flagged (see *Published vs derived rates* below).

```js
const pair = await getRate('USD', 'HKD', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'hkab',
  name: 'Hong Kong Association of Banks',
  rate_date: '2026-11-06',   // Hong Kong Association of Banks's own publication date
  source: 'USD',
  target: 'HKD',
  rate: 7.8415,
  rate_type: 'middle',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full published table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'hkab-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'hkab',
  name: 'Hong Kong Association of Banks',
  rate_date: '2026-11-06',
  rates: [
    { "base": "EUR", "quote": "HKD", "type": "middle", "value": 8.80225 },
    { "base": "EUR", "quote": "HKD", "type": "sell", "value": 8.91 },
    { "base": "EUR", "quote": "HKD", "type": "tt_buy", "value": 8.6945 },
    { "base": "USD", "quote": "HKD", "type": "middle", "value": 7.8415 },
    // … the rest of the published table (22 currencies vs HKD)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2026 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'hkab-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'HKD' });
```

**Response:**

```javascript
{
  bank: 'hkab',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'hkab-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'HKD', from: '2026-01-01', to: '2026-11-06' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'hkab',
  source: 'USD',
  target: 'HKD',
  from: '2026-01-01',
  to: '2026-11-06',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-11-06', rate: 7.8415, rate_type: 'middle', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

Hong Kong Association of Banks currently publishes rates covering **22 currencies** against the HKD (as of the latest table):

🇦🇺 `AUD` · 🇧🇳 `BND` · 🇨🇦 `CAD` · 🇨🇭 `CHF` · 🇨🇳 `CNY` · 🇩🇰 `DKK` · 🇪🇺 `EUR` · 🇬🇧 `GBP` · 🇮🇳 `INR` · 🇯🇵 `JPY` · 🇰🇷 `KRW` · 🇲🇾 `MYR` · 🇳🇴 `NOK` · 🇳🇿 `NZD` · 🇵🇭 `PHP` · 🇵🇰 `PKR` · 🇸🇪 `SEK` · 🇸🇬 `SGD` · 🇹🇭 `THB` · 🇹🇼 `TWD` · 🇺🇸 `USD` · 🇿🇦 `ZAR`

## 🏛️ Source

Hong Kong Association of Banks is the monetary authority of Hong Kong.

- Publisher's own page: [Exchange rates](https://www.hkab.org.hk/en/rates/exchange-rates)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [Hong Kong Association of Banks rates page](https://allratestoday.com/central-bank-rates-api/hkab/)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- HKAB prints **Hong Kong dollars per 1 unit of foreign currency** (`base: "USD", quote: "HKD"`), with `sell` and `tt_buy` opening counter rates and a computed `middle` of the two.
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the bank association's series a row belongs to (`middle` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official Hong Kong Association of Banks rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/hkab/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('hkab')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate hkab ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Published vs derived rates

If Hong Kong Association of Banks does not print a pair directly, the API resolves it from the bank association's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The bank association printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via HKD from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by Hong Kong Association of Banks |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'hkab-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('hkab-exchange-rate');

getRate('USD', 'HKD', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the published table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the published table |
| `getLatestRates({ apiKey })` | Free | The bank association's full latest published table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2026 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same published tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/hkab.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/hkab/latest.json`

## 🔗 Links

- **Website:** [allratestoday.com](https://allratestoday.com)
- [Hong Kong Association of Banks rates page](https://allratestoday.com/central-bank-rates-api/hkab/) — live table, publication cadence, FAQ
- [All central bank sources](https://allratestoday.com/central-bank-rates-api/)
- [Download central bank rates](https://allratestoday.com/download-central-bank-rates/) — every bank's latest table and history as Excel, CSV or JSON
- [Package docs on the site](https://allratestoday.com/docs/sdk/hkab-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [ChatGPT app](https://chatgpt.com/plugins/plugin_asdk_app_6ae1e76098f48191a285ac3f5ab7a83b) — ask ChatGPT for live and official central bank rates
- [OpenAPI reference on Bump.sh](https://bump.sh/allratestoday/doc/allratestoday-api) — also on [SwaggerHub](https://app.swaggerhub.com/apis-docs/allratestoday/allratestoday-exchange-rate-central-bank-rates-api/2.2.0)
- [GitHub](https://github.com/AllRates-Today/hkab-exchange-rate)

## 📜 License

MIT
