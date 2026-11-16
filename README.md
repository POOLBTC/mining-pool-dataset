# Mining pool dataset

Fees, payout schemes, minimum payouts and Stratum endpoints for 26 cryptocurrency mining pools, 21 of them mining Bitcoin. Maintained by [POOL BTC](https://pool-btc.com/), an independent site that compares mining pools. POOL BTC is not a pool and has no affiliation with BTC.com Pool or poolbtc.io.

Every row links to the pool page the figure came from and says when we last checked it. If a pool does not publish its fee, the field is empty. We do not fill it with an estimate.

## Files

- `pools.csv`: one row per pool
- `pools.json`: the same data plus metadata (`updated`, `count`, license)

## Columns

| Column | Meaning |
|---|---|
| `id`, `name`, `website` | Pool identifier, name, official site |
| `coins`, `btc`, `solo`, `algorithm` | Supported coins, whether it mines BTC, whether it offers solo mining, hash algorithms |
| `payout_scheme` | FPPS, PPS+, PPLNS and so on, as the pool lists them |
| `fee_percent` | Published fee for the default scheme, empty if not published |
| `min_payout` | Default payout threshold |
| `fee_source`, `fee_verified` | Page the fee came from and the date we checked it |
| `stratum`, `worker_format`, `stratum_source` | Connection endpoints, worker name format and where we found them |
| `note` | Caveats, such as terms that differ by hashrate |

Pools change their terms without notice. Check the fee and payout rules on the pool site before you point hardware at it.

## Web version

The table with a ranking by net BTC per day and a profitability calculator: https://pool-btc.com/dataset/en/ (Russian: https://pool-btc.com/dataset/ru/).

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You can reuse the data, including commercially, as long as you credit POOL BTC with a link to https://pool-btc.com/.

Found a wrong fee or a dead endpoint? Open an issue or write to support@pool-btc.com.
