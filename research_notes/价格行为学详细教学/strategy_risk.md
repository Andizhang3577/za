# 价格行为学交易系统：形态、入场、出场、风险管理与学习路径（股票，美股 + A股）

> 研究说明（写给报告撰写者）：本环境的出站代理拒绝连接 brookstradingcourse.com、nexusfi.com、daxiapi.com 等站点（CONNECT 403），因此无法抓取全文。下面的引用基于搜索引擎返回的片段和摘要。很多“Brooks 规则”出自 Brooks Trading Course 论坛问答或第三方总结，不是 Brooks 书中的原文，文中都已注明。数值算例是我根据引用的公式推算的，放在 “Inferences” 部分，没有当作引用事实。

## 1. 高胜率形态及分步规则（H2/L2 回调、首次回调到 20 EMA、突破与突破回踩、失败突破、楔形、双顶/双底、区间高抛低吸）

### Takeaway
Brooks 体系最可靠的顺势形态是牛市趋势中的两腿回调（H2，熊市对应 L2）。逆势形态（楔形、双顶/双底、失败突破）胜率较低，需要更大的盈亏比，最好等到二次入场。交易区间里，突破尝试大多失败（常被引用的数字约为 80%），因此做法是在区间上 1/3 卖、下 1/3 买，并交易失败突破。

