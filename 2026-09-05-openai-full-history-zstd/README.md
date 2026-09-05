# 2026-09-05 Pair Collector Snapshot

Frozen snapshot of the `systemd --user` collect-only stream for:

- `io:OAI|binance:OPENAIUSDT`

CSV compression: `zstd`.

Source files at snapshot time:

- `exports/pair_collectors/systemd/io_OAI__binance_OPENAIUSDT/market_data.csv`
- `exports/pair_collectors/systemd/io_OAI__binance_OPENAIUSDT/collector_events.csv`
- `exports/pair_collectors/systemd/io_OAI__binance_OPENAIUSDT/collector_fills.csv`

Snapshot coverage:

- `io:OAI|binance:OPENAIUSDT` through `2026-09-05T15:27:25.751Z`

Files:

- `io_OAI__binance_OPENAIUSDT_market_data.csv.zst`
- `io_OAI__binance_OPENAIUSDT_collector_events.csv.zst`
- `io_OAI__binance_OPENAIUSDT_collector_fills.csv.zst`
- `summary.json`

Quick read:

- `io:OAI|binance:OPENAIUSDT`: `487301` rows, `20160` clean rows, `20160` clean rows with `best_edge_bps >= 10`
- Event mix: `20160` clean snapshots, `429587` stale snapshots, `37554` desynced snapshots
- Freshness: target fresh `20.1245%`, reference fresh `58.7224%`, synchronized `6.8089%`, fully clean `4.1371%`

Clean rows are those where:

- `target_book_is_fresh == true`
- `reference_book_is_fresh == true`
- `pair_is_synchronized == true`
- `event == snapshot`
