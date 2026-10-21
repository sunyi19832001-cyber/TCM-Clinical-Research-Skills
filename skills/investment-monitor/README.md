# Investment Monitor Skill

A reusable, source-first workflow for monitoring crypto, gold, equity indices, A-shares and bonds.

## Files
- [SKILL.md](SKILL.md): evidence hierarchy, analytical framework and decision labels.
- [config.example.yaml](config.example.yaml): safe example configuration with no personal financial data.
- [examples/daily-report-template.md](examples/daily-report-template.md): daily report structure.
- [PRIVACY.md](PRIVACY.md): public release checklist.

## Use
In an AI environment that supports instruction-based Skills, load SKILL.md and request a daily market brief, weekly review or monthly portfolio review. Fresh information requires access to reliable current data or web/search tools.

Example prompt:

> Read this Skill and prepare today's investment monitoring brief. Cover BTC, ETH, gold, Nasdaq-100, China broad-market indices/A-shares, and bonds. Prioritize official data, cross-check material claims, include timestamps and source URLs, and say “观望” where evidence does not justify action. Do not invent missing prices or indicators.

## Important
This directory contains instructions, not a continuously running service. Scheduled monitoring requires a separate scheduler and current data access. Buy/sell labels are decision support, not trade execution or guaranteed returns.

Do not place private balances, holdings, account details, transaction records or credentials in this public directory.
