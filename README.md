# SplitStream
![SplitStream logo](assets/logo.png)

**Real-time salary and subscription streaming in stablecoins on Solana**

## Overview
SplitStream lets DAOs and companies pay contributors continuously, second by second, instead of waiting for monthly payroll cycles. Payments flow as stablecoin streams on Solana, and recipients can withdraw their accrued balance at any time.

## Problem
Freelancers and DAO contributors often wait weeks to get paid for completed work. At the same time, payers have no easy way to adjust, pause, or cancel payment commitments as project scope or performance changes.

## Solution
SplitStream is a Solana program that creates payment streams which accrue stablecoins per second. Recipients see their balance grow in real time and can withdraw whenever they want. Payers can pause, cancel, or top up a stream instantly, with everything visible in a simple dashboard.

## Features (MVP)
- Create and fund a payment stream with a start time, end time, and rate
- Real-time balance accrual visible to both payer and recipient
- Instant withdrawal of accrued funds by the recipient
- Pause, cancel, and top-up controls for the payer
- Multi-recipient batch streaming for payroll runs

## Tech Stack
- Anchor, Rust (Solana program)
- Next.js (frontend dashboard)
- Solana Pay
- USDC SPL token
- Wallet Adapter

## How It Works
```
Payer Wallet
   |
   v
[Create Stream] --funds USDC--> [Anchor Program on Solana]
                                      |
                     accrues balance per second
                                      |
                                      v
                              Recipient Wallet
                        (withdraw anytime via dashboard)
```
1. Payer creates and funds a stream, setting start/end time and rate.
2. The on-chain program tracks elapsed time and accrues the recipient's withdrawable balance.
3. The recipient withdraws accrued USDC at any time through the dashboard.
4. The payer can pause, cancel, or top up the stream, with changes reflected instantly on-chain.
5. For payroll, payers can batch-create streams for multiple recipients in one flow.

## Roadmap
- Invoicing and tax-reporting export tools
- Support for multiple stablecoins with FX auto-conversion
- Integration with DAO tooling (Realms, Squads) for governance-approved payroll

## Pitch
- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team
- Name / Role — placeholder
- Name / Role — placeholder
- Name / Role — placeholder

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://ytakahashi2020.github.io/splitstream/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.
