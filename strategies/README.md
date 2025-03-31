# Strategies
You can add your own strategy to this folder. The filename must end with `_strategy.py`,
and contain the following:

```python
from binance_trade_bot.auto_trader import AutoTrader

class Strategy(AutoTrader):

    def scout(self):
        # Your custom scout method

```

Then, set your `strategy` configuration to your strategy name. If you named your file
`custom_strategy.py`, you'd need to put `strategy=custom` in your config file.

You can put your strategy in a subfolder, and the bot will still find it. If you'd like to
share your strategy with others, try using git submodules.

Some premade strategies are listed below:
## `default`

## `multiple_coins`
The bot is less likely to get stuck

kbudmcd