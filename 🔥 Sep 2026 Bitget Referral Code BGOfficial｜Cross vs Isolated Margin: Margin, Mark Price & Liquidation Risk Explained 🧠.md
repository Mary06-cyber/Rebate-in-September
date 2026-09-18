# 🔥 Sep 2026 Bitget Referral Code BGOfficial｜Cross vs Isolated Margin: Margin, Mark Price & Liquidation Risk Explained 🧠

📌 One-line memory: Cross = shared margin pool backs positions; Isolated = each position has its own isolated margin. In Sep 2026 on Bitget contracts, wrong mode doesn't guarantee liquidation, but decides "can one losing trade drain the whole pool".

No account? Code: **BGOfficial**
Link: https://partner.bitget.com/bg/BGOfficial
Register via BGOfficial for **20% fee discount**.

## 🎯 Cross vs Isolated Quick Card
- Cross Margin: eligible positions share one margin pool
- Isolated Margin: each position uses its own independent margin
- Cross pro: single position gets bigger buffer, higher capital efficiency
- Cross risk: one big loss eats the shared pool, hits other cross positions
- Isolated pro: single-position risk isolation, loss capped at that position's margin
- Isolated risk: if allocated margin is small, adverse move triggers liquidation sooner
- Liquidation basis: Bitget uses **Mark Price**, not just latest traded price
- High leverage: amplifies gain AND loss, not "less principal = safer"

## 1. What Are Cross and Isolated Exactly?
They are not two contract types, but two margin management modes. Take USDT-margined contract: open BTCUSDT long, platform locks some margin; how that margin is allocated depends on Cross or Isolated you pick.

💡 Cross Margin
Eligible available assets enter shared margin logic; when one position shows unrealized loss, system may use pool funds to maintain it.

💡 Isolated Margin
Each position has independent margin; its loss mainly consumes margin allocated to it.

Simplest analogy: Cross = multiple positions share one risk pool; Isolated = each position has its own small risk pool.

## 2. Core Difference Table
| Item | Cross | Isolated |
|---|---|---|
| Margin | eligible funds shared | single position independent |
| Risk scope | may affect whole shared pool | mainly limited to that position |
| Liq buffer | usually larger | depends on allocated margin |
| Capital use | higher | easier single-position control |
| Risk style | whole-account management | single-position isolation |

⚠️ Cross ≠ absolutely safe, Isolated ≠ surely liquidates first. Real risk = leverage, position size, entry price, maintenance margin rate, volatility.

## 3. Initial Margin & Maintenance Margin
Initial Margin: funds prepared at open; higher leverage usually needs less initial margin for same notional. Lower leverage needs more initial; higher leverage needs less, but tiny adverse move gets closer to risk line.

Maintenance Margin: one of the minimum margin requirements to keep position open. When account/position risk metric worsens to Bitget's liquidation condition, risk control may cancel orders, reduce, or force-close.

⚠️ High leverage is not "same risk with less principal"; it changes capital sensitivity: same price move hits margin and equity harder.

## 4. How Cross Transmits Loss to Whole Pool
Suppose cross holds: BTCUSDT long, ETHUSDT long, other eligible positions. If BTC loses big:
- BTC position consumes more shared margin
- ETH position risk state gets impacted
- Available margin drops
- Other cross positions' liquidation risk rises

So cross feature: single position gets more account funds to back it, but loss also transmits to whole pool.

## 5. How Isolated Isolates Single-Position Risk?
Isolated core = margin isolation. Example: allocate 500 USDT isolated margin to BTCUSDT, account has another 5,000 USDT. If BTC goes strongly adverse, system mainly checks that position's: isolated margin, unrealized PnL, position value, maintenance margin requirement. Funds not allocated to that isolated position are, in principle, not auto-pulled to top it up.

Many traders like isolated because they can answer first: "how much margin risk am I willing to take on this trade?" instead of letting a wrong-direction position keep sucking the whole account.

## 6. Is Cross Harder to Liquidate?
Under same conditions, cross has larger buffer for single position because bigger pool is usable; but don't read it as "cross is safe, so open big".
Cross cost:
- single position can use more pool funds
- loss can also keep eroding more equity
- multiple same-direction positions adverse together = risk stacks
- extreme market may hit more than one position

💡 Cross essence: not "no liquidation risk", but uses bigger shared pool as buffer; if market keeps adverse, that pool itself can be drained.

