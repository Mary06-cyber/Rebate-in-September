# 🚀 2026 Binance 合约交易新手全攻略｜从注册到平仓一次学会（BNOFFICIAL）

> 风险提示：合约属于高杠杆衍生品，可能出现超过本金的亏损。本文仅作操作流程与教育概念整理，不构成投资建议。请只用官方 App／网站，完成 KYC 后再小额练习。

## 🎯 邀请与注册（先绑定再操作）
- 邀请码：BNOFFICIAL
- 注册入口：https://www.binance.com/join?ref=BNOFFICIAL
- 费率说明：Binance 推荐计划按绩效评估；现货邀请人佣金常见基准 20%，可随评估升至 30%／41%／50%，合约邀请人佣金基准 10%，可随评估升至 30%／40%／50%。被邀请人实际返现比例由邀请人设置，并非注册即自动固定 40%。以注册页、Referral 仪表板及当期活动条款为准。[2](@ref)
- 注册检查：邮箱/手机→密码→如出现邀请码栏确认显示 BNOFFICIAL→完成邮箱/短信验证。

## 🧭 完整流程总览
注册 Binance → 完成 KYC → 邮箱/手机/Google Authenticator/防钓鱼码 → 准备 USDT → Spot 转 Futures Wallet → 选 USDT-M 交易对 → 判断 Long/Short → 选 Isolated/Cross → 设 Leverage → 设 Position Size → 设 Stop Loss/Take Profit → 选 Market/Limit → 开仓 → 盯 Mark Price/Unrealized PnL/Liquidation Price → 平仓 → 复盘 Realized PnL/手续费/Funding Fee。

## 💰 现货与合约区别
- Spot：用 USDT 买 BTC/ETH/BNB/SOL，成交后持有资产，无杠杆强平问题。
- Futures：建立价格方向仓位，支持 Long/Short，涉及 Margin、Leverage、Liquidation、Funding Fee；盈亏受杠杆与保证金影响更敏感。

## 📘 账户准备与安全
KYC 实名→邮箱→手机→Google Authenticator→防钓鱼代码→设备管理→提币白名单（后期再开）。不要与他人共用验证码，Authenticator 备份离线保存。

## 📗 新手先选 USDT-M Futures
原因：以 USDT 作保证金，盈亏用 USDT 显示，理解成本较低。常见对：BTCUSDT、ETHUSDT、BNBUSDT、SOLUSDT。相比 Coin-M，USDT-M 更适合第一次做合约的人。

## 🔄 资金划转（内部，非链上）
Spot Wallet → Transfer → USDⓈ-M Futures → USDT → 金额 → 确认。属于账户内划转，不产生链上提币费；但转进合约账户代表该部分资金将承担合约风险。

## 🧮 资金分配原则
例如总可投资 1000 USDT：Spot 留流动/学习资金，Futures 只转“能接受全损”的部分。新手可先转 50～200 USDT 练流程，不把全部资金进合约。

## 🎯 选交易对
优先高流动性：BTCUSDT、ETHUSDT。低流动性小币可能 Spread 大、Slippage 高、Order Book 薄、插针更剧烈。

## 📈 Long / Short
- Long：看涨价开多；价格涨利于仓位。
- Short：看跌价开空；价格跌利于仓位。
开仓前写三件事：进场理由、失效价、最大亏损额。

## 🔐 Isolated 逐仓
单仓独立保证金，亏损原则上限于该仓分配保证金，不影响 Futures 其他空闲资金。新手更易控制单笔风险。

## 🔁 Cross 全仓
Futures Wallet 可用余额共同支撑仓位；不利行情下可能动用到更大范围合约资金，强平影响更广。有经验后再评估。

## 🎚 Leverage 杠杆
常见 2x/3x/5x/10x/20x，部分对更高。杠杆放大盈利也放大亏损：低杠杆≠稳赚，高杠杆≠高胜率。新手建议先 1x～5x，熟练后再按止损距离反推。

## 📐 Position Size 仓位
先定“止损触发愿亏多少 USDT”，再反推仓位：
名义仓位≈可亏金额÷（入场价-止损价）×方向系数；再结合杠杆看所需初始保证金。比盲目选倍数更重要。

## 💲 Entry Price 开仓价
市价单以成交均价作 Entry；限价单以撮合价作 Entry。后续浮盈浮亏均相对 Entry 与市场价格计算。

