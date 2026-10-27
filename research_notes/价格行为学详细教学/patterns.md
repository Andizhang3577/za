# 价格行为学中的K线形态与图表形态（Candlestick & Chart Patterns in Price Action Trading）

> Research notes for the report writer. Scope: definitions, buyer/seller psychology, strong vs. weak versions, context, entry/stop, and reliability evidence, with a stock-market focus (US and China A-shares).
>
> **Source-access caveat (important):** In this session the proxy blocked direct page fetches from thepatternsite.com, traders.com, fidelity.com and brookstradingcourse.com (403 / DNS failure). Statistics below therefore come from search-engine extracts of those primary pages, or from secondary pages that quote them. Where a number appears only on a secondary or reposted page, it is flagged. Items in **Inferences** that are marked "[standard definition, not verified this session]" are textbook conventions from general knowledge. The writer should present them as conventional definitions, not as cited findings.

---

## Q1. Single-bar patterns (单根K线): pin bar / hammer / shooting star, doji, trend bars, inside bar, outside bar, reversal bars. How does Brooks define a good reversal bar?

### Takeaway
A single bar is only a *signal bar* (信号K线). Its meaning depends on where it prints: at support/resistance, after a sell-off or a run-up, or at a trend-channel line. Brooks' good reversal bar has a tail of about 1/3 to 1/2 of its range on the rejected side, closes beyond the prior close in the new direction, and overlaps the prior bars little. Brooks treats dojis, and outside or inside bars that print in tight trading ranges, as mostly meaningless on their own.

