# 🎯 October 2026 Bybit Invite Code (BYOFFICIAL)｜Isolated vs Cross Margin on Bybit: Collateral and Liquidation Risk Comparison

When trading Bybit perpetual or futures contracts in October 2026, besides direction, leverage and position size, the choice between Isolated Margin and Cross Margin directly changes your liquidation risk.

Quick mental model:

- Isolated Margin: each position has its own collateral pool. A problem in one position mainly affects the margin allocated to that position.
- Cross Margin: available collateral inside the Unified Trading Account (UTA) is shared across eligible positions and orders. One losing position can keep consuming overall account equity.

Invite details used in this guide:

- Bybit invite code: **BYOFFICIAL**
- Bybit invite link: [https://partner.bybit.com/b/BYOFFICIAL](https://partner.bybit.com/b/BYOFFICIAL)

Register through the BYOFFICIAL link to receive a built-in 33% trading fee discount. After enabling MNT fee deduction, spot trading can enjoy up to 50% fee discount and derivatives trading up to 40% fee discount.

💡 Extra note: MNT (Mantle) is part of the Bybit ecosystem. Turn on MNT fee payment in your account fee settings and keep enough MNT balance; the system uses MNT to offset part of the trading fee, which unlocks the higher combined discount. Actual eligibility depends on your account status and current campaign rules.

## 📌 Isolated vs Cross quick comparison

| Item | Isolated Margin | Cross Margin |
|:---|:---|:---|
| Collateral source | Allocated per position | Shared UTA available collateral |
| Risk calculation | Single position focused | Whole account focused |
| Liquidation trigger | Mark Price hits position Liquidation Price | Account Maintenance Margin Rate (MMR) reaches 100% |
| Liquidation price | Relatively fixed reference | Dynamic reference |
| Margin sharing between positions | No | Yes |
| One position loss affecting others | Limited | Can affect whole account |
| Capital efficiency | Lower | Higher |
| Risk isolation | Clearer | Weaker |
| UTA default | Not default | Cross Margin is default |

## 1️⃣ What is Bybit Isolated Margin?

Isolated Margin manages each position’s collateral separately.

Example: you hold BTCUSDT long and ETHUSDT long at the same time. Under isolated mode, BTC collateral risk and ETH collateral risk are calculated independently. If BTC moves sharply against you and Mark Price touches the BTC position’s Liquidation Price, Bybit may force-close the BTC position. That BTC liquidation normally does not take ETH isolated collateral to cover the BTC loss.

Main advantage: single-position risk stays inside a relatively independent margin box.

Trade-off: capital efficiency is lower because margin already assigned to one isolated position cannot be freely reused by other positions.

💡 Extra note: in supported isolated setups you can manually add margin to one position to push its liquidation price farther away, but that also means you accept more funds at risk for that specific trade. For small accounts that want a hard cap on every trade, isolated is usually easier to control.

## 2️⃣ What is Bybit Cross Margin?

Cross Margin lets eligible available collateral in the Unified Trading Account support all positions and working orders together.

Example: you hold BTC, ETH and SOL derivatives positions. If BTC has a large unrealized loss, as long as the account still has available collateral, the system may keep using shared collateral to maintain the BTC position.

Cross margin can:

- Improve overall capital utilization
- Let profits and losses from different derivative positions interact under account rules
- Use more account assets to support total risk

Important downside: one continuously losing position may gradually drain the entire UTA available collateral and therefore pressure other positions.

So “cross looks farther from a fixed liquidation price” does not mean “safer”. The risk simply moves from one position to the entire account.

💡 Extra note: under cross, watch Account MMR constantly, not only the liquidation tag on one chart. MMR near 100% means the whole account is close to forced liquidation even if one individual position still looks fine.

## 3️⃣ Core difference between isolated and cross

See the quick table above.

One-line summary: isolated controls how much margin this single position may use; cross manages how much margin the whole account can afford to risk.

## 4️⃣ When does isolated margin get liquidated?

In Bybit isolated mode, every position has its own collateral and Liquidation Price. When Mark Price touches that position’s Liquidation Price, forced liquidation may start.

Key point: Bybit liquidation evaluation primarily uses Mark Price, not simply the Last Traded Price shown on the candlestick chart.

Possible scenario:

- Chart last price has not yet reached the liquidation level
- Mark Price already touched the Liquidation Price
- Position still gets liquidated

If your stop order triggers by Last Traded Price and sits too close to the isolated Liquidation Price, Mark Price may trigger liquidation before the stop fills.

⚠️ Do not judge liquidation only by latest chart price. Understand Last Traded Price, Mark Price and Liquidation Price together. Bybit clearing mainly references Mark Price.

💡 Extra note: Mark Price usually blends multiple reference prices and funding data to reduce manipulation from one exchange spike, but during extreme volatility it can still move fast. Keep stop distance wide enough.

## 5️⃣ When does cross margin get liquidated?

Cross does not rely on one fixed liquidation price per position.

In Bybit UTA cross mode, the system continuously calculates:

- Account equity
- Available collateral
- Initial Margin Rate (IMR)
- Maintenance Margin Rate (MMR)
- Unrealized PnL of all relevant positions

When Account Maintenance Margin Rate reaches 100%, the account enters liquidation conditions.

The cross interface may still show a Liquidation Price, but treat it as reference only. It can change with:

- Account equity changes
- Profit or loss from other positions
- Opening or closing positions
- Available collateral changes
- Maintenance Margin Requirement changes

Therefore, checking only one displayed liquidation price is not enough under cross. Account MMR is the core account risk metric.

## 6️⃣ Why cross can show a farther liquidation price but still be risky?

Assume you open a BTC long.

Under isolated, you allocate only 1,000 USDT to that position. Risk is mostly calculated inside that 1,000 USDT box.

Under cross, if the UTA still has another 5,000 USDT available, the BTC position may be supported by more shared funds. The displayed Liquidation Price can look farther.

But if BTC keeps moving against you, that position may also consume account collateral you never intended for BTC.

So the real difference is not “isolated is dangerous, cross is safe”. Isolated concentrates risk in one position; cross allows risk to spread into the whole shared collateral pool.

## 7️⃣ Initial Margin vs Maintenance Margin

Before comparing margin modes, separate two concepts.

Initial Margin (IM): collateral required to open a position. Larger notional size and lower leverage usually require higher initial margin.

Maintenance Margin (MM): minimum collateral required to keep the position open. As the market moves against you, unrealized loss reduces the available buffer.

If risk keeps rising:

- Isolated may liquidate when Mark Price hits the position Liquidation Price
- Cross mainly judges whether Account MMR reaches 100%

In current Bybit contract margin calculations, some IM and MM components already use Mark Price, so risk should not be understood only from entry price.

💡 Extra note: IMR and MMR often rise in tiers as notional size grows. Higher VIP levels usually lower these rates. Check Bybit’s official fee and margin schedule for your account tier.

## 8️⃣ Does higher leverage always mean higher liquidation risk?

Leverage directly affects initial margin and risk buffer.

With other conditions equal, higher leverage usually means:

- Less initial margin for the same notional position
- Smaller adverse price room before problems
- Liquidation condition potentially closer

But remember: actual PnL is driven by notional value and price change, not by the leverage number itself.

Example: two traders both hold 10,000 USDT notional BTC long. If BTC falls 5%, ignoring fees, both have similar price-loss exposure on that notional. The difference is how much collateral each committed and what percentage of that collateral is lost.

⚠️ High leverage does not make the market more volatile. The market volatility is unchanged, but high leverage leaves a smaller margin buffer, so small price moves can approach liquidation faster.

💡 Extra note: new derivatives traders can start with isolated mode and modest leverage such as 3x–5x, then adjust after learning margin behavior.

## 9️⃣ Which mode fits which risk situation?

Isolated emphasizes single-position isolation. Use it when you want a fixed collateral cap per strategy, for example:

- Different coins with completely different strategies
- No desire for one wrong position to drain other funds
- Clear maximum collateral per position

Cross emphasizes shared collateral and capital efficiency. If one account manages many positions, cross lets account assets and unrealized PnL share risk calculation under eligibility rules.

It improves capital use, but one position’s risk may spread to the entire UTA. Never assume cross is safer just because the reference liquidation price looks farther.

💡 Extra note: UTA margin mode is account-level. You cannot set BTC isolated, ETH cross and SOL another mode at the same time under the same UTA product scope.

## 🔟 Can Bybit spot leverage use isolated margin?

Currently no. This is a common confusion.

Bybit UTA Spot Margin Trading supports:

- Cross Margin
- Portfolio Margin

Isolated Margin is not supported for Spot Margin Trading.

So the isolated vs cross discussion above mainly applies to perpetual, futures and other derivative positions. For spot margin borrowing, confirm the account uses cross or eligible portfolio margin, and understand:

- Collateral assets
- Borrowing
- Interest
- Repayment
- Account MMR
- Liquidation risk

💡 Extra note: spot cross margin also has liquidation risk. If collateral value drops fast, the account may face margin calls or forced repayment.

## 1️⃣1️⃣ How to switch isolated and cross on Bybit?

Bybit UTA supports:

- Isolated Margin
- Cross Margin
- Portfolio Margin

UTA defaults to Cross Margin.

Common App switching path:

1. Open Bybit App
2. Enter Futures or derivatives trading page
3. Tap the top-right three-dot menu
4. Check current Margin Mode
5. Select the margin mode you want
6. Tap Switch Margin Mode
7. Confirm

Important notes:

- UTA Margin Mode is account-level, not per trading pair
- You cannot simply run BTC cross, ETH isolated and SOL another mode under the same UTA scope
- Current mode applies to relevant account products

Switching may be blocked when:

- Collateral would be insufficient after switch
- Positions or orders do not meet switching conditions
- Spot margin borrowing or orders exist
- Switch could immediately cause liquidation
- Account does not meet target margin mode requirements

💡 Extra note: close or flat relevant derivative positions and remove spot borrowings before switching if you want a smoother change. Portfolio Margin has extra eligibility rules.

## 1️⃣2️⃣ Bybit isolated and cross FAQ

**What is the October 2026 Bybit invite code?**
This guide uses **BYOFFICIAL**.
Bybit invite link: [https://partner.bybit.com/b/BYOFFICIAL](https://partner.bybit.com/b/BYOFFICIAL)

**What fee discount does BYOFFICIAL give?**
Register through the BYOFFICIAL link for a built-in 33% fee discount. After enabling MNT fee deduction, spot can enjoy up to 50% fee discount and contracts up to 40% fee discount.

**Which is harder to liquidate, isolated or cross?**
No universal answer. Isolated calculates risk per position; cross shares available account collateral. Cross may show a farther reference liquidation price for one position but can consume more total account funds.

**Does isolated liquidation affect other positions?**
Each isolated position manages its own collateral, so a single position liquidation usually does not directly use other independent positions’ isolated collateral to cover the loss.

**Will cross liquidation drain all account money?**
Cross uses eligible shared UTA collateral to support account risk, so continued loss can affect a wider fund range than one isolated position. Actual liquidation depends on assets, collateral settings, positions and Bybit risk controls.

**Why does cross Liquidation Price keep changing?**
Because cross risk is calculated at account level. Changes in equity, other positions’ PnL, available collateral and Maintenance Margin Requirement can move the reference Liquidation Price.

**What metric matters most under cross?**
Besides the reference Liquidation Price, check Account Maintenance Margin Rate. At 100% MMR the account may enter liquidation.

**Does Bybit liquidation use latest traded price?**
Not mainly. Bybit uses Mark Price as the important liquidation trigger reference.

**Can isolated margin be increased manually?**
Isolated centers on independent per-position collateral. If the account and product allow it, you can adjust collateral for that position, but adding margin means accepting more funds at risk for that position.

**Is Bybit default isolated or cross?**
UTA currently defaults to Cross Margin.

**Can spot leverage use isolated?**
Bybit UTA Spot Margin Trading does not support Isolated Margin, only Cross Margin and Portfolio Margin.

**Forgot BYOFFICIAL at registration, can I add it later?**
Most reliable is registering through the BYOFFICIAL link before account creation. If the account already exists, do not assume the referral can be changed arbitrarily; check current referral status and Bybit account rules.

**Can I delete the account and re-register if I forgot the code?**
Do not treat re-registration as the first solution. KYC, campaigns and referral rules may restrict changes. Check the existing account status first.

💡 Extra FAQ:

**Does the BYOFFICIAL fee discount apply immediately?**
After qualifying registration through the link, the base 33% referral discount is typically applied per Bybit fee rules. MNT additional discount requires enabling MNT payment and having sufficient MNT.

**Where to enable MNT deduction?**
Use account fee settings or the relevant trading-fee page, turn on MNT fee payment, and keep MNT balance for deduction.

## ✅ October 2026 Bybit isolated/cross checklist

- [ ] Invite code: **BYOFFICIAL**
- [ ] Invite link: [https://partner.bybit.com/b/BYOFFICIAL](https://partner.bybit.com/b/BYOFFICIAL)
- [ ] Isolated: margin managed per position
- [ ] Cross: UTA available margin shared across positions
- [ ] Isolated liquidation mainly checks Mark Price vs position Liquidation Price
- [ ] Cross liquidation mainly checks Account MMR reaching 100%
- [ ] Cross Liquidation Price is a dynamic reference
- [ ] Do not judge liquidation only by Last Traded Price
- [ ] High leverage usually means smaller margin buffer
- [ ] Isolated emphasizes single-position isolation
- [ ] Cross emphasizes shared collateral and capital efficiency
- [ ] Cross single loss may affect other account assets
- [ ] Spot Margin Trading does not support Isolated Margin
- [ ] UTA currently defaults to Cross Margin
- [ ] Margin Mode is account-level
- [ ] Confirm collateral and open positions before switching mode
- [ ] Set stop-loss before derivatives trading and confirm trigger price type

One-sentence memory: isolated means each position carries its own margin risk; cross means the whole account jointly carries margin risk.

Use BYBIT official link for new account:

- Bybit invite code: **BYOFFICIAL**
- Bybit invite link: [https://partner.bybit.com/b/BYOFFICIAL](https://partner.bybit.com/b/BYOFFICIAL)

Built-in 33% fee discount via link; with MNT deduction up to 50% spot discount and up to 40% derivatives discount.

October 2026 actual trading should follow your Bybit account’s displayed Margin Mode, Account MMR, Liquidation Price, fee rate and risk limits.