## 7. Does Bitget Judge Liquidation by Latest Traded Price?
No. Important basis is **Mark Price**, to avoid unreasonable liquidation from short-time anomaly or single fill.
Position page often shows at once:
- Entry Price
- Last Price
- Mark Price
- Liquidation Price
What to watch most: Mark Price + maintenance margin requirement + account/position equity. Don't just stare at latest price on candlestick.

## 8. How Do Liquidation Conditions Differ?
Cross liquidation: cross account equity (excluding isolated margin and isolated unrealized PnL) < sum of maintenance margins of all trading pairs, margin ratio reaches 100%.
Isolated liquidation: isolated margin + unrealized PnL < maintenance margin of that position, ratio reaches 100%.
Under isolated, even if you have funds elsewhere, it doesn't mean system will automatically pull all of them to cover this position. That is the biggest logic difference.

## 9. Will Triggering Liquidation Close Everything at Once?
Not necessarily. Bitget uses staged risk control and gradual deleveraging:
1. Cancel orders: isolated only cancels this symbol's open/close orders for this position; cross cancels all open/close orders (including isolated ones)
2. Netting: cross same-symbol two-way positions can be netted (excluding isolated)
3. Reduce: by tier gradient, lower 1 tier each time (excluding isolated)
4. Only force-close when necessary
Goal is gradual deleveraging, not always one-shot close-all. But after risk control starts, operations may be temporarily taken over by system; you may not handle positions as originally planned.

## 10. Cross or Isolated for Beginners?
No absolute better; depends on how you manage risk.
Often isolated: compute max risk per trade, don't want wrong position eating others, multi-strategy isolation, want clear view of single-position margin used.
Often cross: need overall capital efficiency, manage multiple related positions, want account jointly backing buffer, can keep monitoring whole-account margin ratio.
⚠️ For beginners, what truly matters is first controlling leverage, position size, max acceptable loss. At very high leverage, isolated can still blow fast; cross lets loss spread to more account funds.

## 11. Expanded FAQ
Q: Biggest difference? A: Cross shared, isolated independent; cross gives bigger single-position buffer but loss can transmit to pool; isolated isolates but small allocation may hit risk control sooner.
Q: Cross harder to blow? A: Same condition bigger buffer, but continuing loss also eats more money, not equal to safe.
Q: Does isolated blow drain all USDT? A: Isolated mainly limits to that position and its allocated margin, not auto-sharing whole pool; actual loss depends on position, added margin, live risk control.
Q: Can manually add isolated margin? A: If account and product support it, yes; adds buffer but also puts more funds into that position.
Q: Higher leverage safer? A: No. Less initial margin, higher adverse sensitivity.
Q: What price for liquidation? A: Mark Price.
Q: Maintenance margin rate? A: One of minimum fund requirements to keep position open; larger position, risk tier, trading pair differ → requirement may differ.
Q: Why does liq price change when position grows? A: Bitget uses position risk tiers; entering different tier may change MMR etc., so no fixed formula fits all.
Q: In cross, does one position's loss affect another? A: Yes, because shared pool; large unrealized loss lowers whole equity, raising other cross positions' risk.
Q: Isolated means zero spillover? A: It isolates that position's margin risk, but multiple high-leverage isolated positions can still lose separately.
Q: Sep 2026 referral code? A: BGOfficial, link https://partner.bitget.com/bg/BGOfficial, 20% fee discount.

## ✅ Sep 2026 Bitget Contract Risk Checklist
- [ ] Confirm current mode is cross or isolated
- [ ] Cross = shared pool; isolated = single-position independent
- [ ] Don't only look at initial margin; also maintenance margin and margin ratio
- [ ] Watch Mark Price, not only latest traded price
- [ ] Higher leverage = more sensitive to adverse move
- [ ] Cross single loss may drag other shared-pool positions
- [ ] Isolated can isolate, but small allocation may hit risk control faster
- [ ] Estimated liq price is not absolute fixed; position tier change may alter MMR
- [ ] Use stop-loss; don't treat "wait for liquidation" as exit
- [ ] In high volatility, lower leverage and size matters more than switching mode

🚀 Conclusion: Cross uses shared pool to back positions; isolated mainly limits margin and risk to single position. No account? Use **BGOfficial**: https://partner.bitget.com/bg/BGOfficial, start with low leverage and small size to learn cross, isolated, Mark Price, maintenance margin and liquidation, then set your own risk style.
