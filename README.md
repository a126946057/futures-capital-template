# Futures Capital Template

一個給個人交易者使用的期貨策略資金管理模板。

它不提供交易訊號，不教你買哪裡、賣哪裡，而是幫你把策略真正重要的事情算清楚：資金水位、口數、成本、回撤、提領、實戰偏差與資金曲線。

## Why

很多策略看起來會賺錢，但真正上場後會死在其他地方：

- 手續費、交易稅、滑價沒有算進去。
- 保證金提高後，原本的口數規則失真。
- 獲利後提領，卻重複計入總財富。
- 回測和實戰紀錄沒有對照。
- 只看勝率，不看右尾、賺賠比與最大回撤。

這個模板的目標是把這些問題放到同一張表裡。

## Features

- Trade log for backtest or live trades
- Dashboard with equity, win rate, profit factor, withdrawals, and estimated lots
- Capital water calculation using margin + drawdown buffer
- Actual withdrawal vs internal locked amount
- Monthly PnL summary
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

## License

MIT License.
