# Market & Quant Analytics Lab Docs

Public-safe navigation hub for Michael Panico's market-data, financial-data, and quant-adjacent analytics proof shells.

This repository does not publish private source code. It explains how the public documentation shells fit together while keeping implementation repos, OAuth tokens, broker/API state, SQLite databases, watchlists, Discord/n8n/TradingView state, and production experiments private.

## Recruiter Snapshot

The market / quant analytics lane demonstrates:

- Python market-data ingestion and normalization.
- SQLite-backed local data organization.
- Streamlit and Plotly dashboard review.
- Risk, volatility, expected-move, and options-research concepts.
- Backtesting and no-lookahead validation discipline.
- Public/private source-governance judgment.
- Quant-adjacent analytics interest without claiming professional quant trader, quant developer, or production trading-platform experience.

The main public portfolio page for this lane is:

- [Institutional Market Data Engine](https://www.michaelspanico.com/projects/institutional-market-data-engine)

The lightweight GitHub Pages landing page for this hub is:

- [Market & Quant Analytics Lab Pages](https://mp2123.github.io/Market-Quant-Analytics-Lab-Docs/)

## Ecosystem Map

| Public surface | Role in the ecosystem | Public link |
| --- | --- | --- |
| Institutional Market Data Engine Docs | Primary market-data engineering proof shell: ingestion, SQLite storage, dashboard review, and public/private boundary. | [Open repo](https://github.com/mp2123/Institutional-Market-Data-Engine-Docs) |
| Market Data Dashboard Docs | Dashboard and source-governance proof shell: Streamlit review, market-data observability, validation boundaries, and private runtime separation. | [Open repo](https://github.com/mp2123/Market-Data-Dashboard-Docs) |
| QuantStrat ML Docs | Research and validation proof shell: backtesting, options/volatility analytics, expected-move research, no-lookahead discipline, and model evaluation boundaries. | [Open repo](https://github.com/mp2123/QuantStrat-ML-Docs) |
| Portfolio Website Docs | Public docs shell for the private portfolio implementation and recruiter-facing website architecture. | [Open repo](https://github.com/mp2123/Portfolio-Website-Docs) |
| Live portfolio | Recruiter-facing narrative layer that explains the projects without exposing private implementation details. | [Open site](https://www.michaelspanico.com/projects/institutional-market-data-engine) |

## Sanitized Internal Source-Lineage Map

The private local ecosystem uses a clearer internal structure than the public GitHub surface. This public hub borrows the structure, not the private paths:

| Internal lane | Public-safe description | Public treatment |
| --- | --- | --- |
| Production Engine | Private production/runtime QuantStrat engine and operational source lineage. | Mention only as private runtime boundary; do not link publicly. |
| ML Research Lab | Private QuantStrat ML research workspace for backtesting, expected-move, volatility, and validation artifacts. | Public summary lives in [QuantStrat ML Docs](https://github.com/mp2123/QuantStrat-ML-Docs). |
| Schwab / Market-Data Ingestion | Private ingestion workspace for authorized market-data access and local storage. | Public summary lives in [Institutional Market Data Engine Docs](https://github.com/mp2123/Institutional-Market-Data-Engine-Docs). |
| Streamlit Dashboard | Private market-data dashboard and review workspace. | Public summary lives in [Market Data Dashboard Docs](https://github.com/mp2123/Market-Data-Dashboard-Docs). |
| Public Documentation | Public docs-shell layer for recruiter-safe review. | This hub links the public docs shells together. |
| MacOS Automations | Local LaunchAgent/monitoring/support automation around private runtime workflows. | Not public proof; mention only as private runtime state. |

## Private Boundary

The following are intentionally not public:

- private implementation repos;
- Schwab/Plaid/API credentials, OAuth token files, `.env` files, webhook secrets, or broker credentials;
- SQLite runtime databases, exported account-specific records, and private watchlists;
- Discord, n8n, TradingView, Streamlit runtime state, monitor payloads, or local machine automation;
- production QuantStrat runtime code and account/broker-specific workflows;
- private research artifacts, local backtest output, raw model registries, or unsanitized screenshots.

## What This Hub Does Not Claim

This hub does not claim that Michael operates a public live trading system, broker automation platform, professional quant production stack, or institutional trading desk. It documents market-data analytics, dashboarding, validation discipline, and quant-adjacent research proof in a recruiter-safe way.

## Suggested Reading Path

1. Start with the [portfolio project page](https://www.michaelspanico.com/projects/institutional-market-data-engine) for the recruiter narrative.
2. Review [Institutional Market Data Engine Docs](https://github.com/mp2123/Institutional-Market-Data-Engine-Docs) for the primary data-engineering proof shell.
3. Use [Market Data Dashboard Docs](https://github.com/mp2123/Market-Data-Dashboard-Docs) for dashboard/source-governance context.
4. Use [QuantStrat ML Docs](https://github.com/mp2123/QuantStrat-ML-Docs) for research, expected-move, volatility, and validation context.
5. Treat all private production/runtime material as source lineage only, not as a public proof surface.

## Internal Sections

- [Institutional Market Data Engine](./institutional-market-data-engine/README.md)
- [Market Data Dashboard](./market-data-dashboard/README.md)
- [QuantStrat ML Research Framework](./quantstrat-ml/README.md)
- [Source Governance](./source-governance/README.md)
- [Privacy Boundaries](./privacy-boundaries/README.md)
- [Validation Notes](./validation-notes/README.md)
- [Private Runtime Boundary](./private-runtime-boundary/README.md)

## GitHub Pages Decision

This hub is Pages-ready but still Markdown-first.

The root `index.md` gives GitHub Pages a simple entry point if Pages is enabled later. There is no custom build, no generated static site, and no duplicate private content. The portfolio website remains the primary polished public web surface; Pages would only provide a lightweight docs landing page for the market / quant proof shells.
