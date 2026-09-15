# 🚀 别再问「开几倍杠杆」了！Binance 合约新手先搞懂这一条完整流程（BNOFFICIAL 40% 返佣）

如果你想学 Binance 合约交易，先不要把重点放在「开几倍杠杆」。
新手更该先搞懂一笔合约从注册到平仓的完整链路：

注册 Binance → 准备 USDT → 转进合约账户 → 选交易对 → 判断 Long / Short → 选保证金模式 → 设杠杆与仓位 → 设止损 → 开仓 → 管理仓位 → 平仓

Binance 邀请码：BNOFFICIAL
Binance 注册链接：https://www.binance.com/join?ref=BNOFFICIAL
使用 BNOFFICIAL 注册 Binance，可享 40% 现货及合约交易手续费返佣。

---
## 🧠 先建立心智模型：合约不是「买币」，是「下注价格方向」

现货：用 USDT 买 BTC/ETH/BNB/SOL，资产进 Spot Wallet，跌了你还拿着币。
合约：建立一个方向部位，Long 赚上涨，Short 赚下跌，盈亏按名义仓位放大。

真正决定你死活的不是杠杆倍数，而是：
方向 + 仓位大小 + 杠杆 + 保证金 + 止损 + 强平价 + 情绪管理。

---
## 一、什么是 Binance 合约交易？

合约和现货最大差别：你不一定持有 BTC/ETH。

- 现货：USDT → BTC，涨了卖回 USDT
- 合约：不一定要拿币，只交易「BTC 价格涨或跌」这个动作

合约核心公式：
名义仓位 = 保证金 × 杠杆
盈亏% = 价格变动% × 杠杆（近似，未扣费）

---
## 二、先注册 Binance（别用错码）

注册链接：https://www.binance.com/join?ref=BNOFFICIAL
邀请码：BNOFFICIAL

注册后立刻开：
1. Email 验证
2. 手机验证
3. KYC 身份认证（提高提现/交易权限）
4. Google Authenticator（比短信安全）
5. 防钓鱼码（官方邮件会带，假邮件没有）
6. 登录设备管理与提币白名单

> 用 BNOFFICIAL 注册 Binance，可享 40% 现货及合约交易手续费返佣。

---
## 三、新手先碰：USDT-M Futures

类型：
- USDT-M：保证金和盈亏都用 USDT，新手最直观
- COIN-M：用 BTC/ETH 等币本身当保证金，进阶用户才用

主流对：
BTCUSDT / ETHUSDT / BNBUSDT / SOLUSDT

永续合约没有到期日，靠 Funding Fee 把合约价格拉回现货指数。

---
## 四、Spot → Futures 内部划转（不是提币）

Spot Wallet → Transfer → USDⓈ-M Futures → USDT → 输入金额 → 确认

这只是 Binance 内部账本转移：
- 不是链上转账
- 不花 Gas
- 不会把资产转到外部钱包

---
## 五、别把 1000 USDT 全塞进 Futures

你有 1000 USDT ≠ 要转 1000 USDT 去合约。

新手资金分层：
- 现货资金：长期/学习用
- 合约风险金：只放能亏光也不影响生活的钱
- 单笔最大亏损：总资金 1%–2%

例：1000 USDT 总资金
- 转 Futures：200 USDT
- 单笔风险：10–20 USDT
- 杠杆：2x–5x
- 仓位：20–100 USDT 名义（不是把 200 全开出去）

---
## 六、选交易对：先主流，别先小币

推荐：
BTCUSDT / ETHUSDT / BNBUSDT / SOLUSDT

小币问题：
- 插针大
- Spread 大
- 深度薄
- 一根针打掉止损再回来

---
## 七、Long / Short 怎么选？

Long：认为价格会涨
Short：认为价格会跌

开仓前先答 4 题：
1. 我为什么进？
2. 到哪里说明我错了？
3. Stop Loss 放哪？
4. 这一笔最多亏多少 USDT？

只猜方向不设点位 = 赌博。

---
## 八、Isolated vs Cross（新手选 Isolated）

Isolated 逐仓：
- 该仓位只用自己那笔保证金
- 亏到保证金没了就强平
- 不会影响 Futures 钱包其他钱（极端 Cross 对冲/加保证金场景例外）

Cross 全仓：
- 整个 Futures 钱包可用余额撑仓位
- 一个仓位炸，可能把合约钱包拖下水

