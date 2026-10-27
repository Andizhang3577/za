# Price Action (价格行为学) and Technical Analysis: Evidence, Criticisms, Limits, and Comparison with Other Approaches

Research date: 2026-10-27. Study dates are given inline. Most core academic evidence comes from 1992–2020. I found no major new peer-reviewed study from 2024–2026 that overturns these findings, but this search was not exhaustive for the newest literature.

## 1. What does academic research say about technical analysis profitability?

### Takeaway
The evidence is mixed and depends on the period. Some simple rules and chart patterns showed statistical signal in older data, especially before about 1990, and price momentum over 3–12 months is one of the most robust anomalies in finance. But once studies correct for data snooping and transaction costs, and require that the best rules be chosen *ahead of time*, most short-horizon technical rules lose their apparent edge. Candlestick patterns specifically have little reliable predictive power in the studies found.

### Cited Findings
**Classic positive evidence**
- Brock, Lakonishok & LeBaron (1992, *Journal of Finance*) tested 26 simple moving-average and trading-range-breakout rules on the Dow Jones Industrial Average over roughly 1897–1986 and reported that the rules had predictive power. Secondary sources disagree on whether the sample ends in 1985 or 1986. — [Sullivan, Timmermann & White, LSE record](https://researchonline.lse.ac.uk/id/eprint/119144); [Bajgrowicz & Scaillet working paper (EFMA 2008)](https://www.efmaefm.org/0EFMAMEETINGS/EFMA%20ANNUAL%20MEETINGS/2008-Athens/papers/Bajgrowicz.pdf)
- Lo, Mamaysky & Wang (2000, *Journal of Finance* 55:1705–1765; NBER WP 7613) automated chart-pattern recognition (head-and-shoulders, double bottoms, and others) using nonparametric kernel regression on U.S. stocks from 1962 to 1996. Over the 31-year sample, several technical patterns provided "incremental information" and might have some practical value. The effect was stronger for Nasdaq stocks. — [NBER w7613](https://www.nber.org/papers/w7613); [MIT abstract page](https://web.mit.edu/Alo/www/Papers/techanal.html); [CFA Institute digest](https://rpc.cfainstitute.org/-/media/documents/article/cfa-digest/2001/dig-v31-n1-811-pdf.pdf)
- Two important caveats from the same work. First, the study looks at "incremental information," meaning a change in the return distribution, not net trading profit. Second, the CFA digest notes that the authors say statistically informative patterns are not necessarily the most profitable ones, and that the classic head-and-shoulders may not be optimal. — [CFA Institute digest](https://rpc.cfainstitute.org/-/media/documents/article/cfa-digest/2001/dig-v31-n1-811-pdf.pdf)
- Park & Irwin (2007, *Journal of Economic Surveys* 21(4):786–826) surveyed 95 "modern" studies. 56 found positive results for technical trading strategies, 20 found negative results, and 19 found mixed results (about 59% / 21% / 20%). The survey warns that many studies suffer from data snooping, rules chosen after the fact, and difficulty estimating risk and transaction costs. — [IDEAS/RePEc listing](https://ideas.repec.org/a/bla/jecsur/v21y2007i4p786-826.html); [2004 AgMAS precursor report](https://ageconsearch.umn.edu/record/37487/files/AgMAS04_04.pdf); counts also quoted by a [secondary blog summary](https://thortradecopier.com/blog/does-technical-analysis-work)

**Corrections for data snooping and costs**
- Sullivan, Timmermann & White (1999, *Journal of Finance* 54:1647–1691) expanded the Brock et al. universe to about 7,846 rules over 100 years of Dow data and applied White's Reality Check bootstrap to correct for data snooping. Secondary accounts summarize the result this way: the best rules looked significant in the original sample, but performance did not hold up in the following ~10 years out of sample. — [LSE record](https://researchonline.lse.ac.uk/id/eprint/119144); [FMG discussion paper](https://www.fmg.ac.uk/publications/discussion-papers/data-snooping-technical-trading-rule-performance-and-bootstrap)
- Bajgrowicz & Scaillet (2012, *Journal of Financial Economics* 106(3):473–491) used Dow data from 1897 to 2011 and false-discovery-rate methods. They found that an investor could not have picked the future best-performing rules in advance, and that even in-sample, low transaction costs fully offset the rules' performance. Their conclusion was that the economic value of technical trading is "seriously in doubt." — [JFE abstract (SUFE mirror)](https://academicnewsletter.sufe.edu.cn/info/356896); [IDEAS](https://ideas.repec.org:443/a/eee/jfinec/v106y2012i3p473-491.html); [CFA digest 2013](https://rpc.cfainstitute.org/research/cfa-digest/2013/02/technical-trading-revisited-false-discoveries-persistence-tests-and-transaction-costs-digest)

**Momentum: the most robust "trend" evidence**
- Jegadeesh & Titman (1993, *Journal of Finance* 48(1):65–91) found that buying past 3–12-month winners and selling losers earned significant positive returns over 3–12-month holding periods, around 1% per month. The profits were not explained by systematic risk. Part of the first-year abnormal return dissipated over the following two years. — [IDEAS](https://ideas.repec.org/a/bla/jfinan/v48y1993i1p65-91.html); [NBER w7159 follow-up](https://www.nber.org/system/files/working_papers/w7159/w7159.pdf)
- Their follow-up found momentum profits continued in the 1990s, out of sample, which argues against pure data snooping. — [NBER w7159](https://www.nber.org/system/files/working_papers/w7159/w7159.pdf)
- Moskowitz, Ooi & Pedersen (2012, *Journal of Financial Economics* 104:228–250) studied 58 futures across equity indices, currencies, commodities, and bonds from 1985 to 2009. An instrument's own past 12-month return predicted its future return ("time-series momentum," i.e., trend following). The effect persisted for about a year and then partially reversed. — [SSRN](https://papers.ssrn.com/abstract=2089463); [AQR](https://www.aqr.com/Insights/Research/Journal-Article/Time-Series-Momentum)

**Candlestick patterns**
- Marshall, Young & Rose (2006, *Journal of Banking & Finance*) tested 28 candlestick signals on DJIA stocks from 1992 to 2002 with a 10-day holding period. Bullish single-day signals rarely produced positive returns. Bearish signals were followed by negative returns more often than not. Commentary notes that the few promising patterns may be spurious given how many hypotheses were tested. — [CXO Advisory summary](https://www.cxoadvisory.com/technical-trading/candlesticks-fiddlesticks/); [paper PDF mirror](https://c.mql5.com/forextsd/forum/211/Market%20Timing%20with%20Candlestick%20Technical%20Analysis.pdf)
- A 2017 *SAGE Open* study of SET50 stocks in Thailand (2006–2016) found that most candlestick reversal patterns had mean returns not statistically different from zero and could not reliably predict direction. Adding %D, RSI, and MFI filters generally did not help. — [SAGE Open 2017](https://journals.sagepub.com/doi/10.1177/2158244017736799)

**Theory: EMH vs. behavioral explanations**
- The behavioral explanation for why trends and momentum exist centers on investor biases. The disposition effect is one: investors sell winners more readily than losers. Odean's 1998 study of 10,000 discount-brokerage accounts found that winners were roughly 1.5–2 times as likely to be sold as losers, relative to the opportunity to sell; reported multipliers vary by source. This slows the incorporation of news into prices, which can produce underreaction and trends. — [Wikipedia: Disposition effect](https://en.wikipedia.org/wiki/Disposition_effect); [Barber & Odean "Courage of Misguided Convictions"](https://faculty.haas.berkeley.edu/odean/Papers/Courage/Courage.pdf)

### Inferences
- "Technical analysis works" and "technical analysis doesn't work" are both too strong. The defensible claim is narrower. Medium-horizon trend/momentum (months) has robust, out-of-sample, multi-asset support. Short-horizon pattern rules (bars, candles, intraday setups) have weak or no evidence of net profitability once costs and selection bias are accounted for.
- Price Action as taught by Al Brooks and others is mostly intraday or short-horizon and discretionary. That is the region where academic evidence is weakest and costs matter most.
- Under the efficient market hypothesis (EMH), any edge that is published or widely known should decay. Behavioral finance explains why some patterns, such as momentum and underreaction, may persist: biases like anchoring, herding, and the disposition effect are durable and arbitrage is limited. The two views are not mutually exclusive. Markets may be "adaptively" efficient, with edges appearing and fading.

### Gaps
- I did not find peer-reviewed studies that test Al Brooks-style price action specifically (e.g., "two-legged pullback," "H2/L2," "measured moves"). Discretionary methods are rarely testable in the literature.
- I did not verify the exact statistics in the Marshall, Young & Rose full text. The figures above come from summaries.
- I did not find a Menkhoff & Taylor (2007) source in search. Their survey shows that foreign exchange professionals widely use technical analysis, but I have no verified numbers from it.
- I did not survey newer (2020–2026) machine-learning studies on pattern predictability.

## 2. Evidence on retail day traders' outcomes

### Takeaway
Large-sample studies using complete exchange or regulator data are strikingly consistent. The vast majority of retail day traders lose money net of costs, fewer than 1% are reliably profitable, and persisting does not make most people better.

### Cited Findings
- **Taiwan, all investors, 1995–1999** (Barber, Lee, Liu & Odean, *Review of Financial Studies* 2009, 22(2):609–632). Individual investors' aggregate portfolio suffered an annual performance penalty of 3.8 percentage points, equal to 2.2% of Taiwan's GDP or 2.8% of total personal income. Institutions gained 1.5 percentage points per year. Virtually all individual losses traced to aggressive (market-type) orders. The total was about US$32 billion over the sample. — [IDEAS](https://ideas.repec.org/a/oup/rfinst/v22y2009i2p609-632.html); [SUFE abstract](https://academicnewsletter.sufe.edu.cn/info/354990); [Berkeley Haas newsroom](https://newsroom.haas.berkeley.edu/individual-investors-see-red-prof-terry-odean-finds/)
- **Taiwan day traders, 1992–2006** (Barber, Lee, Liu & Odean, "The Cross-Section of Speculator Skill," *Journal of Financial Markets* 2014, 18:1–24). Fewer than 1% of the day-trader population could predictably and reliably earn positive abnormal returns net of fees. Skill persists: in the following year, the top 500 traders earned 61.3 bps/day before fees and 37.9 after, while the bottom group earned −11.5 before and −28.9 after. — [IDEAS](https://ideas.repec.org/a/eee/finmar/v18y2014icp1-24.html); [eScholarship PDF](https://www.escholarship.org/uc/item/7k75v0qx)
- **Taiwan day traders, learning** (Barber, Lee, Liu, Odean & Zhang, "Learning, Fast or Slow," *Review of Asset Pricing Studies* 2020, 10(1):61–93). More than 75% of day traders quit within two years. Aggregate day-trader performance is negative. 74% of day-trading volume comes from traders with a history of losses, and 97% of day traders are likely to lose money in future day trading. Rational learning does not explain the persistence; traders keep going despite losing. — [IDEAS](https://ideas.repec.org/a/oup/rasset/v10y2020i1p61-93..html); [PUC-Rio seminar PDF](https://www.econ.puc-rio.br/uploads/adm/seminarios/Learning_fast_or_slow_180606.pdf)
- **Brazil mini-Ibovespa futures, 2013–2015** (Chague, De-Losso & Giovannetti, "Day Trading for a Living?", working paper 2019, FGV EESP TD 525 / SSRN 3423101). The sample was everyone who began day trading these futures and persisted for 300 or more days. 97% lost money. Only 1.1% earned more than the Brazilian minimum wage, and only 0.4% earned more than a bank teller's starting salary (about US$54/day). The best individual earned about US$310/day "with great risk." The authors found no evidence of learning and conclude it is "virtually impossible" for individuals to compete with HFTs (high-frequency traders), contrary to what course providers claim. The data came from Brazil's securities regulator (CVM). — [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3423101); [IDEAS (FGV)](https://ideas.repec.org/p/fgv/eesptd/525.html); [IDEAS (USP)](https://ideas.repec.org/p/spa/wpaper/2019wpecon47.html); [Quantpedia summary](https://quantpedia.com/?p=4771); [CNN Brasil](https://www.cnnbrasil.com.br/business/day-trade-o-que-e-como-fazer-e-vale-a-pena/)
- **EU retail CFDs, 2018** (ESMA product intervention). National regulators' analyses found that 74–89% of retail CFD accounts typically lose money, with average losses per client of €1,600 to €29,000. ESMA restricted leverage, imposed negative-balance protection, and mandated a risk warning stating each provider's own percentage of losing retail accounts. — [ESMA press release, 27 March 2018](https://www.esma.europa.eu/node/84933); [RPC legal summary](https://rpclegal.com/thinking/financial-services-regulatory-and-risk/esma-cracks-down-on-the-sale-of-binary-options-and-cfds-to-retail-investors)
- **China, Shanghai Stock Exchange accounts, 2016–2019** (Jones, Shi, Zhang & Zhang, "Understanding Retail Investors: Evidence from China"). Small accounts (below CNY 100k; about 58.7% of accounts) lose money from trading, through both poor stock selection and trading costs. Large accounts show some selection skill, but trading costs offset it. Small retail investors trade in a momentum-chasing style: stocks they buy fall the next day and stocks they sell rise. The pattern is stronger for young male investors. — [ABFER 2022 paper](https://abfer.org/media/abfer-events-2022/annual-conference/papers-investfin/AC22P3020_Understanding-Retail-Investors_Evidence-from-China.pdf); [AAII summary](https://www.aaii.com/images/journal/12912-Heterogeneity%20in%20Retail%20Investors.pdf)
- **U.S. households, 1991–1996** (Barber & Odean, "Trading Is Hazardous to Your Wealth," *Journal of Finance* 2000). This study of more than 66,000 households found that those who trade most earn the lowest net returns. The least active quintile earned about 18.5% per year. — [Barber & Odean "Courage" paper (review of findings)](https://faculty.haas.berkeley.edu/odean/Papers/Courage/Courage.pdf)

### Inferences
- Taiwan, Brazil, the EU, and China are very different markets, yet they produce the same picture: roughly 70–97% of retail speculators lose money and fewer than 1% are reliably profitable. That base rate should anchor a learner's expectations.
- The Taiwan 2014 paper also shows that skill exists and persists in a tiny minority. Price action is therefore not "impossible," but the odds of being in the top fraction are very low, and most quit within two years.
- In China's A-share market, small-account retail behavior (chasing short-term momentum) loses money to larger, contrarian participants. This is directly relevant to Chinese learners of 价格行为学.

### Gaps
- I did not find a CSRC (China Securities Regulatory Commission) report giving a "% of retail day traders who lose" figure. China's A-share market has T+1 settlement, so pure intraday stock day trading is not possible there. Comparable data would come from futures markets (CFFEX/SHFE) or the SSE studies above.
- I did not verify the 11.4% return for the most active quintile in Barber & Odean (2000); search did not confirm it.
- I did not verify whether the Chague et al. paper has been published in a peer-reviewed journal as of 2026. Cite it as a working paper.
- I did not fetch current U.S. broker or FINRA day-trading disclosures.

## 3. Criticisms specific to price action

### Takeaway
Price action is discretionary, and that makes it hard to falsify. Pattern labels are applied with hindsight, rules are hard to code and backtest, and the marketing ecosystem shows survivorship bias. The academic literature on testable rules (Section 1) suggests that whatever edge exists is small relative to costs at short horizons.

### Cited Findings
- Data snooping and selection bias are the central methodological problem even for *mechanical* rules. Sullivan, Timmermann & White (1999) and Bajgrowicz & Scaillet (2012) show that apparent winners in a large rule universe often vanish after correction or out of sample. Discretionary pattern reading has even more implicit degrees of freedom. — [LSE record](https://researchonline.lse.ac.uk/id/eprint/119144); [JFE abstract](https://academicnewsletter.sufe.edu.cn/info/356896)
- Lo, Mamaysky & Wang (2000) built automated kernel-regression definitions precisely because human chart reading is subjective, and they framed their algorithm as a way to make technical analysis objective and testable. — [NBER w7613](https://www.nber.org/papers/w7613)
- On survivorship bias in trading education, Chague et al. explicitly contrast their data with course providers' claims that one can day trade for a living. — [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3423101)
- Candlestick and pattern studies find that a few patterns "work" in-sample, but given the number tested, these may be spurious multiple-comparison results. — [CXO Advisory](https://www.cxoadvisory.com/technical-trading/candlesticks-fiddlesticks/)

### Inferences (no direct citations found; reasoned from the evidence above)
- **Subjectivity:** Two practitioners can label the same bar differently (e.g., "signal bar" vs. "trap"). This makes performance attribution unclear.
- **Hindsight bias:** Pattern names are easy to apply after the fact. Charts in books and courses are often selected examples, so a learner sees a curated sample of successes.
- **Backtesting difficulty:** Rules such as "context," "trend strength," and "probability is about 60%" are not precisely defined, so they cannot be fully coded. Forward-testing (paper or small live trading with a journal) is the main alternative, but it gives small samples and slow feedback.
- **Complexity of Brooks's material:** Al Brooks's books (the 2011 trilogy *Trends / Trading Ranges / Reversals*, plus the earlier *Reading Price Charts Bar by Bar*) run over 1,500 pages. They are often described as dense and hard for beginners, and their many conditional rules increase the discretionary degrees of freedom.
- **Survivorship bias among educators:** Visible "successful" educators are a filtered sample. Those who failed stop publishing. Selling courses can be more reliable income than trading, so educator success does not prove the method is profitable for students.
- **Costs and competition at short horizons:** Intraday price action competes with HFTs (high-frequency traders) and pays the spread and commissions on every trade. The Taiwan and Brazil evidence shows how decisive these frictions are.

### Gaps
- I found no peer-reviewed study testing Al Brooks's specific setups, and no audited track records of price action educators.
- I found no independent survey of price action course outcomes.
- Sourced critiques of Brooks's books (reviews etc.) were not retrieved due to the tool-call budget. The page-count and complexity points are general knowledge, not verified in this session.

## 4. Price action vs. indicator-based trading vs. value investing (and terminology: 价格 vs. 价值, 价格行为学 vs. 行为金融学)

### Takeaway
Price action, indicator-based trading, and value investing answer different questions on different time horizons. Price action and indicators both derive from past prices: indicators are mathematical transforms of price/volume, while price action reads the raw bars. Value investing estimates intrinsic value from fundamentals. Behavioral finance is an academic field explaining *why* prices can deviate from value. It is not a trading method.

### Cited Findings
- Indicators such as RSI and stochastic %D and money-flow filters did not improve candlestick pattern predictability in the Thai SET50 study (2006–2016). Indicators are not automatically a fix for pattern unreliability. — [SAGE Open 2017](https://journals.sagepub.com/doi/10.1177/2158244017736799)
- Moving-average and breakout rules, the canonical indicator-based approach, showed predictive power on the Dow in 1897–1986 (Brock et al. 1992). Out-of-sample and after costs, the value is doubtful (Sullivan et al. 1999; Bajgrowicz & Scaillet 2012). — [LSE](https://researchonline.lse.ac.uk/id/eprint/119144); [JFE abstract](https://academicnewsletter.sufe.edu.cn/info/356896)
- Systematic trend following over 12-month lookbacks (time-series momentum) is the best-supported price-based approach, across 58 futures markets from 1985 to 2009. — [SSRN](https://papers.ssrn.com/abstract=2089463)
- Behavioral finance supplies the mechanisms. The disposition effect, documented in Odean's 1998 sample of 10,000 accounts, is one source of slow price adjustment and momentum. — [Disposition effect](https://en.wikipedia.org/wiki/Disposition_effect)

### Inferences
- **Terminology clarification:**
  - **价格行为学 (Price Action):** reading raw price bars (highs, lows, closes, swing structure, support/resistance) to make short-to-medium-term trading decisions, usually discretionary. Associated with Al Brooks.
  - **价值投资 (Value Investing):** buying assets below an estimated intrinsic value based on earnings, cash flow, and assets, with a horizon of years. Associated with Graham, Buffett, and in Chinese contexts often 巴菲特/价值投资. It ignores short-term price patterns.
  - **行为金融学 (Behavioral Finance):** the academic study of how psychological biases (anchoring, herding, overconfidence, loss aversion, the disposition effect) affect investors and prices. Founded by Kahneman, Tversky, Thaler, Shiller and others. It is a theory, not a strategy, though it supplies a rationale for why price action or momentum might sometimes work.
  - The names look alike in Chinese: 价格 (price) vs. 价值 (value), and 价格行为学 vs. 行为金融学 both contain 行为 (behavior). The concepts are nonetheless distinct.
- **How they complement each other:**
  - Value or fundamental analysis decides *what* is worth owning. Price action or indicators can inform *when* to enter or exit, and where to place a stop-loss.
  - Indicators (MA, MACD, RSI) are lagging smoothings of the same price data price action reads. They add objectivity (codable, backtestable) but no new information. Price action is more granular and more subjective.
  - A practical hybrid used by many practitioners is to trade in the direction of a higher-timeframe trend (momentum evidence), use price action for entry and stop placement, and keep risk per trade small.
- On horizon, the academic evidence is strongest for months-long momentum and years-long value premia, and weakest for intraday pattern trading. A learner's choice of horizon matters more than their choice between "price action vs. indicators."

### Gaps
- I did not retrieve sources on the value premium (e.g., Fama-French HML) or its post-2007 drawdown in this session. A comparison of value vs. momentum returns needs those citations from another researcher or source.
- I found no head-to-head empirical study of "discretionary price action vs. indicator systems."

## 5. Psychological pitfalls and how disciplined traders mitigate them

### Takeaway
The data shows that retail losses come mostly from behavior: overtrading, aggressive orders, holding losers, persisting despite losses, and overconfidence. Discipline tools that limit trade frequency, enforce pre-set stops, and log results objectively directly address the documented failure modes.

### Cited Findings
- **Overtrading:** Households that trade most earn the lowest returns (Barber & Odean 2000; more than 66,000 U.S. households). — [Barber & Odean "Courage"](https://faculty.haas.berkeley.edu/odean/Papers/Courage/Courage.pdf)
- **Aggressive orders:** Virtually all Taiwan individuals' trading losses trace to aggressive orders, i.e., paying the spread or demanding liquidity. — [IDEAS RFS 2009](https://ideas.repec.org/a/oup/rfinst/v22y2009i2p609-632.html)
- **Disposition effect (holding losers, cutting winners):** Winners were roughly 1.5–2 times as likely to be sold as losers, relative to opportunity. — [Disposition effect](https://en.wikipedia.org/wiki/Disposition_effect); [Barber & Odean "Courage"](https://faculty.haas.berkeley.edu/odean/Papers/Courage/Courage.pdf)
- **Persistence despite losing / overconfidence:** 74% of Taiwan day-trading volume comes from traders with a history of losses, and their behavior is inconsistent with rational learning about their own ability. — [IDEAS RAPS 2020](https://ideas.repec.org/a/oup/rasset/v10y2020i1p61-93..html)
- **No learning by doing:** Brazilian day traders who persisted 300 or more days showed no evidence of learning. — [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3423101)
- **Herding / momentum-chasing:** Small Chinese retail accounts chase short-term momentum and lose the next day. — [ABFER paper](https://abfer.org/media/abfer-events-2022/annual-conference/papers-investfin/AC22P3020_Understanding-Retail-Investors_Evidence-from-China.pdf)
- **Leverage:** The EU CFD loss rate (74–89% of accounts) led ESMA to cap leverage and require negative-balance protection. — [ESMA](https://www.esma.europa.eu/node/84933)

### Inferences (mitigation practices; these follow logically from the failure modes above but were not themselves tested in the cited studies)
- **Pre-defined stop-loss and fixed fractional risk** (e.g., ≤1% of equity per trade) counter the disposition effect and catastrophic losses.
- **Trade journal with objective statistics** (win rate, average R, expectancy, sample size ≥100 trades) counters overconfidence and the "rational learning" failure. It forces evidence-based assessment of whether one is in the profitable 1%.
- **Daily or weekly loss limits and maximum trades per day** counter overtrading and revenge trading.
- **Low leverage, and limit orders where appropriate**, reduce cost drag (the Taiwan aggressive-order finding).
- **Written trading plan / checklist** reduces discretionary drift and hindsight rationalization.
- **Paper-trade or small size until a statistically meaningful forward record exists.** Given the 97% loss base rate, a learner should demand evidence before scaling up.
- **Define a "stop rule" for the trading career itself** (e.g., stop if not net-profitable after N months or N trades). Barber et al. show most losing traders continue far longer than rational learning implies.
- **Realistic expectation:** for most learners, the most valuable use of price action may be as a timing and risk-management tool layered on longer-horizon, evidence-supported strategies, not as a primary income source.

### Gaps
- I found no rigorous study showing that trading journals or psychology training improve retail trader profitability. The mitigation practices are practitioner consensus, not empirically validated.
- Sources on specific biases (anchoring, herding) in trading contexts beyond the disposition effect were not fetched. Kahneman & Tversky / Shiller citations would need to come from elsewhere.
