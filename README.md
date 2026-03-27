# Momentum + Smart Money Concepts — First-Hour Trading System

A structured, step-by-step daily trading flowchart combining **momentum trading principles** with **Smart Money Concepts (SMC)** from the LuxAlgo indicator on TradingView. Designed specifically for trading high-momentum *stocks in play* during the **first 1–2 hours of market open**.

---

## What This Is

This flowchart is a visual trading framework — not a signal bot, not a strategy backtester. It is a **decision-making reference** that walks you through every phase of the trading day in order:

1. Pre-market preparation and stock screening
2. Reading the first minutes of market open
3. Identifying SMC signals in real time
4. Executing long (buy) and short (sell) setups
5. Managing the trade once you're in

It is built for traders who already understand the basics of reading charts and want a repeatable, disciplined process for finding and executing momentum setups with institutional-grade entry precision.

---

## Files Included

| File | Description |
|---|---|
| `momentum_smc_trading_flowchart.html` | The interactive flowchart — open in any browser |
| `README.md` | This file |

---

## How to Use the Flowchart

Open `momentum_smc_trading_flowchart.html` in any modern browser (Chrome, Safari, Firefox, Edge). No internet connection required. No installations. Works on desktop and mobile.

The flowchart is colour-coded by phase:

- **Blue** — Pre-market prep and SMC signal detection
- **Amber/Yellow** — Market open and price discovery (caution zone)
- **Green** — Long (buy) setup conditions
- **Red** — Short (sell) setup conditions
- **Neutral/Grey** — Trade management rules

Work through it **top to bottom**, every single trading day, in order. Skipping phases is how losing trades happen.

---

## The Four Phases Explained

### Phase 1 — Pre-Market Prep (6:00 AM – 9:29 AM EST)

Before the bell, you are building a watchlist of *stocks in play*. A stock in play has:

- A meaningful gap (ideally 10%+) driven by a **real catalyst** — earnings beat, FDA approval, merger news, short squeeze. A gap with no catalyst is a trap.
- A **low float** (under 20M shares preferred). Low float means fewer shares available, which means price moves faster and further when volume hits.
- Strong **pre-market volume** (500K+ shares) confirming institutional and retail interest is already building.
- An **ATR (Average True Range)** of at least $0.50. ATR tells you the stock's average daily range — this is what you use to set your stop distance and your profit targets before you ever enter a trade.

During this phase, you also **mark your chart** with key SMC levels from the LuxAlgo script:
- Previous day high and low
- Overnight high and low
- Any open Order Blocks or Fair Value Gaps from prior sessions
- Equal Highs (EQH) and Equal Lows (EQL)
- VWAP as a dynamic anchor

If a stock doesn't pass the pre-market filter, it does not make the watchlist. No exceptions.

---

### Phase 2 — Market Open / Price Discovery (9:30 – 9:33 AM EST)

The first 1 to 3 candles at open are for **observing, not trading**.

This is the most important rule in the system. The opening seconds are dominated by algorithmic orders, retail panic, and market maker manipulation. The spread is wide, fills are unpredictable, and the moves are frequently fake. Entering in the first candle is gambling, not trading.

What you are watching for instead:

- **Opening Range** — the high and low formed in the first 1–3 candles become your bias anchors for the session
- **Relative Volume (RelVol)** — is volume spiking above 2x the average? If yes, institutional money is present. If no, the move lacks conviction and you wait or walk away entirely
- **Gap behaviour** — is the stock holding above its pre-market low (bullish), or is it already fading back toward the gap fill (bearish)? This tells you which direction has the edge

This phase sets your directional bias. You are not guessing — you are reading what the market is actually doing before committing a dollar.

---

### Phase 3 — SMC Signal Detection

Once your bias is established, you shift to the LuxAlgo Smart Money Concepts script and watch for four specific signals, in this priority order:

**1. Internal CHoCH (Change of Character)**
The earliest warning that direction is shifting. Price closes above an internal swing high (bullish CHoCH) or below an internal swing low (bearish CHoCH). This is detected using the script's 5-bar internal structure setting. On its own, CHoCH is a caution signal — combine it with volume and gap direction before acting.

**2. BOS (Break of Structure)**
A clean close above a swing high or below a swing low on the larger swing structure. This is your **directional confirmation**. A Swing BOS with a simultaneous RelVol spike is the highest-probability signal in this entire system. When you see it, the bias is confirmed and you move to entry.

**3. Order Block (OB)**
After a BOS, price will frequently retrace. The LuxAlgo script identifies the **last opposing candle before the break** as the Order Block — the zone where institutions placed their orders. This is your entry zone.
- Bullish OB: the base of the last up candle before a bullish BOS — this is where you buy the retrace
- Bearish OB: the top of the last down candle before a bearish BOS — this is where you short the retrace

