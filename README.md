# DojiFunded

> A crypto **perpetual-futures prop-trading platform** on Arbitrum One.
> [`dojifunded.com`](https://dojifunded.com)

---

## Overview

**DojiFunded** is a **funded-trader platform** for crypto perpetuals. A trader takes an evaluation **challenge**, trades the major perp markets, and on reaching the profit objective within the risk limits earns a **funded account** — with real profit withdrawals settled on-chain in USDC.

The platform pairs a **professional trading terminal** with **on-chain proof of results**, so a trader's track record is verifiable, portable, and tamper-proof.

---

## Why DojiFunded

- **Real markets, real payouts.** Trade the most liquid crypto perps with live pricing and withdraw profits in **USDC on Arbitrum**.
- **Flexible programs.** **Instant Funding**, **1-Step**, **2-Step Classic**, and **2-Step Elite**, across account sizes from **$1,000 to $100,000**.
- **On-chain proof.** Every result can mint a **"Verified on chain" certificate** — a tamper-proof NFT of the trade (entry/exit, PnL, fees).
- **AI trading assistant.** An in-app agent helps traders analyse markets and their own performance.
- **Built-in growth.** **Copy trading**, **affiliate / KOL** share-links, and **referral** rewards.
- **Fast, polished UX.** TradingView charts, one-click wallet onboarding, and instant USDC funding.

---

## Product surfaces

| Surface | Description |
|---|---|
| [`app.dojifunded.com`](https://app.dojifunded.com) | The trading terminal — buy a challenge, trade, manage positions, withdraw. |
| Explorer | Public viewer for the on-chain trade certificates. |

---

## Repositories

A high-level map of the codebase.

### Trading core
| Repo | Description | Stack |
|---|---|---|
| **doji-perp-engine** | The proprietary engine — order matching, risk management, and account accounting. | Rust |
| **doji-price-oracle** | Real-time market pricing and chart (OHLC) history. | Rust |
| **doji-onchain-trading** | On-chain smart contracts — custody, payouts, and trade certificates. | Solidity |

### Applications & services
| Repo | Description | Stack |
|---|---|---|
| **doji-interface** | The trader web app (trading terminal, dashboard, onboarding). | React + Vite (TS) |
| **doji-auth-backend** | Core backend — accounts, payments & funding, challenge lifecycle, and growth features. | TypeScript |
| **doji-explorer** | Public explorer for on-chain trade certificates. | React + Vite (TS) |
| **doji-copy-engine** | Copy-trading service. | Node (TS) |
| **doji-agent-engine** | AI trading-assistant service. | Node (TS) |
| **doji-backtesting-enigne** *(sic — repo-name typo)* | Strategy backtesting. | Rust |

---

## Tech stack

- **Core:** Rust (engine, pricing, backtesting) · Solidity (contracts)
- **Applications:** TypeScript — React + Vite (web) · Express / Fastify (services)
- **Chain:** Arbitrum One · USDC settlement
- **Auth:** wallet sign-in (SIWE) + email
- **Charts:** TradingView Advanced Charts

---

*© DojiFunded. Built for serious crypto traders.*