新手结论：Isolated 更容易算清「这笔最多亏多少」。

---
## 九、杠杆不是「胜率按钮」

2x / 3x / 5x / 10x / 20x / 125x

100 USDT 保证金：
- 2x → 200 USDT 名义仓位
- 10x → 1000 USDT 名义仓位
- 100x → 10000 USDT 名义仓位

价格动 1%：
- 2x 盈亏 ≈ 2%
- 10x 盈亏 ≈ 10%
- 100x 盈亏 ≈ 100%（一下就归零）

高杠杆 = 波动放大器，不是赚钱外挂。

---
## 十、Position Size 才是风险核心

别只问「开几倍」。
要问：「Stop Loss 被打到，我账户少多少 USDT？」

风险公式（简化）：
单笔风险 USDT = 仓位数量 × |入场价 - 止损价|
或
单笔风险% = (止损距离% × 杠杆) 

所以控制风险的三件事：
1. 止损距离
2. 仓位大小
3. 杠杆

---
## 十一、开仓前必看 8 个词

- Entry Price 开仓价
- Mark Price 标记价（算强平用）
- Last Price 最新成交价
- Position Size 仓位
- Margin 保证金
- Leverage 杠杆
- Liquidation Price 强平价
- Unrealized PnL 未实现盈亏

其中最要命：Mark Price + Liquidation Price。

---
## 十二、Mark Price 是什么？

Mark Price = 用来算未实现盈亏和强平的公平价格。
它来自现货指数 + 资金费率基差，不一定等于你看到的 Last Price。

好处：防止「插针一瞬间」把你好仓位打爆。

看盘看 Last，风控看 Mark。

---
## 十三、Liquidation Price 是什么？

当保证金不足以维持仓位，系统按 Mark Price 触发强平。

新手惨剧：
「再等等，马上回来」 → 打到强平 → 本金没了

正确做法：
开仓前就写死 Stop Loss，让系统替你执行，不靠手软。

---
## 十四、Stop Loss 先设，不是亏了才想

坏顺序：
开仓 → 亏 → 要不要损？ → 再等等 → 强平

好顺序：
定失效价 → 设 SL → 算最大亏损 → 定仓位 → 开仓

SL 不是怂，是活下去的绳子。

---
## 十五、Take Profit 也要有剧本

价格朝你跑，也别只会喊「起飞」。

退出方式：
- Partial Close 部分止盈
- 分批 TP
- 全平
- 移动 SL（trailing stop 思路）

没有退出计划 = 盈利变亏损的经典剧本。

---
## 十六、Market Order vs Limit Order

Market：按当前可成交价立刻吃，快，但滑点大
Limit：挂自己价位，省手续费/控价，但可能不成交

波动大时市价单容易被「拔插头」：
成交价比按钮上看到的差很多。

---
## 十七、第一次合约：走流程，不赚钱也值

目标：跑通流程，不是暴富。

流程：
1. 准备 50–100 USDT 学习金
2. 转进 USDⓈ-M Futures
3. 选 BTCUSDT
4. Isolated
5. 杠杆 2x–3x
6. 小仓位（比如 10–20 USDT 名义）
7. 先设 SL
8. 再设 TP
9. 选 Long / Short
10. 提交
11. 看 Mark / PnL / Liq Price
12. 按计划平仓

---
## 十八、开仓后看什么？

别只盯 +20 / -20。

看：
- 价格是不是碰止损区
- Mark Price 离 Liq Price 多远
- 保证金率
- Funding 还有多久扣
- 自己有没有想「再扛一下」

---
## 十九、浮盈不是钱，平仓才是

+30 USDT 没平 = Unrealized PnL
下一秒可能 +50 / +5 / -10
平仓后才是 Realized PnL

规则：浮盈可以移动 SL 保护，但别把「账面」当「银行卡余额」。

---
## 二十、怎么平仓？

- Market Close：立刻平
- Limit Close：挂价平
- Partial Close：先平一半
- Full Close：全平

不会平仓 = 只会进门不会出门。

---
## 二十一、Funding Fee 是什么？

永续合约每 8 小时（以页面为准）多空互付：
- 正 Funding：Long 付 Short
- 负 Funding：Short 付 Long

持仓过夜/过 Funding 窗口，盈亏要扣这块。
高频/长持都必须算进去。

