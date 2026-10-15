# Systematic Portfolio · Live Dashboard

**Live page: https://kavyashah0607-star.github.io/portfolio-dashboard/**

A rules-based portfolio, paper-traded automatically by a cloud server: 47 years of tested history, a live record, and the failed ideas shown alongside the ones that worked. Personal project by Kavya Shah.

## What it is

- **Strategy:** a diversified, trend-following core plus a smaller leveraged US-stock satellite; both step aside into T-bills when their markets turn down.
- **Backtest 1979–2026:** 14.0% a year vs 12.5% for the S&P 500; worst fall −39% vs −50% (after modelled trading costs, before taxes and fund fees). Past and simulated results don't predict future returns.
- **Limits, shown openly:** the extra return relies mostly on US stocks staying strong, and in the 1987 one-day crash the plan fell more than the market.

## How the research is done

- **Pre-registered:** each test's design is saved before it runs, so a bad result can't be explained away afterwards.
- **Everything logged:** 1,100+ logged backtests, most of them failures; the rejected ideas are listed on the page.
- **Checked against luck:** a signal must beat random timing with the same market exposure, on recent years kept out of the design.
- **Independent review:** results are reproduced and code-reviewed by a second reviewer before anything is used.

## How it runs

A cloud server (AWS) runs the engine every weekday, places paper orders through a broker API, checks its own health every few hours with phone alerts, and publishes this page's data nightly. The page shows percentages and asset classes only.

## Files

- `index.html`: the page (no frameworks; SVG charts; light and dark mode; works on phones)
- `data.json`: live data, refreshed nightly
- `research.json`: backtest, crash windows and research grades

The strategy code itself is private. Built with AI coding tools under my direction: I set the strategy, the research rules and the reviews.

*Paper money only. Nothing here is investment advice.*
