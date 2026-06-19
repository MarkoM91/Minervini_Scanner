# Minervini Scanner Pro v2

Updated BUY NOW logic based on your latest scan.

## Main changes

BUY NOW is now less rigid and more Minervini-style:

- RS >= 90
- VCPScore >= 70
- WeeklyTightnessScore >= 40
- DistanceFromPivot > -10%
- DistanceFromPivot <= 3%

READY:

- RS >= 88
- VCPScore >= 65
- DistanceFromPivot between -12% and +4%

Also added:

- Relative Volume calculation
- Relative Volume breakout boost
- Cleaner signal buckets
- Stronger focus on VCP + weekly tightness

## Run

```bash
pip install -r requirements.txt
python scanner_pro_v2.py
```

## Test

```bash
SCAN_LIMIT=300 python scanner_pro_v2.py
```

## Output

Inside `results/`:

- all_candidates.csv
- buy_now.csv
- ready.csv
- early_vcp.csv
- leaders.csv
- tradingview_watchlist.txt
- tradingview_buy_now.txt