Entering at the OB gives you the tightest possible stop and the best risk-to-reward ratio of the setup.

**4. Fair Value Gap (FVG)**
A three-candle pattern where an aggressive middle candle leaves a price gap between candle 1's high and candle 3's low. FVGs serve three roles:
- Bullish FVG below price = a hard support floor (potential add zone)
- Bearish FVG above price = a magnet and resistance target
- Price almost always revisits nearby FVGs within the first hour — treat them as price destinations, not just visual noise

---

### Phase 4 — Long and Short Setup Conditions

All of the following must align before entry. If even one is missing, you wait or you pass.

**Long (Buy) Setup**
- Gap up 5–10%+ with a real catalyst, holding above pre-market low
- Float under 50M, pre-market volume above 500K
- Internal bullish CHoCH confirmed on the SMC script
- Swing BOS above the opening range high with RelVol above 2x
- Price retraces into a bullish demand Order Block
- Bullish FVG visible below price as a support floor
- Entry: top of the OB zone
- Stop: below the OB low or below the FVG low
- Target 1: 0.75× ATR — exit 50% of position here
- Target 2: 1.5× ATR, or the next visible FVG above price

**Short (Sell) Setup**
- Gap fade, gap down, or extended move that is overcooked relative to ATR
- Internal bearish CHoCH confirmed on the SMC script
- Swing BOS below the opening range low with RelVol above 2x
- Price rejects from a bearish supply Order Block
- Bearish FVG visible above price as a ceiling
- Entry: bottom of the OB zone
- Stop: above the OB high or above the FVG high
- Target 1: 0.75× ATR — exit 50% of position here
- Target 2: 1.5× ATR, or the next visible FVG below price

---

### Phase 5 — Trade Management

Getting in is the easy part. Staying disciplined once you're in is where most traders lose money.

**Scaling out**
At Target 1, take 50% of your position off. Immediately move your stop to breakeven on the remaining half. Let the runner work toward Target 2 or the next FVG without interference.

**Invalidation rules — exit immediately if:**
- Price closes through your Order Block (the thesis is broken)
- Volume collapses after entry (smart money left the trade)
- Price closes back inside the supporting FVG (the floor has failed)

Do not hope. Do not average down. Exit clean and reset.

**Time rule**
If a momentum trade does not start moving within 10–15 minutes of entry, reduce size or exit entirely. Valid momentum setups are immediate and violent. A slow grind after entry means your read was wrong, your timing was off, or the stock has lost its in-play status. Move on.

---

## The SMC Script (LuxAlgo)

The flowchart is designed around the **Smart Money Concepts [LuxAlgo]** indicator on TradingView.

For this first-hour momentum system, the most relevant settings are:

| Setting | Recommended Value | Why |
|---|---|---|
| Mode | Historical | See all structure, not just recent |
| Show Internal Structure | On | CHoCH is your first signal |
| Show Swing Structure | On | BOS is your confirmation |
| Show Internal Order Blocks | On | Entry precision |
| Show Swing Order Blocks | Optional | Useful for bigger picture |
| Fair Value Gaps | On | Entry floors and targets |
| Equal Highs/Lows | On | Liquidity levels to watch |
| Show Strong/Weak High/Low | On | Bias anchor reference |

The internal structure layer (5-bar) is your primary signal source during the first hour. The swing structure layer provides the bigger picture bias confirmation.

---

## Key Concepts Glossary

| Term | Meaning |
|---|---|
| **BOS** | Break of Structure — price closes beyond a prior swing high or low, confirming trend direction |
| **CHoCH** | Change of Character — the first sign of a trend reversal, faster than a full BOS |
| **Order Block (OB)** | The last opposing candle before a structure break — marks an institutional order zone |
| **Fair Value Gap (FVG)** | A price gap left by an aggressive three-candle move — acts as support, resistance, or target |
| **EQH / EQL** | Equal Highs / Equal Lows — price levels where stop orders cluster, often swept before reversing |
| **Float** | The number of shares available to trade publicly — lower float = higher volatility potential |
| **ATR** | Average True Range — measures average daily price range, used to size stops and targets |
| **RelVol** | Relative Volume — current volume vs. average volume at the same time of day |
| **Gap** | The difference between yesterday's close and today's open, expressed as a percentage |
| **Catalyst** | The fundamental news event driving the gap — earnings, FDA, merger, short squeeze, etc. |
| **Opening Range** | The high and low formed in the first 1–3 candles — used as session bias anchors |

---

## Disclaimer

This flowchart and README are for **educational purposes only**. Nothing here constitutes financial advice or a recommendation to buy or sell any security. Trading involves substantial risk of loss. Always do your own research, manage your own risk, and never trade with money you cannot afford to lose.

---

*Built with 20+ years of momentum trading experience combined with Smart Money Concepts structure analysis.*
