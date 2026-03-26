[[Processamento de Sinais Financeiros]]

Algorithmic trading (algo trade) is using computer programs to execute trades automatically based on predefined rules, mathematical models, or machine learning signals.

The idea: instead of a human watching charts and clicking buy/sell, an algorithm monitors market data in real time and executes trades in milliseconds — faster and more consistently than any human could.

Types of algo trading strategies:
- **Trend following** — identify and ride market trends. Buy when the price is going up, sell when it's going down. Simple in concept, hard in execution (when is a trend a trend vs. noise?).
- **Mean reversion** — prices tend to return to their average over time. If a stock drops unusually far, buy it expecting a bounce back.
- **Arbitrage** — exploit price differences between markets. If the same asset is priced differently on two exchanges, buy low and sell high simultaneously. Requires extreme speed.
- **Market making** — provide liquidity by continuously offering to buy and sell, profiting from the bid-ask spread. High frequency, low margin per trade.
- **Statistical arbitrage** — find correlations between assets and trade when they diverge from their usual relationship.
- **Sentiment analysis** — analyze news, social media, and other text data to predict market movements.

Key components:
- **Signal generation** — the model that identifies trading opportunities
- **Risk management** — position sizing, stop losses, exposure limits. This is what keeps you alive.
- **Execution** — actually placing trades with minimal market impact and latency
- **Backtesting** — testing your strategy against historical data before risking real money

The danger: backtesting can be deceiving. Strategies that look amazing on historical data often fail in live markets. Overfitting, survivorship bias, and changing market conditions are real threats.

Related: [[Investing]], [[Data crunching]], [[Machine Learning]]