### Cited Findings
**Brooks reversal bar (反转K线), as paraphrased by third parties (primary book text not retrieved):**
- Bull reversal bar (看涨反转K线) per Brooks: "an open near or below the close of the prior bar and a close above the open and above the prior bar's close, a lower tail that is about one-third to one-half the range of the bar and a small upper tail, not much overlap with the prior bar", and the mirror image for a bear reversal bar — [TradingView "Al Brooks Suite" script description](https://www.tradingview.com/script/wCM07z8n-Al-Brooks-Suite) (also on [in.tradingview.com](https://in.tradingview.com/script/wCM07z8n-Al-Brooks-Suite)).
- A SlideShare copy of a "Brooks probabilities" document gives the criteria as "two or more of the following" (open vs. prior close, close vs. open, tail of 1/3 to 1/2 of the bar, little overlap). Its wording for the *bull* bar appears mirrored, which is almost certainly a transcription error, so use the TradingView wording above — [SlideShare "brooksprobabilities"](https://www.slideshare.net/slideshow/brooksprobabilitiesdoc/258643754).
- A Brooks-based indicator defines a reversal bar operationally as a single bar that makes a new extreme and closes in the opposite half of its range. It *disables* reversal-bar signals inside trading ranges when overlap with the prior bar exceeds 50%, reflecting Brooks' view that heavy-overlap bars in ranges are weak signals — [TradingView Al Brooks Suite](https://id.tradingview.com/script/wCM07z8n-Al-Brooks-Suite).

**Hammer / shooting star / pin bar (锤子线 / 射击之星 / Pin Bar 或 "Pinocchio bar"):**
- Nison, *Japanese Candlestick Charting Techniques* (1991), is credited with the rule that a hammer's lower shadow is at least twice the real body. The body sits near the top of the range with little or no upper shadow, and the candle must follow a decline. Confirmation is a later close beyond the candle — [TheRightTrader: Hammer](https://therighttrader.com/learn/candlestick-patterns/hammer); [LuxAlgo: Inverted Hammer](https://www.luxalgo.com/library/concept/inverted-hammer.md).
- The shooting star mirrors it: a small body near the low, an upper shadow at least 2x the body, appearing after an advance. Confirmation is usually a later close below the shooting star's low — [LuxAlgo: Shooting Star](https://www.luxalgo.com/library/concept/shooting-star.md); [TheRightTrader: Shooting star](https://therighttrader.com/learn/candlestick-patterns/shooting-star).

**Doji (十字星):**
- Brooks, as summarized: never assume a doji is a reversal by itself. Wait for the next bar to show which side wins — [NexusFi Academy: Al Brooks Price Action Method](https://nexusfi.com/a/strategies/al-brooks-price-action-method).

**Inside bar (内包线 / 孕线) and outside bar (外包线):**
- An inside bar's high and low are both within the prior bar's range. An outside bar exceeds the prior bar's range on both sides — [Al Brooks Price Action Pro (TradingView)](https://in.tradingview.com/script/MjUXio51-Al-Brooks-Price-Action-Pro/); [technical-analysis-pro.com](https://www.technical-analysis-pro.com/patterns-inside-bar-outside-bar-trading/).
- Classic inside-bar entry: a buy stop one tick above the inside bar's high and a protective stop one tick below its low. The wider fallback stop goes below the low of the "mother" bar (the bar that contains the inside bar) — [technical-analysis-pro.com](https://www.technical-analysis-pro.com/patterns-inside-bar-outside-bar-trading/).
- Brooks (Ask Al Q&A, as quoted in search extract): outside bars that occur in a tight trading range "are meaningless" — [Ask Al Brooks: Outside Bars](https://www.brookstradingcourse.com/ask-al/outside-bars-significance/) (page itself not fetchable this session; extract only).
- Brooks teaches that stops cluster one tick beyond the signal bar or entry bar, which is why entries and protective stops conventionally sit one tick beyond the signal bar — [NexusFi Academy](https://nexusfi.com/a/strategies/al-brooks-price-action-method).

**Trend bars / marubozu (趋势K线 / 大阳线、大阴线 / 光头光脚):**
- Bulkowski's candle research, as summarized by StockCharts: Three White Soldiers (三白兵), a cluster of three strong trend bars, shows an 82% reversal rate and ranks #3 of 103 for reversal, but is extremely rare — [StockCharts Insider: 5 Bullish Candlestick Patterns](https://articles.stockcharts.com/article/stockcharts-insider-5-bullish-candlestick-patterns-ranked-tested-and-mostly-easy-to-spot/).

### Inferences
- **Brooks' framework, in teaching form** [standard definition, not verified this session]:
  - A *trend bar* (趋势K线) has a large body and small tails. It shows one side in control, and consecutive large trend bars ("strong breakout") favor follow-through, not reversal.
  - A *doji* or *trading-range bar* has a small body relative to range and shows balance. Brooks says a doji can be a weak signal bar but a "bad" one, especially when it is one of several overlapping bars.
  - A *signal bar* (信号K线) is the bar before entry. The *entry bar* (入场K线) is the bar that triggers the stop order.
- **Psychology**:
  - Hammer / bull reversal bar: sellers pushed to a new low but could not hold it. Buyers absorbed the selling and closed the bar near its high. Trapped late shorts must buy back above the bar, which fuels the move.
  - Shooting star: the mirror of the hammer.
  - Inside bar: contraction or indecision (酝酿, "breakout mode" in Brooks' terms).
  - Outside bar: both sides were stopped out in one bar. Its meaning comes from where it closes and where it sits.
- **Strong vs. weak signal bar checklist** (synthesized from the Brooks criteria above):
  - Strong: the tail is on the rejected side; the bar closes in the new direction beyond the prior close; little overlap with prior bars; it appears at a logical location (support, a trend-channel line overshoot, a test of a prior extreme, a second-entry setup); it is larger than average without being climactic.
  - Weak: a doji body; heavy overlap with prior bars; it sits in the middle of a tight trading range; it is a counter-trend signal against a strong trend with no prior trendline break.
- **Location rule for hammers**: a hammer printed mid-range or during a strong bear channel with no prior trendline break is a low-probability buy. The same bar at a double-bottom test or a measured-move target carries more weight.
- **Pin bar** is the Western/forex price-action name (popularized by forex educators). It is essentially a hammer or shooting star judged on tail size, without the strict 2x-body rule. [not verified this session]
- **A-share adaptation**: daily-chart signal bars are more reliable than intraday ones for most A-share traders because T+1 settlement (T+1交易制度) prevents same-day exit. A trader who buys on an intraday reversal bar cannot stop out until the next session. This is a mechanical reason to favor end-of-day signals and to size positions for overnight gap risk. (This is my inference from the T+1 rule itself. No study found.)

### Gaps
- Brooks' primary text (*Trading Price Action Reversals*, 2012) could not be fetched. The exact wording of his "good reversal bar" list and his bar-count probabilities (e.g., "60% / 40%" trader's-equation language) are unverified in this session.
- No Bulkowski statistics were retrieved for the single-candle hammer, shooting star or doji (his pages list a "reversal rate" for each, but the sites were blocked).
- No source was retrieved for Brooks' specific definition of a "good" bear reversal bar beyond the mirrored description.

---

## Q2. Multi-bar patterns (组合K线): engulfing, ii / iii, ioi, morning/evening star, two-bar reversal

### Takeaway
Multi-bar patterns are mostly variants of the same idea: a failed push followed by a strong bar the other way (engulfing, two-bar reversal, stars), or compression before a breakout (ii, iii, ioi). Bulkowski's large-sample work finds that many of the best-ranked reversal candles are rare. The common ones (engulfing, roughly 63% reversal per secondary summaries) are only modestly better than a coin flip.

### Cited Findings
- **Bulkowski's candle methodology**: he examined more than 4.7 million price bars to identify and track 103 candle patterns, ranking each on reversal rate, frequency and overall performance — [Stocks & Commodities V.29:11, "The Eight Best-Performing Candles"](https://store.traders.com/stcov292eibe.html) (search extract).
- **Morning star (早晨之星 / 启明星)** reversal rate is about 78%, and **bullish engulfing (看涨吞没 / 阳包阴)** is about 63% (StockCharts summary of Bulkowski) — [StockCharts Insider](https://articles.stockcharts.com/article/stockcharts-insider-5-bullish-candlestick-patterns-ranked-tested-and-mostly-easy-to-spot/).
- **Three inside up (三内部上涨)**, an inside-bar or harami variant confirmed by a third bar, acts as a bullish reversal 65% of the time (Bulkowski) — search extract of [Bulkowski Pattern Site](https://thepatternsite.com/MorningStar.html) results set.
- **Evening doji star (黄昏十字星)** ranks 12th for reversal rate but 81st of 103 for frequency, meaning it is rare — [thepatternsite.com/EveningDojiStar.html](https://thepatternsite.com/EveningDojiStar.html) (search extract).
- **Bearish breakaway** reverses 63% of the time (rank 23) with overall performance rank 11 — [thepatternsite.com/BearBreakaway.html](https://thepatternsite.com/BearBreakaway.html) (search extract).
- **Rarity trap**: Three Stars in the South ranks #1 for reversal, but on only 9 samples, and is 103/103 overall — [thepatternsite.com/ThreeStarsSouth.html](https://www.thepatternsite.com/ThreeStarsSouth.html) (search extract).
- An Investing.com piece cites an 84% reversal rate for the bearish three-line strike. This is a commercial secondary claim and not confirmed against Bulkowski — [Investing.com: Chart Patterns Ranked by Accuracy](https://uk.investing.com/analysis/chart-patterns-ranked-by-accuracy-200622665).
- **ii (双内包)**: two consecutive inside bars, "a classical Brooks breakout setup" — [Al Brooks Price Action Pro (TradingView)](https://in.tradingview.com/script/MjUXio51-Al-Brooks-Price-Action-Pro/).
- **ioi (内-外-内)**: definitions conflict. One indicator calls it a 3-bar "breakout mode" compression. Another describes it as inside bar, then outside bar, then inside bar, often serving as a second counter-trend entry. Entry is one tick above the last inside bar's high, and the stop goes one tick below that inside bar's low or below the low of all three bars — [Brooks Price Action H-L Counts and Bar Types (TradingView)](https://www.tradingview.com/script/g0vTIdy2-Brooks-Price-Action-H-L-Counts-and-Bar-Types/); [technical-analysis-pro.com](https://www.technical-analysis-pro.com/patterns-inside-bar-outside-bar-trading/).
- **Two-bar reversal (双K反转)**: a strong trend bar followed immediately by a strong bar in the opposite direction — [Al Brooks Price Action Pro (TradingView)](https://in.tradingview.com/script/MjUXio51-Al-Brooks-Price-Action-Pro/).
- **Final flag as ii**: Brooks' glossary says a final flag "often can be as simple as an ii pattern" — [NexusFi: Al Brooks definition: Final Flag](https://nexusfi.com/showthread.php?t=20752).

### Inferences
- **Engulfing (吞没形态: 阳包阴 / 阴包阳)** [standard definition, not verified this session]: the second real body fully covers the first body, in the opposite color, after a move in the first bar's direction. In Brooks terms, a bullish engulfing is usually an *outside up bar* or a *two-bar reversal*. Its strength rises with the size of the second body, a close above the first bar's high, and a location at support or a trend-channel overshoot.
- **Morning star / evening star (早晨之星 / 黄昏之星)** [standard definition]: bar 1 is a long trend bar in the existing direction. Bar 2 is a small body (star; a doji makes it a doji star), ideally gapping away from bar 1. Bar 3 is a strong opposite trend bar that closes well into bar 1's body, conventionally beyond its midpoint. Psychology: momentum stalls, then the other side takes control. In Brooks' terms this is a three-bar version of a reversal bar. On US daily charts true body gaps are rare, so the definition is usually relaxed.
- **iii (三连内包)**: a further compression than ii. Brooks treats it as breakout mode: enter on a stop in either direction, and expect a failed first breakout fairly often. [not verified this session]
- **Entry/stop convention for all multi-bar reversals**: enter on a stop one tick beyond the extreme of the last bar of the pattern. The protective stop goes one tick beyond the pattern's opposite extreme (the low of the whole morning star, for example). The first target is often at least 1R, or the nearest opposite magnet such as a prior swing or the moving average.
- **The headline lesson from the statistics**: frequent patterns (engulfing ~63%) are only modestly above 50%. High-percentage patterns are rare and small-sample. Context and trade management therefore matter more than pattern name.

### Gaps
- Bearish engulfing, evening star (non-doji) and harami (孕线) reversal rates from Bulkowski were not retrieved.
- Primary Brooks definitions of ioi and of entry rules for the two-bar reversal were not verified, and secondary sources conflict on ioi.

---

## Q3. Chart patterns (图表形态): double top/bottom, head & shoulders, wedges / three pushes, flags & pennants, triangles, channels, trading ranges, breakout pullbacks, failed breakouts / traps, Brooks' final flag

### Takeaway
Bulkowski's stock data shows reversal *bottoms* (inverse head-and-shoulders: 11% break-even failure, 45% average rise) outperforming reversal *tops* (H&S top: 19% failure, 16% average decline). Short-term continuation patterns such as standard flags and pennants have high failure rates (around 44 to 54%) when measured on the swing. Brooks re-frames patterns as sequences of breakouts that either follow through or fail. Wedges (three pushes), final flags and failed breakouts are his core reversal structures, and measured moves are his standard targets.

### Cited Findings
**Double bottom / double top (双底 "W底" / 双顶 "M头"):**
- Bulkowski's failure rate means price failing to rise at least 5% above the breakout price, where the breakout price is the highest high between the two bottoms. His average rise runs from breakout to the "ultimate high" (the high before a 20% reversal). He warns the numbers come from "hundreds of perfect trades, so your chance of duplicating such a rise on a consistent basis is probably zero" — [Bulkowski: Double Bottom Types](https://thepatternsite.com/DoubleBottomTypes.html) (search extract).
- Of the four Adam/Eve combinations, Eve & Eve (two rounded bottoms) has the smallest failure rate and highest average rise, making it the best double bottom to trade per Bulkowski — [Bulkowski: Double Bottom Types](https://thepatternsite.com/DoubleBottomTypes.html) (search extract).
- Adam & Eve double bottom (bull market): rank 17 of 39, break-even failure 12%, average rise 43%. These figures come from third-party TradingView reposts and were not confirmed against Bulkowski's table — [TradingView repost](https://it.tradingview.com/chart/SOLUSDT/6ceahBVB-SOL-Adam-Eve-Double-Bottom-Confirming); [TradingView overview](https://www.tradingview.com/chart/ICPUSDT/4NUciFTn-Adam-Eve-Double-Bottoms).

**Head and shoulders (头肩顶 / 头肩底):**
- H&S top (bull market): break-even failure 19%, average decline 16%, pullback rate 68%, 51% meet price target, more than 2,800 trades, rank 9 of 36 — [Bulkowski on Head-and-Shoulders Tops](https://www.thepatternsite.com/hst.html) (search extract).
- Complex H&S top (头肩顶复合形态, multiple heads or shoulders): failure 18%, average decline 17%, pullback rate 66%, 47% meet target, more than 650 trades — [Bulkowski on Complex H&S Tops](https://thepatternsite.com/chst.html) (search extract).
- H&S bottom (头肩底): failure 11%, average rise 45%, throwback rate 65%, 71% meet target — [Bulkowski on H&S Bottoms](https://thepatternsite.com/hsb.html) (search extract).
- Bulkowski's trading tip: "pullbacks hurt post breakout performance" — [Bulkowski on H&S Tops](https://www.thepatternsite.com/hst.html).
- A TitanFX article claims a 93% H&S success rate from "2021-2023 research." This is unverifiable and contradicts Bulkowski, so do not use it — [TitanFX](https://research.titanfx.com/technical-analysis/candlestick-chart/head-and-shoulders-top-bottom).

**Flags, pennants, triangles, wedges (旗形、三角旗、三角形、楔形):**
- Bull flag (上升旗形 / 牛旗), Bulkowski data via a secondary summary: 44% break-even failure, 9% average rise, 46% reach target. Bulkowski does not rank standard flags against breakout-to-ultimate-high patterns because flags are measured on the short-term swing. The high-and-tight flag (高窄旗形) is far stronger: 15% failure and 39% average rise — [LiberatedStockTrader: Chart patterns ranked](https://www.liberatedstocktrader.com/chart-patterns-reliable-profitable/) (secondary; figures vary between blogs).
- Bull pennant (三角旗): breaks upward 57% of the time, and 54% of upward breakouts fail to clear the 5% break-even threshold; average rise 7%, 35% reach the flagpole target — [ChartScout: Bull pennant](https://chartscout.io/bull-pennant-pattern-crypto) (secondary, quoting stock data).
- Ascending triangle (上升三角形): one ranking gives 17% failure and 43% average gain, but figures vary by source. Bulkowski's own page ranks it 16 for performance and 27 for failure in bull markets — [LiberatedStockTrader](https://www.liberatedstocktrader.com/chart-patterns-reliable-profitable/); [Bulkowski on Chart Pattern Performance](https://thepatternsite.com/id75.html).
- Falling wedge (下降楔形): only an unattributed 74% figure was found, so it is unconfirmed — [Barchart PDF](https://www.barchart.com/media/education/pdf/Chart%20Patterns%20That%20Actually%20Work%20-%20Proven%20Setups%20Traders%20Use%20to%20Win.pdf).

**Brooks' structures:**
- **Wedge / three pushes (楔形 / 三推)**: Brooks' glossary defines three pushes as three swing highs, each usually higher, or three swing lows, each usually lower. The wedge shape increases the chance of success, but any three-push pattern trades like a wedge — [Brooks Trading Course: Learn to trade Emini wedges](https://www.brookstradingcourse.com/futures-market/learn-to-trade-emini-wedges/); [O'Reilly: Trading Price Action Reversals, Ch. 5 "Wedges and Other Three-Push Reversal Patterns"](https://www.oreilly.com/library/view/trading-price-action/9781118172308/OEBPS/9781118172308_epub_ch_05.htm).
- After a three-push reversal triggers, the typical targets are first the start of the wedge, then a measured move based on the pattern's height — [O'Reilly Ch. 5](https://www.oreilly.com/library/view/trading-price-action/9781118172308/OEBPS/9781118172308_epub_ch_05.htm).
- If a wedge fails (e.g., a wedge top breaks out above instead of reversing, or a bull wedge falls below its low), the move "often will extend for a measured move" equal to the wedge's height — [Brooks: Emini wedges](https://www.brookstradingcourse.com/futures-market/learn-to-trade-emini-wedges/) (search extract).
- **Final flag (最终旗形)**: late in a protracted trend, a mostly horizontal flag forms that extends sideways for several bars and breaks a trendline. It then breaks out to a new trend extreme but quickly reverses. This Failed Final Flag breakout "often marks the end of the trend." It can be as simple as an ii — [NexusFi: Al Brooks definition: Final Flag](https://nexusfi.com/showthread.php?t=20752); [Brooks: Learn to trade Emini final flags](https://www.brookstradingcourse.com/futures-market/learn-to-trade-emini-final-flags/).
- **Failed breakout (假突破 / 失败突破) and breakout pullback (突破回踩)**: Brooks' "failed failure" is a failed breakout that then resumes in the original breakout direction. That is effectively a breakout pullback, a small flag right after the breakout. Brooks reportedly came to dislike the term — [Brooks forum: Failed Failure](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/failed-failur/).
- Brooks' book *Trading Price Action Trading Ranges* covers ranges, breakouts and pullbacks (PDF copies circulate online; not used as a source here) — [O'Reilly book listing](https://www.oreilly.com/library/view/trading-price-action/9781118172308/OEBPS/9781118172308_epub_ch_05.htm).

### Inferences
**Teaching definitions and psychology** [standard definitions, not verified this session]:
- **Double bottom / top (双底 / 双顶)**
  - Structure: two lows at about the same price, separated by a rally whose high is the neckline (颈线). Confirmation is a close above the neckline.
  - Psychology: the second test fails to attract new sellers below the first low, and bears who sold the first low take profits.
  - Brooks nuance: the second bottom can be slightly higher (higher low) or slightly lower (a "double bottom with a lower low", effectively a failed breakout below the first low). A double bottom inside a strong bear trend is usually just a bear flag.
  - Measured target: neckline plus the pattern height.
  - Entry: either on the second-bottom signal bar (wider risk, better price), or on the neckline breakout or its pullback (higher probability, worse price).
  - Stop: below the second bottom.
- **Head and shoulders (头肩顶 / 头肩底)**
  - Structure: left shoulder, then a higher head, then a lower right shoulder, with a neckline through the two troughs.
  - Psychology: the right shoulder is a *lower high*, the first sign the bulls failed to make a new high.
  - Brooks view: an H&S top is just a lower-high double top or a wedge variant, and in a bull trend most H&S tops become bull flags (they fail).
  - Classic entry: a break of the neckline, or the pullback to it (Bulkowski: 68% pull back, and pullbacks hurt performance). Stop above the right shoulder.
- **Wedge / three pushes (楔形 / 三推)**: three pushes with converging trendlines show diminishing momentum (each push gains less), and late trend followers get trapped at the third push. Brooks treats the wedge as a *trend-channel-line overshoot and reversal*.
  - Entry: on a strong reversal signal bar after the third push, ideally with a prior trendline break.
  - Stop: beyond the third push's extreme.
  - Targets: the start of the wedge first, then a measured move.
  - If the wedge fails (the third push breaks out strongly), expect a measured move in the breakout direction.
- **Flag / pennant (旗形 / 三角旗)**
  - Structure: a short, tight counter-trend drift or symmetrical triangle after a strong move (the flagpole, 旗杆).
  - Brooks terms: High 1 / High 2 (H1/H2, 一次/二次回调买点) in bull trends and Low 1 / Low 2 in bear trends.
  - Entry: on a stop above the flag's signal bar. Stop below the flag low.
  - Target: the flagpole height, or a measured move.
  - Bulkowski's high failure rate for ordinary flags (44%) argues for requiring a strong pole and a tight flag; the high-and-tight flag has only 15% failure.
- **Triangles (三角形: 上升 / 下降 / 对称)**: converging range boundaries show both sides losing conviction (contraction before expansion).
  - Brooks sees most triangles as trading ranges in breakout mode, where the first breakout fails often enough that a second entry is preferred.
  - An ascending triangle's flat top with rising lows shows buyers absorbing supply at one price.
- **Channels (通道)**: tight channels (窄通道) mean strong trends. Fade only after a clear break.
  - Broad channels (宽通道) behave like sloped trading ranges: buy low, sell high within them.
  - A channel-line overshoot followed by a reversal bar is a classic wedge-type reversal setup.
- **Trading range / box (震荡区间 / 箱体)**: Brooks' principle is that roughly 80% of breakout attempts from a trading range fail [commonly attributed to Brooks; not verified this session].
  - Traders buy near the bottom third and sell near the top third, avoid the middle, and treat strong-looking breakouts with skepticism until follow-through appears.
- **Breakout pullback (突破回踩)**: after a strong breakout, the first pullback that holds above the breakout point (or never fills the "breakout gap") is a high-probability with-trend entry. This is the same idea as the Bulkowski "throwback" / "pullback", though Bulkowski's data shows pullbacks reduce average performance.
- **Failed breakout / trap (假突破 / 诱多诱空)**: a breakout bar with no follow-through, followed by a strong reversal bar back inside the range. Breakout traders are trapped and their stops fuel the reversal. Brooks' "final flag" and "failed wedge" are specific trap contexts.
- **A-share specifics**:
  - In A-shares, breakouts often occur via 涨停板 (limit-up). A limit-up breakout bar is a "trend bar" whose true range is capped. The follow-through often comes as a gap the next day, so the classic Western "pullback to neckline" entry may never happen.
  - Conversely, a 炸板 (failed limit-up) at a breakout level is a strong local failed-breakout signal.
  - (Inference from the price-limit mechanics; no quantitative study found.)

### Gaps
- Bulkowski's primary tables for flags, pennants, triangles, wedges, rectangles, double tops and double bottoms (all Adam/Eve variants) could not be fetched. The flag, pennant and triangle numbers above come from secondary blogs and disagree with each other.
- No source retrieved for Brooks' "80% of trading-range breakouts fail" or his "measured move" probabilities.
- No A-share-specific statistical study of classic chart patterns was found in this session.

---

## Q4. Wyckoff accumulation / distribution schematic (威科夫吸筹 / 派发): springs, upthrusts, signs of strength

### Takeaway
Wyckoff describes a trading range in five phases (A to E).
- Phase A stops the prior trend: PS, SC, AR, ST.
- Phase B builds the cause inside the range.
- Phase C tests it: a spring in accumulation, an upthrust / UTAD in distribution.
- Phase D shows strength: SOS, LPS, back-up.
- Phase E is the trend out of the range.
A spring is functionally Brooks' failed downside breakout of a trading range, and an upthrust is the failed upside breakout.

### Cited Findings
- Accumulation Phase A: Preliminary Support (PS), Selling Climax (SC), Automatic Rally (AR) and Secondary Test (ST) define the trading range — [LuxAlgo: Wyckoff Accumulation Schematic](https://www.luxalgo.com/library/concept/wyckoff-accumulation-schematic.md).
- Phase B: large interests accumulate while the range develops. Phase C: the test, often a **spring (弹簧 / 震仓)** below support. Phase D: Sign of Strength (SOS), Last Point of Support (LPS) and the back-up (BU) after the breakout above resistance (the "creek"). Phase E: markup (拉升) — [LuxAlgo](https://www.luxalgo.com/library/concept/wyckoff-accumulation-schematic.md).
- There are two accumulation schematics, one with a spring and one without. In the no-spring version price never breaks support, the ST makes a higher low, and the breakout comes directly from consolidation — [TrendSpider: Wyckoff Accumulation](https://trendspider.com/learning-center/chart-patterns-wyckoff-accumulation/).
- Distribution mirrors accumulation. Phase A has PSY (preliminary supply), BC (buying climax), AR and ST. Key events are UT / UTAD (upthrust after distribution), SOW (sign of weakness) and LPSY (last point of supply) — [TrendSpider](https://trendspider.com/learning-center/chart-patterns-wyckoff-accumulation/); [TradingView Wyckoff cheat-sheet repost](https://th.tradingview.com/scripts/search/accumulation/page-8).

### Inferences
- **Volume signatures** [standard Wyckoff teaching, not verified this session]:
  - SC: a climactic volume spike with wide-range down bars (恐慌性抛售).
  - ST: lower volume on the retest, which shows supply is drying up.
  - Spring: a brief penetration of support that recovers quickly. The best version comes on low volume ("no supply"). A high-volume spring needs a successful low-volume test.
  - SOS: a wide-range up bar on expanding volume through the creek.
  - LPS / BU: a shallow pullback on declining volume, which is the lower-risk entry.
  - UTAD: a break above the range high that fails back inside, the mirror of the spring.
- **Mapping to price-action trading**:
  - Spring = failed bear breakout of a trading range (假跌破), whose bull reversal bar is the signal bar.
  - SOS = strong bull breakout.
  - LPS / BU = breakout pullback.
  - UTAD = failed bull breakout / final flag top.
  - Entry and stop placement follow the same logic: buy above the spring's reversal bar with the stop below the spring low, or buy the LPS with the stop below the LPS.
- **A-share usage**: "主力吸筹 / 洗盘 / 出货" vocabulary in Chinese retail literature is essentially popularized Wyckoff composite-operator thinking. 洗盘 ≈ spring / shakeout, 出货 ≈ distribution.

### Gaps
- No primary Wyckoff source or Pruden / Weis / Villahermosa text retrieved. UTAD criteria and volume rules above are textbook convention, not verified this session.
- No statistical evidence on Wyckoff pattern reliability was found.

---

## Q5. Volume (量价关系) and gaps (缺口) in stocks, including A-share specifics (T+1, 涨跌停)

### Takeaway
Gap meaning depends on location: common/area gaps fill within days, breakaway gaps take months, runaway gaps take weeks. Volume is a supporting confirmation rather than a primary signal. In A-shares, price limits (±10% main board, ±20% ChiNext/STAR, ±30% BSE) create distinctive limit-up bar shapes (一字板, T字板) whose volume interpretation is contested. T+1 makes overnight gap risk unavoidable for any same-day entry.

### Cited Findings
**Gaps (缺口):**
- Bulkowski lists five gap types: area (common, 普通缺口), breakaway (突破缺口), continuation / runaway (中继缺口 / 测量缺口), ex-dividend (除权缺口) and exhaustion (衰竭缺口) — [traders.com: Bulkowski on gaps (2003)](https://traders.com/Documentation/FEEDbk_docs/2003/09/Abstracts_new/Bulkowski/bulk.html); [Bulkowski: Gaps](https://www.thepatternsite.com/gaps.html).
- Average time to close (fill, 回补) a gap per Bulkowski:

  | Gap type | Upward gaps | Downward gaps |
  |---|---|---|
  | Area / common | 3–4 days | 3–4 days |
  | Breakaway | 89 days | 84 days |
  | Runaway | 45 days | 25 days |
  | Exhaustion | 6 days | 5 days |

  These are time-to-fill averages, not fill rates — [Bulkowski: Gaps](https://www.thepatternsite.com/gaps.html); [Bulkowski: Gauging Gaps](https://thepatternsite.com/GaugingGaps.html) (search extracts).
- Breakaway gaps exit congestion areas, runaway gaps occur mid-trend and exhaustion gaps occur at trend ends. Common gaps have no major news and fill quickly — [LuxAlgo: Runaway Gap](https://www.luxalgo.com/library/concept/runaway-gap.md); [TheRightTrader: breakaway gap](https://therighttrader.com/learn/chart-patterns/breakaway-gap).
- A claim that "73% of gaps eventually fill" is attributed to Bulkowski online but was not confirmed. Per-type fill rates on some sites (e.g., 85–95% for exhaustion gaps) are uncited and should not be used — [stockalarm.io](https://pro.stockalarm.io/blog/stock-gap-up-gap-down-explained).

**A-share price-limit rules (涨跌幅限制):**
- Main board (沪深主板) ±10%; ChiNext (创业板) and STAR (科创板) ±20%; Beijing Stock Exchange (北交所) ±30% — [cofool Q&A](https://licai.cofool.com/ask/qa_7231128.html).
- IPOs: main board, ChiNext and STAR have no limit for the first 5 trading days. BSE has no limit on day 1 only, then 30% — [cofool Q&A](https://licai.cofool.com/ask/qa_7114182.html).
- **ST stocks: possibly changed in 2026.** Traditionally main-board ST/*ST was ±5%, while ChiNext/STAR ST stocks follow ±20% and BSE ST ±30%. A July 2026 Guancha commentary discusses aligning main-board ST to ±10%, and a 2026 Q&A says main-board ST stocks are ±10% under rules effective 6 July 2026. Verify against SSE/SZSE announcements before relying on it — [Guancha 2026-07-03](https://www.guancha.cn/liuboyu/2026_07_03_822453.shtml); [cofool Q&A](https://licai.cofool.com/ask/qa_7021317.html).

**A-share limit-up bar shapes and volume lore (涨停板形态 / 量价):**
- **一字板** (one-price limit bar): the stock opens at the limit and stays sealed all day. Its essence is that liquidity is locked: buyers queue and sellers may be unable to sell. Judge it by seal stability, whether volume expands, and whether it reseals after opening — [Toutiao: 什么是一字板](https://www.toutiao.com/article/7591384037807014409/).
- **T字板**: the stock hits the limit, opens intraday (炸板), and reseals, forming a T-shaped bar. A first-time T-board that reseals strongly is considered strong. A T-board at a high position (e.g., 5+ consecutive limit-ups) is more likely distribution (出货). A shorter lower shadow and fewer openings mean a stronger board — [Zhihu: 涨停板分类终极指南](https://zhuanlan.zhihu.com/p/31679636961); [Zhihu: T字板战法](https://zhuanlan.zhihu.com/p/64205005).
- Low-volume limit-up (缩量涨停): one view holds that a large seal with small turnover means chips are well locked, so continuation is more likely. The opposite view is that a low-volume 一字板 at a high price level after a big run can be the tail end of distribution on good news — [CSDN: 量价关系总结](https://blog.csdn.net/u010025781/article/details/148390865); [cofool: 缩量一字板](https://licai.cofool.com/ask/qa_7272119.html).
- High-volume limit-up (放量涨停): heavy turnover at the limit is commonly read as possible distribution, so beware a pullback — [CSDN](https://blog.csdn.net/u010025781/article/details/148390865).
- General Chinese 量价 maxims: rising price on rising volume (价涨量增) and falling price on shrinking volume are "healthy." Price up on falling volume (价涨量缩) is a divergence (背离) showing weak follow-up demand. Be wary of high-level volume expansion; watch low-level volume contraction. The maxims are inconsistent across sources and not evidence-based — [Sina: A股量价口诀](https://www.sina.cn/news/detail/5311476315195591.html); [Sina: 量价关系六大口诀](https://www.sina.cn/news/detail/5314000985527585.html).

### Inferences
- **Brooks on volume** [not verified this session]: Brooks largely trades price alone and treats volume as secondary. Wyckoff, Bulkowski and Chinese 量价 traditions weight it heavily. For teaching, present volume as *confirmation*:
  - Breakouts on expanding volume, with pullbacks or tests on contracting volume, are better.
  - Climactic volume at the end of an extended move suggests exhaustion.
- **Gap teaching rule**:
  - A gap that is *not* filled during the next few bars acts like a strong trend bar (a breakout gap, which Brooks calls a "measuring gap" when it forms near the midpoint of a move).
  - A gap that fills quickly is a common/area gap or an exhaustion gap.
  - Bulkowski's fill times (3–4 days vs. 89 days) give a concrete way to classify in hindsight.
  - In A-shares, an unfilled gap left by a limit-up open (跳空涨停) is frequently used as a support level ("缺口不补").
- **Price limits distort candles**:
  - An A-share limit-up day caps the high, so a "marubozu" on a limit day understates demand.
  - Price limits also produce sequences of consecutive gaps, since the next-day open carries pent-up orders.
  - Sealed limit-down days (跌停) can leave sellers unable to exit, so "stop placement" can be meaningless. Positions in limit-prone small caps need smaller size.
- **T+1 (T+1交易制度)**: shares bought today cannot be sold until the next trading day. Intraday price-action setups (Brooks' 5-min E-mini style) cannot be traded symmetrically in A-shares. Long-side stops can only be executed from the next session onward, so the effective risk is "stop + overnight gap." (Rule well known; implication is inference.)

### Gaps
- No academic study on A-share gap fill rates or limit-up continuation probabilities was retrieved.
- Bulkowski gap fill *rates* (as opposed to fill times) were not confirmed.
- The 2026 change to main-board ST price limits (5% → 10%) is reported by low-reliability sources only and needs exchange confirmation.
- Search returned no authoritative source on how T+1 affects pattern behavior empirically.

---

## Q6. What does the evidence say about reliability?

### Takeaway
The evidence is mixed and mostly skeptical for *mechanical* candlestick rules:
- Marshall, Young & Rose (2006) found no significant excess returns from candlestick strategies on DJIA stocks (1992–2002), and similar null results appear in Japan and Thailand.
- Lo, Mamaysky & Wang (2000) found that algorithmically detected chart patterns carry *some incremental information*, especially for Nasdaq stocks, but did not show a trading profit.
- Bulkowski's descriptive statistics show many patterns beat random somewhat, with large dispersion and a strong rarity/sample-size caveat.
- Results depend heavily on exit rules and context, which supports the price-action view that location and management matter more than the pattern label.

### Cited Findings
- **Lo, Mamaysky & Wang (2000)**, "Foundations of Technical Analysis," *Journal of Finance* 55(4): 1705–1765. They used nonparametric kernel regression to detect patterns such as head-and-shoulders and double bottoms algorithmically on a large number of US stocks, 1962–1996. Several patterns "do provide incremental information and may have some practical value" — [MIT (Lo) paper page](https://web.mit.edu/Alo/www/Papers/techanal.html); [NBER w7613](https://www.nber.org/papers/w7613).
- The incremental information was especially notable for Nasdaq stocks — [CFA Institute Digest summary](https://rpc.cfainstitute.org/-/media/documents/article/cfa-digest/2001/dig-v31-n1-811-pdf.pdf).
- LMW caution that traditional patterns like head-and-shoulders "may not be optimal." A pattern that best flags statistical anomalies need not be optimal for trading profits, and vice versa. They also identify subjectivity ("in the eyes of the beholder") as the field's main obstacle — [NBER w7613 PDF](https://www.nber.org/system/files/working_papers/w7613/w7613.pdf); [MIT page](https://web.mit.edu/~alo/www/Papers/techanal.html).
- **Marshall, Young & Rose (2006)**, "Candlestick technical trading strategies: Can they create value for investors?" *Journal of Banking & Finance*. On DJIA stocks 1992–2002, using a bootstrap of random OHLC series, candlestick strategies did not generate statistically significant excess returns over random trading — [ResearchGate](https://www.researchgate.net/publication/223853109_Candlestick_technical_trading_strategies_Can_they_create_value_for_investors); [Scribd copy](https://www.scribd.com/document/232577907/Marshall-Young-Rose-2006).
- **Marshall, Young & Cahan (Japan)**: candlestick strategies on the Tokyo Stock Exchange provided no consistent profitability. (The search summary named the co-author "Chang"; the published paper's co-author is believed to be Cahan, so verify.) — [ResearchGate: Are candlestick technical trading strategies profitable in the Japanese equity market?](https://www.researchgate.net/publication/5157791_Are_candlestick_technical_trading_strategies_profitable_in_the_Japanese_equity_market).
- **Caginalp & Laurent (1998)**: some three-day candlestick patterns showed short-term predictive power in S&P 500 stocks — cited in [Lu, Chen & Hsu / ScienceDirect: Profitable candlestick trading strategies—The evidence from a new perspective](https://www.sciencedirect.com/science/article/abs/pii/S1058330012000092).
- **Lu, Chen & Hsu (2015 / Review of Financial Economics)**: found significant positive returns using the Caginalp–Laurent holding/exit rule but *not* using the Marshall–Young–Rose exit rule, so the conclusion depends on exit design — [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S1058330012000092).
- **Thailand (Tharavanij, Siraprapasiri & Rajchamaha 2017, SAGE Open)**: most candlestick reversal patterns do not yield statistically significant mean returns — [SAGE Open](https://journals.sagepub.com/doi/10.1177/2158244017736799).
- **Taiwan (Goo, Chen & Chang 2007)**: tested Japanese candlestick strategies on Taiwan stocks — [Business Perspectives PDF](https://businessperspectives.org/images/pdf/applications/publishing/templates/article/assets/1934/imfi_en_2007_04_1_Goo.pdf) (results not extracted this session).
- **Bulkowski**: 103 candle patterns tracked across more than 4.7M bars, ranked on reversal rate, frequency and performance — [S&C V.29:11](https://store.traders.com/stcov292eibe.html).
  - He warns his chart-pattern figures are based on "hundreds of perfect trades" that traders are unlikely to replicate — [Bulkowski: Double Bottom Types](https://thepatternsite.com/DoubleBottomTypes.html).
  - His top reversal candle (Three Stars in the South) rests on only 9 samples — [thepatternsite.com](https://www.thepatternsite.com/ThreeStarsSouth.html).
- Bulkowski also maintains pages on chart pattern failure and performance ranking — [Bulkowski on Chart Pattern Failure](https://thepatternsite.com/id84.html); [Bulkowski on Chart Pattern Performance](https://thepatternsite.com/id75.html).
- A 2026 blog claims analysis of 370K+ trades on whether chart patterns work. It is commercial and its methodology was not reviewed — [StockDataAnalytics](https://www.stockdataanalytics.com/blog/do-chart-patterns-work-in-2026-what-the-data-shows/).

### Inferences
- **How to present reliability in teaching**:
  1. Pattern labels alone give at most a small edge. Frequent candle patterns sit around 60–65% "reversal" by Bulkowski's definition, and academic tests with transaction-cost-free benchmarks often find no excess return.
  2. The edge practitioners claim comes from *context* (trend, location at support/resistance, trendline break first, second entries) plus *asymmetric trade management* (stops one tick beyond the signal bar, targets at measured moves). That is Brooks' "trader's equation": probability × reward vs. (1 − probability) × risk. [Concept widely attributed to Brooks; not verified this session.]
  3. Bulkowski statistics are descriptive, use idealized entries and exits (breakout price to ultimate high), and include survivorship and hindsight in pattern identification. Treat them as relative rankings, not expected returns.
  4. Bottoms in Bulkowski's data have lower failure and larger moves than tops (H&S bottom: 11% failure / +45% vs. H&S top: 19% / −16%). This partly reflects the long-run upward drift of equities in bull-market samples.
- **A-share reliability** is under-researched in English-language literature. Chinese retail 量价 / 涨停 lore is anecdotal and internally contradictory (e.g., low-volume limit-up read as both bullish and bearish). Teach it as hypotheses to test, not rules.

### Gaps
- No peer-reviewed study of candlestick or chart pattern profitability specifically on China A-shares was retrieved (search could not identify a named "Lu" A-share study). Recommend the report flag this.
- Detailed result tables of LMW (2000), e.g., which patterns were significant on NYSE/AMEX vs. Nasdaq, were not extracted. Only abstract-level conclusions are confirmed.
- No independent, peer-reviewed test of Al Brooks' methods exists in the sources found.
- Post-2020 replication studies (e.g., machine-learning pattern detection) were not searched due to the tool-call budget.

---

### Appendix (within scope): Chinese–English pattern name glossary
(Standard Chinese terms; general usage, not individually sourced unless cited above.)

**Candles and bar patterns**

| English | 中文 |
|---|---|
| Candlestick | K线 / 蜡烛图 |
| Bull / bear trend bar | 阳线 / 阴线, 大阳线 / 大阴线 |
| Marubozu | 光头光脚阳线 / 阴线 |
| Doji | 十字星 |
| Long-legged doji | 长腿十字 |
| Dragonfly / gravestone doji | 蜻蜓十字 (T字线) / 墓碑十字 (倒T字线) |
| Hammer | 锤子线 / 锤头线 |
| Hanging man | 上吊线 |
| Inverted hammer | 倒锤子线 |
| Shooting star | 射击之星 / 流星线 |
| Pin bar | Pin Bar / 长影线 |
| Inside bar | 内包线 / 孕线 (harami) |
| Outside bar | 外包线 |
| Bullish / bearish engulfing | 看涨吞没 (阳包阴) / 看跌吞没 (阴包阳) |
| Piercing line / dark cloud cover | 刺透形态 / 乌云盖顶 |
| Morning / evening star | 早晨之星 (启明星) / 黄昏之星 |
| Three white soldiers / three black crows | 红三兵 / 三只乌鸦 |
| Two-bar reversal | 双K反转 |
| Signal bar / entry bar | 信号K线 / 入场K线 |

**Chart patterns**

| English | 中文 |
|---|---|
| Double top / bottom | 双顶 (M头) / 双底 (W底) |
| Triple top / bottom | 三重顶 / 三重底 |
| Head and shoulders top / bottom | 头肩顶 / 头肩底 |
| Neckline | 颈线 |
| Rising / falling wedge | 上升楔形 / 下降楔形 |
| Three pushes | 三推 |
| Flag / pennant | 旗形 / 三角旗形 |
| Ascending / descending / symmetrical triangle | 上升 / 下降 / 对称三角形 |
| Channel | 通道 |
| Trading range / box | 交易区间 / 箱体 (震荡区间) |
| Breakout pullback | 突破回踩 / 回抽确认 |
| Failed breakout | 假突破 |
| Bull trap / bear trap | 诱多 / 诱空 |
| Final flag | 最终旗形 |
| Measured move | 等距运动 / 测量目标 |

**Gaps, Wyckoff and A-share terms**

| English | 中文 |
|---|---|
| Common / breakaway / runaway / exhaustion gap | 普通缺口 / 突破缺口 / 中继 (测量) 缺口 / 衰竭缺口 |
| Island reversal | 岛形反转 |
| Wyckoff spring / upthrust | 弹簧 (终极震仓) / 上冲回落 (UT) |
| Sign of strength / last point of support | 强势信号 SOS / 最后支撑点 LPS |
| A-share limit-up bar shapes | 一字板, T字板, 炸板, 回封 |