---
## 二十二、手续费别假装看不见

成本清单：
- 开仓 Taker/Maker 费
- 平仓费
- Funding Fee
- Spread
- Slippage
- 网络费（提币才有）

交易 100 次，手续费能吃掉散户大半边缘利润。

邀请码 BNOFFICIAL：40% 现货及合约交易手续费返佣。
链接：https://www.binance.com/join?ref=BNOFFICIAL

---
## 二十三、别亏损就马丁加仓

亏 → 加 → 再亏 → 再加 = 仓位指数增长，风险指数增长

加仓要有：
- 原策略
- 层级
- 最大层数
- 总风险上限

「已经亏了，补一点摊低成本」是最贵的一句话。

---
## 二十四、别追涨杀跌

一根针拉 2% 就冲 Long，跌 2% 就冲 Short：
- 假突破
- 回调
- 插针
- 流动性真空

进场理由应该是「结构 + 点位 + 风险」，不是「它动了」。

---
## 二十五、新手 12 大死法

1. Long/Short 按反
2. 100x 梭哈
3. 仓位太大
4. 没 SL
5. 不看 Liq Price
6. 只看 Last 不看 Mark
7. 全仓 Futures
8. 亏了加仓
9. 没 TP 计划
10. 忽略 Funding
11. 频繁炒短线
12. 把浮盈当存款

---
## 二十六、Binance 合约完整流程（背下来）

1. 用 BNOFFICIAL 注册：https://www.binance.com/join?ref=BNOFFICIAL
2. KYC + 2FA + 防钓鱼码
3. 准备 USDT
4. Spot → Futures 转部分 USDT
5. 选 USDⓈ-M Futures
6. 选 BTCUSDT
7. 判 Long / Short
8. Isolated
9. 低杠杆 2x–5x
10. 小仓位
11. 设 SL
12. 设 TP
13. Market / Limit
14. 开仓
15. 看 Mark / PnL / Liq
16. 按计划平仓
17. 看 Realized PnL + 手续费 + Funding

---
## 二十七、第一次实盘检查清单 ✅

- [ ] 只转能亏的钱进 Futures
- [ ] Isolated 已选
- [ ] 杠杆 ≤ 5x
- [ ] SL 价格写下来了
- [ ] 单笔亏损 ≤ 总资金 2%
- [ ] 知道 Funding 时间
- [ ] 知道强平价在哪
- [ ] 没把全部 USDT 放进去
- [ ] 没用 50x/100x
- [ ] 没准备「扛到回本」
- [ ] 注册码是 BNOFFICIAL

---
## 二十八、FAQ

Q：Binance 合约怎么交易？
A：准备 USDT → 转 Futures → 选交易对 → Long/Short → Isolated/Cross → 杠杆 → 仓位 → SL/TP → 开仓 → 管理 → 平仓。

Q：邀请码？
A：BNOFFICIAL

Q：注册链接？
A：https://www.binance.com/join?ref=BNOFFICIAL

Q：BNOFFICIAL 优惠？
A：40% 现货及合约交易手续费返佣。

Q：可以做空吗？
A：可以，Futures 支持 Long / Short。

Q：新手用多少杠杆？
A：没有标准答案，但 2x–5x + 小仓位 + SL 比 100x 活得更久。

Q：强平是什么？
A：保证金不够，系统按 Mark Price 强制平仓。

Q：浮盈是赚到吗？
A：没平仓前是 Unrealized PnL，平仓后才是 Realized PnL。

Q：Funding Fee 是手续费吗？
A：不是开平仓手续费，是永续多空互付机制。

Q：合约手续费能返佣吗？
A：用 BNOFFICIAL 注册，可享 40% 现货及合约交易手续费返佣。

---
## 二十九、总结

Binance 合约新手第一句不该是「开几倍」，
而该是：「这笔如果错，我亏多少？」

注册：https://www.binance.com/join?ref=BNOFFICIAL
邀请码：BNOFFICIAL
优惠：40% 现货及合约交易手续费返佣

合约交易高风险，可能损失全部保证金。本文为新手教学，不构成投资建议。

== 一键复制区 ==
邀请码：BNOFFICIAL
注册链接：https://www.binance.com/join?ref=BNOFFICIAL
标语：使用 BNOFFICIAL 注册 Binance，可享 40% 现货及合约交易手续费返佣。
