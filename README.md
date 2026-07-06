# COPPER 5m OHLCV Commodities Historical Data — Free Sample

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Dataset rows](https://img.shields.io/badge/full_dataset-1_019_827_rows-blue)](https://ork.ad/) [![Updated](https://img.shields.io/badge/weekly_update-every_Sunday-green)](https://ork.ad/) [![Full data on ork.ad](https://img.shields.io/badge/download-ork.ad-orange)](https://ork.ad/)

### → [**Download the full COPPER dataset on ork.ad**](https://ork.ad/)

**COPPER 5m OHLCV Commodities historical data** — ultra high-quality 5m OHLCV for **Copper**. Extended-session energy and industrial metals — beyond US cash hours. Clean `time, open, high, low, close, volume` CSV for backtesting, algorithmic trading and quantitative research.

## Table of contents

- [Why this dataset?](#why-this-dataset)
- [Download sample CSV](#download-sample)
- [GitHub Pages preview](#github-pages)
- [Sample vs full dataset](#sample-vs-full-dataset)
- [Timeframes on ork.ad](#timeframes-on-orkad)
- [Weekly updates](#weekly-updates)
- [Data preview](#data-preview)
- [Schema](#schema)
- [Code examples](#code-examples)
- [Download full data on ork.ad](#download-full-data)

## Why this dataset?

- **Ultra high-quality 5m OHLCV** for **Copper** (Commodities)
- **Extended-session energy and industrial metals — beyond US cash hours**
- **Clean CSV schema** — `time, open, high, low, close, volume` (no gaps in formatting)
- **Free evaluation sample** on GitHub (`5m`) · **13 timeframes** on [ork.ad](https://ork.ad/) · **1,019,827** `5m` rows in the full archive
- Built for **backtesting**, **algorithmic trading** and **quantitative finance** workflows
- **Weekly refresh** — [ork.ad](https://ork.ad/) every **Sunday**; GitHub `5m` sample updated in sync

> **Sample on GitHub** · `COPPER_5m.csv` (35,335 rows, `2026-01-04` → `2026-07-03`). **Full archive on [ork.ad](https://ork.ad/)** — **1,019,827** `5m` rows (~48.96 MB), **13 timeframes** (``1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W``), `2011-08-28` → `2026-07-03`.

## Download sample

**[COPPER_5m.csv](https://github.com/ork-ad/copper-5m-ohlcv-commodities-historical-data/blob/main/COPPER_5m.csv)** on GitHub ([raw CSV](https://raw.githubusercontent.com/ork-ad/copper-5m-ohlcv-commodities-historical-data/main/COPPER_5m.csv)) · [GitHub Releases](https://github.com/ork-ad/copper-5m-ohlcv-commodities-historical-data/releases) when the release workflow is active.

## GitHub Pages

Interactive chart & stats: **[https://ork-ad.github.io/copper-5m-ohlcv-commodities-historical-data/](https://ork-ad.github.io/copper-5m-ohlcv-commodities-historical-data/)**

## Sample vs full dataset

| | **Sample (this repo)** | **Full dataset ([ork.ad](https://ork.ad/))** |
|---|--:|---|
| Instrument | Copper · Commodities | Copper · Commodities |
| Timeframes | `5m` (sample) | **13** — `1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W` |
| 5m rows | 35,335 | **1,019,827** |
| Size | 1.75 MB | ~48.96 MB |
| Period | `2026-01-04` → `2026-07-03` | `2011-08-28` → `2026-07-03` |
| File | `COPPER_5m.csv` | ZIP on [ork.ad](https://ork.ad/) |
| Updates | Weekly (Sunday) — GitHub sample | Weekly (Sunday) — all timeframes |

## Timeframes on ork.ad

This GitHub repository ships a **`5m` evaluation sample** only. On **[ork.ad](https://ork.ad/)**, each full asset archive is delivered as a ZIP with **13 gap-free OHLCV timeframes** (one CSV per timeframe):

**1m** · **3m** · **5m** · **15m** · **30m** · **1H** · **2H** · **4H** · **8H** · **12H** · **16H** · **1D** · **1W**

GitHub = `5m` sample · [ork.ad](https://ork.ad/) = all **13** timeframes above for the same instrument.

## Weekly updates

- **[ork.ad](https://ork.ad/)** — Full datasets on ork.ad are updated every Sunday.
- **GitHub (this repo)** — GitHub samples are refreshed weekly (every Sunday), in sync with ork.ad.

When a new `5m` sample is published on GitHub, the README, chart preview and CSV reflect the latest week of data.

## Data preview

First and latest rows from the GitHub sample **`COPPER_5m.csv`**:

**First rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| 2026-01-04T23:00:00Z | 5.702 | 5.7222 | 5.702 | 5.7222 | 156 |
| 2026-01-04T23:05:00Z | 5.7222 | 5.7282 | 5.6974 | 5.7043 | 167 |
| 2026-01-04T23:10:00Z | 5.7043 | 5.7122 | 5.7041 | 5.709 | 94 |
| 2026-01-04T23:15:00Z | 5.709 | 5.712 | 5.7049 | 5.707 | 127 |
| 2026-01-04T23:20:00Z | 5.707 | 5.7123 | 5.707 | 5.7105 | 105 |

**Last rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| time | open | high | low | close | volume |
| 2026-07-03T16:35:00Z | 6.2161 | 6.2169 | 6.2155 | 6.217 | 50 |
| 2026-07-03T16:40:00Z | 6.217 | 6.2204 | 6.2165 | 6.2199 | 59 |
| 2026-07-03T16:45:00Z | 6.2199 | 6.2221 | 6.2199 | 6.2209 | 73 |
| 2026-07-03T16:50:00Z | 6.2209 | 6.2243 | 6.2203 | 6.224 | 58 |

## Schema

```text
time,open,high,low,close,volume
```

## Code examples

### pandas

```python
import pandas as pd

df = pd.read_csv('COPPER_5m.csv', parse_dates=['time'])
df.set_index('time', inplace=True)
print(df.describe())
print(df.resample('1h').agg({'open': 'first', 'high': 'max',
                              'low': 'min', 'close': 'last', 'volume': 'sum'}).head())
```

### backtrader

```python
import backtrader as bt
import pandas as pd

df = pd.read_csv('COPPER_5m.csv', parse_dates=['time'])
df.set_index('time', inplace=True)

class PandasData(bt.feeds.PandasData):
    params = (('datetime', None), ('open', 'open'), ('high', 'high'),
              ('low', 'low'), ('close', 'close'), ('volume', 'volume'))

cerebro = bt.Cerebro()
cerebro.adddata(PandasData(dataname=df))
# cerebro.addstrategy(YourStrategy)
# cerebro.run()
```

### vectorbt

```python
import pandas as pd
import vectorbt as vbt

df = pd.read_csv('COPPER_5m.csv', parse_dates=['time'])
close = df.set_index('time')['close']
fast, slow = vbt.MA.run(close, 10), vbt.MA.run(close, 50)
entries = fast.ma_crossed_above(slow)
exits = fast.ma_crossed_below(slow)
pf = vbt.Portfolio.from_signals(close, entries, exits, init_cash=10_000, freq='5min')
print(pf.stats())
```

## Download full data

The complete **COPPER** archive on **[ork.ad](https://ork.ad/)** includes **13 OHLCV timeframes** (`1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W`) — **1,019,827** rows at `5m`, plus all other timeframes in the same ZIP.

**[→ Get the full COPPER dataset on ork.ad](https://ork.ad/)**

---
*GetData · COPPER 5m OHLCV sample on GitHub · Full historical data on [ork.ad](https://ork.ad/) · 2026-07-06 UTC*