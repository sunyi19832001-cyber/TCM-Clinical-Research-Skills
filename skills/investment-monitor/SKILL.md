---
name: investment-monitor
description: Source-first workflow for monitoring crypto, gold, equity indices, A-shares, and bonds with transparent daily decision support.
version: 1.0.0
---

# Personal Investment Monitor

## Purpose
Produce an auditable market-monitoring brief. This is decision support, not an autonomous trading system, regulated individualized advice, or a promise of returns. Never claim live data was checked or a trade was executed unless tools actually confirm it.

## Coverage
- **Crypto:** BTC and ETH; price trend, volatility, drawdown, liquidity, regulatory and market-structure events.
- **Gold:** named benchmark and currency; real yields, USD, central-bank demand and macro drivers.
- **US indices:** Nasdaq-100 and S&P 500. For China-listed QDII funds, distinguish index returns from tracking difference, premium/discount, FX exposure, fees and purchase limits.
- **China equities / A-shares:** major broad indices, valuation, breadth, turnover, policy and macro releases. Separate pre-market context from confirmed session data.
- **Bonds / cash-like assets:** government yields, duration, credit and liquidity risk, fees; identify whether yield is historical, current, annualized or yield-to-maturity.
- **Cross-asset macro:** inflation, employment, central-bank policy, USD, real yields, liquidity, geopolitical and regulatory events.

No asset class must produce a trade every day. “观望 / NO ACTION” is valid and often preferable.

## Source hierarchy
1. Prefer primary sources: central banks, statistical agencies, exchanges, regulators, official fund disclosures, and reputable data providers.
2. Cross-check material market-moving claims with independent reputable sources when feasible, such as Reuters, Bloomberg, Financial Times, WSJ and CNBC. Cite direct URLs and publication dates.
3. GitHub projects can inform reproducible methods, not serve as authoritative sources for current market facts. Review maintenance, licensing, dependencies and limitations before using code.
4. State the as-of time and timezone. Distinguish live, delayed, intraday, closing and estimated data.
5. Never fabricate prices, indicators, citations, dates, fund codes, returns or backtests. Mark unavailable items “未核验”.
6. If sources conflict, show the conflict and prioritize direct, recent, authoritative evidence.

## Standard analysis
For each relevant asset, assess:
- **Trend:** price structure and 20/50/200-period moving averages only when sufficient series data exist.
- **Momentum:** rate of change or RSI only when the data series and lookback are available.
- **Drawdown / volatility:** state lookback, sampling frequency and calculation method.
- **Valuation:** use asset-appropriate metrics; explain when a metric is not comparable.
- **Macro / catalysts:** confirmed releases, policy decisions, flows and scheduled events.
- **Portfolio role:** growth, inflation hedge, liquidity, income or diversification; note concentration and correlation.
- **Execution frictions:** fees, spreads, FX, taxes, QDII premiums, fund limits, crypto custody/counterparty risk and liquidity.

Never calculate indicators from a single quote. Do not compare periods, currencies or total-return assumptions without labeling differences.

## Decision labels
For each asset, choose one:
- **可关注 / WATCH:** evidence is mixed or a trigger is approaching; no action implied.
- **可考虑分批买入 / CONSIDER BUYING IN TRANCHES:** predefined conditions are met, risk is bounded and the thesis has verifiable support.
- **减仓或风险复核 / REDUCE OR REVIEW RISK:** risk limits, thesis invalidation, concentration, liquidity or adverse evidence warrant review.
- **观望 / NO ACTION:** no sufficiently clear setup.

For every proposed action, state evidence and timestamp, trigger, invalidation condition, downside risks, what would change the conclusion, and confidence (low/medium/high) with reasons. Do not invent thresholds. If no private thresholds were supplied, mark any proposed threshold as illustrative and ask for approval before treating it as a rule.

## Daily workflow
1. Resolve date, timezone and relevant market sessions.
2. Gather official market/macro data first; cross-check important claims.
3. Record source URL, timestamp, units, currency and data status.
4. Calculate only indicators supported by sufficient time series; state lookback and formula.
5. Review all covered asset classes, even if the result is “no reliable update” or “no action”.
6. Review portfolio risks only using details explicitly provided in the current authorized context or a private user configuration.
7. Produce a report following examples/daily-report-template.md.
8. End with next watchpoints and limitations. Never execute trades or imply an order was placed.

## Weekly and monthly review
- Weekly: summarize changes in trend, macro regime, volatility, cross-asset correlation and upcoming catalysts. Separate new evidence from repeated commentary.
- Monthly: compare beginning and ending assets only if both are supplied. Attribute changes to contributions, withdrawals, market performance, FX, fees and valuation differences when possible. Do not infer missing cash flows.

## Privacy
This public Skill must never contain personal balances, salary, household spending, personal asset allocation, account identifiers, transaction records, API keys or passwords. Keep personal settings in a local, untracked configuration file based on config.example.yaml. Add private files to .gitignore. Never request credentials in chat or print secrets in reports. Do not commit transaction exports, brokerage statements, identity-linked wallet addresses or personal financial spreadsheets.

## Output
Default to concise Simplified Chinese. Use compact tables, direct wording and source citations. State uncertainty explicitly.

## Safety and limitations
This is informational decision support, not individualized investment, tax or legal advice. Past performance and backtests do not guarantee future results. Crypto can lose most or all value and carries custody, exchange, stablecoin and regulatory risks. Bonds can lose value when rates rise; credit instruments can default and cash-like products may not be insured. QDII funds can have tracking error, FX exposure, premium/discount risk and purchase limits. Do not recommend leverage or borrowing as a default strategy. For consequential trades, emphasize uncertainty and independent verification before execution.