### Cited Findings
**H1/H2/L1/L2（趋势回调）**
- 定义：回调开始后，第一根高点超过前一根 K 线高点的 K 线是 H1；H1 的上涨尝试失败、回调形成第二腿后，再次出现高点超过前一根 K 线高点的 K 线就是 H2。H2 是上升趋势中两腿回调之后的顺势做多信号 K 线 — [NexusFi: Two-legged pullback trading](https://nexusfi.com/a/strategies/two-legged-pullback-trading)
- 同一来源称两腿回调是 Brooks 最可靠的顺势入场，以 20 EMA 作为参考位，并提醒 K 线计数不是绝对的；它还转述 Brooks 的观点，认为 H2 是新手最安全的买入形态 — [NexusFi](https://nexusfi.com/a/strategies/two-legged-pullback-trading)
- 一个 TradingView 社区脚本（不是 Brooks 本人编写）把它写成机械规则：价格在上升的 EMA 之上，出现一串更低的高点，信号 K 线收盘位于 K 线区间 50% 以上，目标为 1:2 盈亏比或前一个主要波段高点 — [TradingView script TIyW8vKv](https://www.tradingview.com/script/TIyW8vKv)
- 第二入场的中文定义：第一入场之后价格再回调一次，再次突破对应位置时触发第二入场 — [bilibili《如何数入场计数【价格行为学】》](https://www.bilibili.com/video/BV1wV8Z6yEM7/)

**首次回调到 20 EMA / 20 缺口 K 线（20-gap bar）**
- 20 缺口 K 线买入形态：市场完全运行在均线之上约 20 根 K 线、一直没有触及均线，交易者在均线处挂限价买单，押注价格回到均线时反转向上；论坛把它描述为“大约 20 根 K 线后第一次回调到 EMA” — [BTC forum: 20 gap bar buy setup](https://brookstradingcourse.com/support-forum/14-trends/20-gap-bar-buy-setup); [BTC forum: v 11b gaps](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/v-11b-gaps-20-gap-bar-buy-set-up/)
- 这个形态不同于“均线缺口 K 线”（MAG）。只有趋势仍在运行时才成立；有学员引用 Brooks 的说法，认为之后测试高点的概率约为 70–75%，但也有好看的均线缺口 K 线没能测试高点的情况 — [同上论坛帖](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/v-11b-gaps-20-gap-bar-buy-set-up/)
- 有第三方指标说明称 Brooks 认为 20 周期 EMA 是他最重要的均线，这句话我无法在 Brooks 的原始资料中核实 — [TradingView: Price Action Brooks Pro](https://kr.tradingview.com/script/NcOnkKwT-Price-Action-Brooks-Pro)

**突破、突破回踩与测量目标**
- 交易区间突破后，交易者预期一次测量移动，幅度约等于区间高度；大多数底部都是双底的变体，趋势通常至少有第二腿，第二腿大小与第一腿相关 — [Brooks Trading Course (p=121544)](https://www.brookstradingcourse.com/?p=121544)
- 一段论坛回答引用 Brooks 的观点：需要先有突破，再有跟随 K 线（follow-through），才能认为测量移动的概率超过 50% — [Brooks Trading Course 摘要（同上搜索结果）](https://www.brookstradingcourse.com/?p=121544)
- 在一段实盘视频文字稿中，Brooks 描述了一个更低低点的双底，随后是三腿的楔形牛旗。他等到一根 K 线收盘在均线之上并高于当日高点、下一根跟随 K 线确认后，才在信号 K 线高点上方 1 tick 买入 — [Brooks Trading Course (p=121544)](https://www.brookstradingcourse.com/?p=121544)
- 非 Brooks 来源（CMC Markets）：旗杆投影的测量移动被视为最低预期，强趋势常常超过它 — [CMC Markets: Bull flag](https://www.cmcmarkets.com/en/technical-analysis/bull-flag-pattern)
- Lance Beggs（YTC）的形态分类：TST（测试支撑/阻力）、BOF（突破失败）、BPB（突破回踩）、BP（普通回调）；不同形态的止损放法不同。他用 30 分钟图找支撑阻力，用 3 分钟图交易，有时用 1 分钟图找入场时机 — [emofid（波斯语 YTC 指南）](https://learning.emofid.com/?p=55287); [NexusFi YTC thread](https://nexusfi.com/beginners-introductions-tutorials/12944-ytc-price-action-trader-getting-going.html)
- Bob Volman《Understanding Price Action》的五种形态：pattern break（形态突破）、pattern break pullback（突破回踩）、pattern break combi（突破组合）、pullback reversal（回调反转）、trade-for-failure（交易失败）。书中针对 EURUSD 5 分钟图设定了 10/20 点（pip）的止损/目标组合 — [Babypips forum](https://forums.babypips.com/t/bob-volman-for-the-d1-chart/234239)
- Volman 的“双十字星”（double doji）：回调末端、贴近 EMA 处出现几根十字星，价格突破这组十字星时入场（第三方总结） — [TradingView VN idea](https://vn.tradingview.com/chart/GOLD/92cF13U5/)

**失败突破 / 交易区间高抛低吸**
- 约 80% 的交易区间突破尝试会失败：价格突破、延续几根 K 线，然后回到区间内。Brooks 把这归因于市场惯性（倾向于继续之前的行为）。他在区间上 1/3 找卖点，在下 1/3 找买点。失败突破被称为区间内胜率最高的形态 — [NexusFi: Trading range strategies](https://nexusfi.com/a/strategies/trading-range-price-action-strategies)
- 但论坛用户指出，Brooks 也说过长时间区间后的第一次突破成功率约 50%。这些百分比应视为“加权证据”，不是精确数字。在区间极端位置要获得高胜率，需要宽止损加分批建仓 — [BTC forum: breakout probability](https://brookstradingcourse.com/support-forum/general-trading-discussion/breakout-probability); [BTC forum: trading range and BO mode](https://brookstradingcourse.com/support-forum/18-trading-ranges/trading-range-and-break-out-mode)

**楔形反转与双顶/双底**
- 楔形是 Brooks 主要的逆势形态：第三推动的动能变弱，趋势在第三推动处失败。推动之间必须有有意义的回调分隔，单根内包 K 线不算。楔形失败后的延续交易常常走出约等于楔形高度的测量移动（第三方总结） — [NexusFi: Wedge reversals](https://nexusfi.com/a/strategies/wedge-reversals-price-action)
- 楔形既可以是反转（楔形顶/底），也可以是延续（楔形旗）。如果楔形顶先向上假突破再失败，做空的胜算比单纯楔形更高 — [BTC forum: 24d wedges](https://www.brookstradingcourse.com/support-forum/24-wedges/video-24d-wedges-understanding-wedges-given-the-context-at-left/)
- 第三方实例（BTC）：在楔形底出现强阳反转 K 线后入场，止损放在楔形低点下方，目标为当日高点 — [TradingView BTC review](https://tw.tradingview.com/chart/BTCUSDT.P/68fPcX6E-Market-Makers-Baited-Traders-Into-Perfect-Reversals)
- Brooks 也会用“三腿下跌”标注楔形顶，第三腿即反转，这容易造成计数混淆 — [BTC forum](https://www.brookstradingcourse.com/support-forum/24-wedges/sometimes-al-points-out-a-wedge-top-and-says-3-pushes-down/)

### Inferences
- 各形态的分步规则可以综合如下（规则来自上面的引用，具体参数是我建议的默认值）：
  1. **H2 做多**：(a) 背景是牛市趋势，价格在上升的 20 EMA 之上，有更高高点和更高低点；(b) 回调出现两腿，第二腿通常靠近或触及 20 EMA；(c) 信号 K 线是阳线、收盘在上半部（最好在上 1/3）、影线小；(d) 在信号 K 线高点上方 1 tick 挂买入止损单；(e) 初始止损放在信号 K 线低点下方（或整段回调低点下方）；(f) 目标先看前高（测试高点），然后是 2R 或测量移动；(g) 如果 1–2 根 K 线内没有成交就撤单。L2 做空规则完全对称。
  2. **首次回调到 20 EMA / 20 缺口 K 线**：趋势远离均线约 20 根 K 线后，第一次触及均线是高胜率的顺势入场；之后测试趋势极点的概率高（论坛引用约 70–75%），但它更像“测试前高”，未必能突破前高。
  3. **突破回踩**：价格从区间突破，并有跟随 K 线（两根以上的强趋势 K 线），然后第一次回踩突破位置（区间上沿或突破 K 线高点附近）。在回踩出现 H1/H2 时入场，止损放在回踩低点下方，目标是区间高度的测量移动。
  4. **失败突破反转**：价格突破区间高点（或前高、楔形顶），但没有跟随 K 线，随后出现阴线反转 K 线并收回区间内。在反转 K 线低点下方挂卖出止损单，止损放在突破极点上方，目标是区间中部或另一侧边界。
  5. **楔形反转**：三推动结构，每推动之间有可辨识的回调，第三推动动能衰竭（K 线变小、影线变长、与通道线重叠）。等待强反转 K 线后，在反转 K 线外侧挂止损单入场。由于胜率通常不超过 40%（见第 3 节），最好等第一次反弹后的二次入场（更低高点 / 更高低点）。目标至少 2R，或回到楔形起点。
  6. **双底（双顶）**：在下跌趋势或区间底部，第二次测试前低（价格略高于或略低于前低都可以）并出现阳线反转 K 线，在该 K 线高点上方买入，止损放在双底下方，目标是颈线及颈线以上的测量移动。“双底牛旗”（趋势中的回调双底）属于顺势形态，胜率高于逆势的趋势反转双底。
  7. **区间高抛低吸**：只在区间上 1/3 做空、下 1/3 做多，区间中部不交易。目标是区间中部或对侧边界（剥头皮，1R 或更小）。止损要宽（放在区间外），或者分批建仓。
- 对股票来说，上述规则可以直接用在日线上（K 线换成日 K），止损用前一日或信号日的高低点；A 股的调整见第 6 节。

### Gaps
- 无法取得 Brooks 书中（如《Trading Price Action Trends》）关于 H2/L2、楔形、双底止损位置和目标的逐字规则，代理拒绝访问 brookstradingcourse.com 原文；以上大多来自论坛转述和第三方总结。
- 没有找到各形态在美股个股日线或 A 股上可靠的独立回测胜率数据。

## 2. 入场方法：信号 K 线外的止损单 vs 限价单（Brooks 对两类交易者的区分）

### Takeaway
新手应在信号 K 线外侧用止损单入场（顺势突破信号 K 线时成交）。用限价单“在 K 线下方买、在 K 线上方卖”是有经验交易者的做法，主要用于交易区间、强趋势中的回调和 20 缺口 K 线这类场景，代价是止损更远、成交不确定。

### Cited Findings
- 论坛解释：Brooks 说的“buying below the bar”是用限价单在 K 线下方买入，例如在牛市微通道里买第四根 K 线的低点。这正是新手应该避免的做法，因为保护性止损必须放在更早的 K 线下方 — [BTC forum: video 09a slide 5](https://www.brookstradingcourse.com/support-forum/09-pullbacks-and-bar-counting/video-09a-slide-5/)
- 限价单经常不会成交，因为它押注市场先朝不利方向运行；但在短暂回调中，如果止损入场所需的信号 K 线是阴线（导致错过交易），限价单就有用。也有交易者发现，趋势日里止损单入场有效，而限价单一整天都不成交 — [BTC forum: how to know when to enter using a stop vs limit](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/how-to-know-when-to-enter-using-a-stop-vs-limit/)
- 论坛成员的经验规则：信号出现后，止损单应在 2 根 K 线内成交，否则撤单，等新信号；无论用哪种入场方式，关键都是把止损放对位置 — [BTC forum: placing orders](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/placing-oders/); [BTC forum: how do people enter with limit order](https://www.brookstradingcourse.com/support-forum/32-orders/how-do-people-enter-with-limit-order/)
- Brooks 实盘示例：在信号 K 线高点上方 1 tick 买入，前提是已出现收盘确认和跟随 K 线 — [Brooks Trading Course (p=121544)](https://www.brookstradingcourse.com/?p=121544)
- 20 缺口 K 线形态的标准入场就是在均线处挂限价买单，是限价入场的典型例子 — [BTC forum: 20 gap bar](https://brookstradingcourse.com/support-forum/14-trends/20-gap-bar-buy-setup)

### Inferences
- 实用区分：**止损单入场者**要求市场先朝自己的方向运行（确认），胜率稍高，但入场价更差，适合趋势、突破和反转 K 线。**限价单入场者**押注价格回归（区间边界、均线回调、强趋势中的一两根逆向 K 线），入场价更好，但需要更宽的止损、分批建仓的计划，以及对背景的准确判断。
- 对美股日线波段交易：在信号日高点上方挂 buy stop（GTC 或当日有效），次日触发即入场。如果次日跳空高开远超信号日高点，可以考虑放弃，因为实际风险变大，盈亏比恶化。
- 对 A 股：没有“盘中买入止损单”的原生条件单时，多数券商 App 提供“条件单 / 突破买入”，可以模拟这种入场方式。但 T+1 意味着当日入场后无法当日止损（见第 6 节），因此 A 股更倾向于收盘确认后、次日入场。

### Gaps
- 未取得 Brooks 原文中“stop-entry traders vs limit-order traders”的直接表述（例如他在《Trading Ranges》中关于机构用限价单逆势加仓的论述）。

## 3. 止损、目标、分批进出、移动止损与 Brooks“交易者方程”

### Takeaway
交易者方程是：胜率 × 收益 > 败率 × 风险。经验法则是：顺势的高胜率形态（≥60%）可以做 1:1；逆势或反转形态（≤40%）至少需要 2:1。不确定胜率时，目标设为风险的 2 倍。目标通常是前一波段高低点、测量移动或 1R/2R。

### Cited Findings
- 方程写作 (胜率) × (收益) > (败率) × (风险)。论坛引用课程中的例子：60% 胜率的 1:1 交易，6 > 4；40% 胜率的 2:1 交易，8 > 6 — [BTC forum: 37b slide 28 traders equation](https://www.brookstradingcourse.com/support-forum/37-how-to-trade/37b-slide-28-traders-equation/); [BTC forum: clarifying the 40 60 rule](https://www.brookstradingcourse.com/support-forum/30-traders-equation-and-probability/clarifying-the-40-60-rule-possible-contradiction/)
- Brooks 建议在胜率不确定时把收益设为风险的约 2 倍。有些形态 1:1 的胜率至少 60%，而大多数反转 1:1 的胜率不超过 40% — [MoneyShow transcript](https://moneyshow.com/articles/videotranstr-26221); [BTC forum](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/probability-and-riskreward/)
- 批评意见：胜率和收益不是相互独立的变量，目标越大，达成概率通常越低；“40% 达到 1:1”不等于“40% 达到 2:1” — [BTC forum: probability and risk/reward](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/probability-and-riskreward/)
- 论坛还讨论了“初始风险 vs 实际风险”：交易者方程应该用实际风险（入场价到止损的距离）还是初始风险（信号 K 线区间）来算 — [BTC forum: initial vs actual risk](https://www.brookstradingcourse.com/support-forum/36-trade-management-and-taking-profits/traders-equation-based-on-actual-risk-or-initial-risk/); [BTC forum: 2x actual risk](https://www.brookstradingcourse.com/support-forum/34-actual-risk/math-is-good-for-2x-actual-risk-profit/)
- 测量移动目标：区间突破后预期的移动幅度约等于区间高度；第二腿与第一腿的大小相关 — [Brooks Trading Course (p=121544)](https://www.brookstradingcourse.com/?p=121544)
- 区间极端位置要得到高胜率，需要宽止损加分批建仓 — [BTC forum: breakout probability](https://brookstradingcourse.com/support-forum/general-trading-discussion/breakout-probability)
- 晚入场的数学问题（入场越晚，风险越大、剩余空间越小）是论坛的专门话题 — [BTC forum: maths of entering late](https://www.brookstradingcourse.com/support-forum/general-trading-discussion/maths-of-entering-late/)

### Inferences
- **数值例（美股日线 H2）**：股票 XYZ 处于上升趋势，回调到 20 日 EMA 附近，信号日高 101.00、低 98.50。在 101.01 挂买入止损单，止损 98.49，每股风险约 2.52 美元（1R）。目标一：前高 104.00（约 1.2R）；目标二：2R = 106.05。用交易者方程检验：假设 2R 目标的胜率为 45%，0.45 × 2 = 0.90 > 0.55 × 1 = 0.55，期望值为 +0.35R/笔，可以交易；如果只做 1R 而胜率 55%，0.55 > 0.45，期望值为 +0.10R/笔，优势很薄。
- **分批出场**：常见做法是 1R 处平掉一半仓位，剩余仓位止损移到保本，再以前一日（或前一根 K 线）低点、或 20 EMA 收盘跌破作为移动止损，持有到 2R 或测量移动目标。
- **分批进场**（只适用于有经验的区间交易者）：在区间下 1/3 先建仓 1/2，在更低处（仍在区间内）加仓 1/2，统一止损放在区间外。总风险必须预先按满仓计算，不能事后扩大。
- **移动止损**：趋势中把止损移到每个新形成的更高低点下方（波段移动止损）；强趋势也可以用“收盘跌破 20 EMA 离场”。

### Gaps
- Brooks 关于“剥头皮 vs 波段”的具体实际风险倍数（如 E-mini 中“风险 2 点、目标 4 点”）未能从原文核实。
- 没有找到美股个股的公开统计，用于确认 60%/40% 这类经验数字。

## 4. 仓位规模、单笔风险（1–2% 规则）、期望值、胜率与盈亏比权衡、回撤控制

### Takeaway
先根据市场结构设定止损（这决定 1R），再按账户权益的固定百分比（通常 0.5–2%）倒推仓位，最后用 R 倍数记录每笔交易并计算期望值（平均 R）。期望值至少需要 30–100 笔交易样本才有意义。

### Cited Findings
- Van Tharp 把 R 定义为由初始止损决定的初始风险，每笔盈亏都以 R 倍数表示；期望值是系统产生的平均 R 倍数，需要 30–100 个样本才有意义 — [vantharp.com](https://vantharp.com/?p=10928); [Traders.com: Tharp system design](https://traders.com/Documentation/FEEDbk_docs/2007/01/Abstracts_new/Tharp/tharp.html)
- Tharp 的例子：一年约 60 笔交易、期望值 1.5R，如果每笔风险当前权益的 1%，一年可以“轻松做到 100%”。这是作者的演示性说法，不是保证 — [vantharp.com](https://vantharp.com/?p=10928)
- 仓位计算步骤：止损必须基于市场结构，再根据止损距离算出每单位的美元风险。例如 10 万美元账户、1% 风险，最大美元风险为 1,000 美元，仓位按 1R = 1,000 美元来确定 — [NexusFi: R-multiples](https://nexusfi.com/a/risk-management/r-multiples)
- 批评：只看平均 R 不够，需要同时考虑胜率和 R 倍数分布；胜率和 R 都不同的两个系统可以有相同的期望值（约 1.1R）；止损滑点或不执行止损时，亏损会超过 -1R。有人认为 Ralph Vince 的资金管理数学更严谨（个人观点） — [NexusFi thread](https://nexusfi.com/showthread.php?p=57165); [NexusFi metrics/journals](https://nexusfi.com/psychology-money-management/4884-trading-metrics-journals-record-keeping-2.html)
- R 倍数被称为“唯一可跨账户、跨品种扩展的绩效指标” — [CrossTrade: R-Multiple](https://crosstrade.io/learn/performance-metrics/r-multiple)

### Inferences
- **仓位公式**：股数 = (账户权益 × 风险%) ÷ (入场价 − 止损价)。例：账户 50,000 美元、风险 1% = 500 美元；套用上一节 XYZ 的例子，每股风险 2.52 美元，仓位为 500 ÷ 2.52 ≈ 198 股（约 2 万美元市值，占账户 40%）。还要检查单只股票市值上限（例如不超过账户的 25–50%）以及日均成交量。
- **期望值公式**：E = 胜率 × 平均盈利 R − 败率 × 平均亏损 R。胜率与盈亏比的权衡：盈亏平衡胜率 = 1 ÷ (1 + 盈亏比)。1:1 需要大于 50%，2:1 需要大于 33.3%，3:1 需要大于 25%。
- **回撤控制**（实践建议，非引用）：在 1% 风险下，连亏 10 笔约回撤 9.6%；在 2% 风险下约为 18.3%。可以设定日/周/月熔断，例如单日亏损 3R 停止交易、月度回撤 6–8% 时把风险减半、10% 时暂停并复盘。新手实盘初期建议用 0.25–0.5% 风险。
- 要报告每笔交易的“实际 R”，包括滑点和跳空。股票隔夜跳空经常让亏损超过 -1R，所以日线波段交易者在算仓位时要预留缓冲。A 股跌停无法卖出时尤其如此。

### Gaps
- 未取得 Van Tharp 关于“百分比风险模型”具体推荐区间的原文页面（只有二手转述）。

## 5. 周期选择：日内（5 分钟图，Brooks 主做 E-mini）vs 股票日线波段；个股 vs 指数期货/ETF

### Takeaway
Brooks 主要用 5 分钟图教学（E-mini），但他强调同一套逻辑适用于所有市场和周期，并在《Reading Price Charts Bar by Bar》中讲到日线/周线、多只股票的日内波段和基于日线的期权交易。对兼职的股票交易者来说，日线波段更现实；日内交易更适合流动性好的指数 ETF 或大盘股。

### Cited Findings
- Brooks 用 5 分钟 K 线图阐述基本原则，同时讨论日线和周线；书中涉及多只股票的日内波段交易和基于日线的期权买入 — [Wiley《Reading Price Charts Bar by Bar》简介 via exlibris](https://www.exlibris.ch/de/buecher-buch/english-books/al-brooks/reading-price-charts-bar-by-bar/id/9781394378128/)
- 《Trading Price Action Reversals》指出价格行为分析适用于所有周期，日内、日线、周线、月线适用不同的技巧 — [O'Reilly: Trading Price Action Reversals](https://oreilly.com/library/view/trading-price-action/9781118172308)
- 视频摘要称 Brooks 每天收盘后标注图表、为次日交易做准备，并强调他对所有市场和周期的方法一致 — [chaindesk summary: 5 Steps to Finding Today's Trades](https://chaindesk.ai/tools/youtube-summarizer/5-steps-to-finding-todays-trades-AGyOld9iY8U)
- 《Trading Ranges》讨论了交易区间、突破、订单管理和交易数学 — [Booksamillion](https://www.booksamillion.com/p/Trading-Price-Action-Ranges/Al-Brooks/9781118066676)
- YTC 用 30 分钟图找结构、3 分钟图交易；Volman 的书针对 5 分钟图 — [NexusFi YTC](https://nexusfi.com/beginners-introductions-tutorials/12944-ytc-price-action-trader-getting-going.html); [Babypips](https://forums.babypips.com/t/bob-volman-for-the-d1-chart/234239)

### Inferences
- **日内（5 分钟图）**：需要盘中全时段盯盘，适合 SPY/QQQ、ES/MES 期货或日均成交额很大的个股。每日交易次数多，统计样本积累快，但手续费和滑点占比高。美股个股日内还要注意 PDT 规则（保证金账户低于 25,000 美元时的日内交易次数限制；我没有在本次检索中核实其 2026 年现状）。
- **日线波段**：每天收盘后花 30–60 分钟扫描和挂单即可。止损更宽（通常 1–3 个 ATR），仓位相应更小。个股受财报跳空影响，规则上应避开财报前后，或者减仓。
- **个股 vs 指数**：指数和 ETF 的价格行为更“干净”，没有单一公司事件风险，也是 Brooks 统计经验的来源。个股更容易出现跳空、消息驱动的趋势和流动性问题，需要加入流动性过滤（如日均成交额）和事件过滤。
- **多周期**：用周线/日线确定背景（趋势还是区间、在区间的哪个位置），用日线/60 分钟图找信号。

### Gaps
- 没有找到 Brooks 关于“个股日线波段专门规则”的原文；brookspriceaction.com 无法访问。

## 6. A股适配：T+1、10%/20% 涨跌停、做空困难

### Takeaway
A股可以使用价格行为框架，但执行层要改写：以只做多为主，以日线/周线收盘确认为主，盘中信号降级为“观察”。还要计算“次日才能止损”和“跌停无法成交”带来的额外风险，并据此给仓位打折。

### Cited Findings
- 涨跌幅限制：主板 ±10%，创业板/科创板 ±20%，北交所 ±30%。涨停时买单可能排不上，跌停时卖单可能无法成交，因此回测不能假设信号一定按价成交 — [tessl.io: Vibe-Trading regulatory knowledge](https://tessl.io/registry/skills/github/HKUDS/Vibe-Trading/regulatory-knowledge); [叩富网: A股交易规则](https://licai.cofool.com/ask/qa_6937546_1_3.html)
- 2026 年变化（新闻报道）：沪深北交易所新规于 2026 年 7 月 6 日起施行，主板 ST/*ST 股涨跌幅由 5% 放宽到 10%。深交所在创业板引入做市商制度。没有找到 T+0 已推行的官方信息；有评论认为可能分步推行 T+0、或在科创板/创业板取消涨跌幅限制，但这只是评论观点 — [虎嗅](https://www.huxiu.com/article/4872571.html); [同花顺 2026-07-05](https://stock.10jqka.com.cn/20260705/c677954625.shtml)。注意：旧资料（如叩富网）仍写 ST 为 ±5%，与 2026 年 7 月以后的规则冲突，以交易所公告为准。
- T+1：当日买入次日才能卖出。回测中常见的错误是当日出信号、当日平仓，这会虚增收益；日线回测通常按次日开盘价成交。融券费率高、券源有限，只做多更现实 — [tessl.io](https://tessl.io/registry/skills/github/HKUDS/Vibe-Trading/regulatory-knowledge)
- A 股适配框架（大虾皮AI投资数据，2026-06-15，“Al Brooks 价格行为交易”系列）：A 股可以借鉴 Brooks 框架，但必须把 T+1、涨跌停、尾盘确认、次日承接和不可成交止损写进执行规则。流程是结构判断 → 收盘确认 → 次日承接 → 仓位折扣 → 可执行止损。信号分为观察、计划、确认三级。盘中突破如果当天收回，风险会延迟到次日，因此盘中触发只算观察级 — [daxiapi.com 文章（据搜索摘要，全文无法访问）](https://daxiapi.com/article/al-brooks-price-action/2026-06-15-09-a-share-t1-limit-move-close-confirmation/)
- T+1 对价格形态的影响：研究发现 A 股存在“低开高走”模式，T+1 是其长期存在的基础之一；T+1 降低成交量和价格波动；市场波动越大，T+1 约束越强，日内与隔夜的反转效应越明显 — [SciOpen《经济学报》2022 论文 PDF](https://www.sciopen.com/local/article_pdf/10.26599/CJE.2022.9300102.pdf); [PHBS: A Unique T+1 Trading Rule in China](https://english.phbs.pku.edu.cn/info/3571/24361.htm); [Emerald CFRI](https://emerald.com/insight/content/doi/10.1108/CFRI-12-2016-0130/full/html); [上财学报](https://qks.shufe.edu.cn/J/ArticleQuery/A67fdee67-f823-44ad-8489-d42bcfae03ae)
- 社区观点：雪球用户认为“只要存在多空博弈，都适用价格行为”（个人观点，未经核实） — [雪球](https://xueqiu.com/3633211179/333953948)
- 散户容易忽略的细节：涨跌停排队、T+1、委托单失效、除权除息、撤单时限 — [悦牛证券](https://ag.yueniuzq.com/stock/a-share-trading-rules-neglected-details/)

### Inferences
- **A 股价格行为执行规则**（综合以上引用）：
  1. **只做多**：L2、楔形顶、双顶等做空信号只用于“不买 / 减仓 / 离场”，不开空仓。
  2. **主周期为日线，背景看周线**：周线上升趋势或区间下 1/3 才考虑买；周线下跌趋势中只做极少量的二次入场反转。
  3. **收盘确认**：信号 K 线必须是收盘确认的日 K（阳线、收在上 1/3）。在尾盘（约 14:30–15:00）确认后下单，或次日用条件单在信号日高点上方触发。
  4. **次日承接**：入场后第二天如果不能站稳信号日高点（例如收盘跌回信号 K 线内部），按“失败信号”处理，第二天即离场，不等止损。
  5. **可执行止损与仓位折扣**：止损放在信号日低点下方。但由于 T+1，当日入场后当天无法止损，最坏情况是入场日收在接近跌停（主板 −10%）的位置，次日再跌停。因此计算仓位时，“风险距离”应取 max(结构止损距离, 预估跳空/跌停风险)。例：结构止损 6%、账户风险 1%，理论仓位 = 1% ÷ 6% ≈ 16.7%；按最坏 1 个跌停（10%）+ 1 个低开计算可能达到 15%，则仓位应降到 1% ÷ 15% ≈ 6.7%。创业板/科创板（±20%）需要进一步折扣。
  6. **涨停相关**：涨停板上无法按突破价买入，不应追涨停排队；涨停后的“突破回踩”（回到涨停 K 线实体中上部并出现 H1/H2）才是价格行为意义上的入场点。
  7. **避免盘中假突破**：A 股“低开高走”和日内/隔夜反转效应意味着盘中突破未必可靠，应以收盘为准。
- **目标与离场**：沿用前高、测量移动、2R；移动止损用前一日低点或收盘跌破 20 日 EMA。
- **回测**：信号日收盘生成信号，次日开盘价（或次日触发价）成交；当日不得平仓；遇一字涨停不得买入，遇跌停不得卖出（顺延到次一可成交日）。

### Gaps
- 没有找到知乎上系统讨论 A 股价格行为的高质量文章（本次使用的美国区搜索引擎对中文社区覆盖有限）。
- 融券/转融通在 2026 年的最新状态未能核实。
- 没有可靠数据说明 Brooks 形态在 A 股日线上的胜率。

## 7. 学习路线：图表复盘、逐 K 线回放、交易日志、回测、模拟交易、常见新手错误

### Takeaway
从“读图”走向“交易”需要分阶段推进：先标注历史图表、用逐根 K 线回放练习决策，再用 R 倍数记录日志和回测，然后模拟盘，最后小风险实盘。最常见的失败原因是过度交易、忽视背景（趋势/区间），以及到处看到形态。

### Cited Findings
- TradingView 的 Bar Replay 可以回到过去某天、隐藏之后的走势、逐根 K 线推进，在不承担风险的情况下练习入场和出场；逐根复盘历史图表有助于识别重复出现的形态 — [Samir Dash Substack: 3 ways to practice price action](https://samirdash.substack.com/p/3-ways-to-practice-price-action-without)
- 常见错误：到处看到形态导致入场过多、忽视市场结构、忽视大趋势 — [同上](https://samirdash.substack.com/p/3-ways-to-practice-price-action-without)
- NexusFi 交易日志：一位交易者把问题归结为“过度交易 + 不理解价格行为”，改进方法是交易前使用纸质检查清单、限制交易次数；另一位记录了报复性交易、不坚持判断、同时看太多东西 — [NexusFi p=827933](https://nexusfi.com/showthread.php?p=827933); [NexusFi p=822211](https://nexusfi.com/showthread.php?p=822211)
- Brooks 课程论坛成员通过录屏发现自己在违背课程规则交易（FOMO/报复/过度交易） — [BTC forum: i donot like what i see](https://www.brookstradingcourse.com/support-forum/trading-journals/i-donot-like-what-i-see/)
- Brooks 每天收盘后标注图表为次日做准备 — [chaindesk summary](https://chaindesk.ai/tools/youtube-summarizer/5-steps-to-finding-todays-trades-AGyOld9iY8U)
- 期望值至少需要 30–100 笔样本 — [vantharp.com](https://vantharp.com/?p=10928)
- 模拟盘工具（A 股）：乐咕乐股提供 A 股模拟交易 — [legulegu](https://legulegu.com/mock-trading/a-share)
- 论坛提醒：Brooks 的百分比是“加权证据”，不是精确数值 — [BTC forum: breakout probability](https://brookstradingcourse.com/support-forum/general-trading-discussion/breakout-probability)

### Inferences
- **建议的 6 阶段路线**（时长为建议值）：
  1. **第 1–4 周，概念与标注**：读 Brooks 三部曲中的趋势卷，或中文版《价格行为交易》系列。每天在 5–10 张日线图上标注趋势/区间、H1/H2/L1/L2、楔形、双底/双顶、测量移动。
  2. **第 5–8 周，逐 K 线回放**：用 TradingView Bar Replay（美股）或同花顺/通达信的历史回放（A 股），每根 K 线写下“多/空/观望 + 理由”，每周至少 200 根日 K。只练 2 种形态：H2/L2 顺势回调，加上区间失败突破。
  3. **第 9–12 周，规则化与回测**：把每种形态写成书面规则（背景、信号 K 线、入场、止损、目标），在 50–100 个历史样本上手工回测，记录 R 倍数、胜率和最大连亏。期望值 > 0.2R 才保留。
  4. **第 13–20 周，模拟盘**：实时下单（含条件单），至少 30–50 笔。日志字段包括日期、标的、周期、背景（趋势/区间/位置）、形态、信号 K 线质量、入场/止损/目标、R 倍数、是否遵守规则、情绪、截图。
  5. **第 21 周起，小风险实盘**：单笔风险 0.25–0.5%，每日最多 2–3 笔（日内）或同时持仓 3–5 只（日线）。连续 50 笔遵守规则、期望值为正，再逐步把风险提到 1%。
  6. **持续复盘**：每周按形态统计 R 分布，淘汰负期望形态；每月检查回撤是否触及熔断线。
- **新手常见错误清单**：过度交易（在区间中部交易、每根 K 线都想交易）；对单根 K 线过度解读而忽视背景；逆势抄底摸顶（用反转形态对抗强趋势，而不是等二次入场）；止损放得太近（在信号 K 线内部）或事后移远止损；不算交易者方程（胜率低的反转只做 1:1）；盈利过早离场、亏损死扛；A 股追涨停、盘中假突破、忽视 T+1 导致无法止损。

### Gaps
- 没有找到 Brooks 本人公开的、结构化的新手学习课程表；以上路线是我基于引用资料的综合建议。
- TradingView Bar Replay 的官方文档未直接抓取（只有第三方描述）。