## 📊 Mark Price 标记价
系统用于强平/部分风险计算的参考价，可能与 Last Price 不同，避免只盯最新成交价误判强平风险。[8](@ref)

## ⚠️ Liquidation Price 强平价
当保证金（含浮亏）不足以满足维持保证金要求，系统可强平。强平价不是止损价；高杠杆会让强平价更靠近 Entry。

## 🛑 Stop Loss 止损
流程：定失效位→设 SL→算最大亏损→定仓位→开仓。可配合 Reduce-Only，避免极端波动下止损单反手开仓。[5](@ref)

## 🏁 Take Profit 止盈
可设一目标/二目标/分批平：Partial Close 先锁部分，剩余按趋势跟踪。开仓前先写退出计划。

## ⚡ Market Order 市价
按盘口可成交价快速吃单，优点快，缺点在剧烈行情有 Slippage。

## 📝 Limit Order 限价
自设价格挂单，控制入场；若价格不到可能不成交。可配合 GTC/IOC/FOK/Post-Only 等时间属性。[5](@ref)

## 🧪 新手第一单示范
少量 USDT→Futures→BTCUSDT→Isolated→2x～5x→小仓位→先挂 SL→再挂 TP→Market 或 Limit 开 Long/Short→成交后看 Entry/Mark/Liq/PnL。目标不是赚钱，是跑通流程。

## 📋 开仓后监控
Entry、Mark、Position Size、Margin、Leverage、Unrealized PnL、Liquidation Price、SL、TP；同时看 Funding Rate 与下次 Funding 时间。

## 💹 Unrealized / Realized PnL
未平仓为 Unrealized PnL，会随价变动；平仓后为 Realized PnL。浮盈不等于已落袋。

## 🔚 平仓方式
Close Position：Market Close（快）、Limit Close（控价）、Partial Close（减仓）、Full Close（全平）。先熟悉按钮再上实盘。

## 💸 Funding Fee 资金费
永续合约按周期在多空间结算，常见约每 8 小时一次；正费率通常 Long 付 Short，负费率相反。持仓久要算 Funding Cost，它不等同开/平仓手续费。[11](@ref)

## 🧾 合约成本清单
开仓手续费、平仓手续费、Funding Fee、Spread、Slippage、部分策略的保证金机会成本。高频会放大费用影响。

## 🚫 亏损不加仓滥用
反向就补、再反向再补，会快速扩大总风险。若加仓须有总预算、最大仓位、明确信号与回撤上限。

## 🎢 不追涨杀跌
急涨追 Long、急跌追 Short 易受 Pullback、Rebound、False Breakout、Stop Hunt 影响。先有逻辑与触发条件再下单。

## ❌ 新手常见错误
多空按反、杠杆过高、仓位过大、无 SL、忽略 Mark/Liq、全资金进合约、亏损摊平、无 TP、忽略 Funding、过度交易。

## ✅ 18 步标准流程
1 用 BNOFFICIAL 注册；2 KYC+安全；3 备 USDT；4 小额定转 Futures；5 进 USDT-M；6 选对；7 Long/Short；8 Isolated/Cross；9 杠杆；10 仓位；11 SL；12 TP；13 Market/Limit；14 核对；15 开仓；16 监控 Mark/PnL/Liq；17 按计划平；18 复盘费用与执行偏差。

## ❓FAQ
Q 合约怎么做？A 转 USDT 到 Futures，选对，设方向/保证金模式/杠杆/仓位/SL/TP，再开仓。
Q 邀请码？A BNOFFICIAL，链接 https://www.binance.com/join?ref=BNOFFICIAL 。
Q 一定返 40% 吗？A 不一定。邀请人合约佣金可达 40%档，但新户实际返现由邀请人设置并以注册页/条款为准；BNB 付手续费另有折扣，不与“邀请返现40%”混算。[10,2](@ref)
Q 做空？A USDT-M 支持 Long/Short。
Q 新手几倍？A 先看止损距离与可亏金额，再定杠杆；很多新手从 1x～5x 起步。
Q 强平？A 保证金不满足维持要求时系统可强平。
Q 资金费是手续费吗？A 不是，属多空定期结算。

## 📌 总结
先学仓位与止损，再学指标；先小额跑通，再谈放大。BNOFFICIAL 仅用于注册绑定，费率以账户与当期推荐规则为准。
