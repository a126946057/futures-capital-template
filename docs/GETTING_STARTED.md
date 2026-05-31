# Getting Started

## 1. 設定商品條件

到 `Settings` 工作表設定：

- `Point Value`：每點價值。
- `Margin Per Lot`：單口保證金。
- `Drawdown Water Points`：每口預留的回撤點數。
- `Starting Equity`：策略起始資金。

模板會用：

```text
Water Per Lot = Margin Per Lot + Drawdown Water Points * Point Value
```

來估算目前資金可承受的口數。

## 2. 匯入交易紀錄

到 `Trades` 工作表填入：

- Entry Date
- Exit Date
- Direction
- Lots
- Entry Price
- Exit Price
- Costs

`Points`、`Gross PnL`、`Net PnL`、`Equity After` 會自動計算。

## 3. 紀錄提領

到 `Withdrawals` 工作表填入提領紀錄。

`Actual` 代表錢已經離開帳戶，會計入總財富。

`Locked` 代表帳內鎖定或心理上預留，但錢仍在帳戶裡，不應重複計入總財富。

## 4. 查看結果

到 `Dashboard` 看：

- Current Account Equity
- Total Wealth
- Win Rate
- Profit Factor
- Max Drawdown
- Estimated Lots

到 `Monthly` 看月損益與交易數。

## 5. 替換範例資料

公開版本內的資料是人工範例，不代表任何真實策略。

正式使用時，請刪除範例交易，再貼上自己的回測或實戰交易。
