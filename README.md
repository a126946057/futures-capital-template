# Futures Capital Template

A futures capital management template for individual traders who want to track backtests, live trades, drawdowns, withdrawals, and equity curves in one place.

This project does **not** provide trading signals. It does not tell users where to buy or sell. Its goal is to help traders measure whether a strategy can survive real-world costs, margin requirements, execution gaps, withdrawals, and drawdowns.

## Why This Exists

Many strategies look profitable in a simple backtest, but break when real trading conditions are included:

- Fees, taxes, and slippage are ignored.
- Margin requirements change over time.
- Position sizing expands too aggressively after gains.
- Withdrawals are double-counted as wealth.
- Backtest trades and live trades are not compared.
- Win rate is overemphasized while profit factor, drawdown, and right-tail capture are ignored.

This template is built to put those hidden risks into one workbook.

## Features

- Trade log for backtest or live trades
- Dashboard for equity, win rate, profit factor, withdrawals, and estimated lots
- Capital water calculation using margin plus drawdown buffer
- Actual withdrawal vs internal locked amount
- Monthly PnL summary
- Equity curve and drawdown charts
- Example data for quick testing
- Disclaimer and publishing checklist for open-source or paid template use

## Files

- `examples/futures_capital_template_v0.1.xlsx` - Excel template
- `examples/sample_trades.csv` - sample trade log
- `docs/GETTING_STARTED.md` - quick start guide
- `docs/DISCLAIMER.md` - disclaimer template
- `docs/PRIVACY_BOUNDARY.md` - what should not be published
- `docs/PRODUCT_IDEA.md` - possible free/paid product roadmap
- `docs/PUBLISH_CHECKLIST.md` - GitHub release checklist
- `tools/build_template.py` - rebuild the Excel template

## Quick Start

1. Open `examples/futures_capital_template_v0.1.xlsx`.
2. Set point value, margin, drawdown water points, and starting equity in `Settings`.
3. Replace sample rows in `Trades` with your own backtest or live trades.
4. Record withdrawals in `Withdrawals`.
5. Review `Dashboard` and `Monthly`.

## Important

This is a capital management and research template. It is not investment advice, a trading signal, copy trading, or a promise of returns.

Futures and options are high-risk products. Historical backtests do not guarantee future results.

## 中文說明

這是一個給個人交易者使用的期貨策略資金管理模板。

它不提供交易訊號，不教你買哪裡、賣哪裡，而是幫你把策略真正重要的事情算清楚：資金水位、口數、成本、回撤、提領、實戰偏差與資金曲線。

## 為什麼做這個

很多策略看起來會賺錢，但真正上場後會死在其他地方：

- 手續費、交易稅、滑價沒有算進去。
- 保證金提高後，原本的口數規則失真。
- 獲利後提領，卻重複計入總財富。
- 回測和實戰紀錄沒有對照。
- 只看勝率，不看右尾、賺賠比與最大回撤。

這個模板的目標是把這些問題放到同一張表裡。

## 功能

- 回測或實戰交易紀錄
- 資金、勝率、PF、提領與估算口數儀表板
- 用保證金加回撤緩衝計算單口資金水位
- 區分實際提領與帳內鎖定金額
- 月損益統計
- 資金曲線與回撤圖
- 可快速測試的人工範例資料

## 使用方式

1. 打開 `examples/futures_capital_template_v0.1.xlsx`。
2. 在 `Settings` 設定每點價值、保證金、回撤水位與起始資金。
3. 用自己的回測或實戰交易取代 `Trades` 裡的範例資料。
4. 在 `Withdrawals` 紀錄提領或帳內鎖定金額。
5. 到 `Dashboard` 和 `Monthly` 查看結果。

## 重要提醒

這是資金管理與研究模板，不是投資建議、交易訊號、跟單服務或獲利承諾。

期貨與選擇權屬於高風險商品。歷史回測不代表未來結果。

## License

MIT License.
