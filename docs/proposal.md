# SplitStream

_Real-time salary and subscription streaming in stablecoins on Solana_

## Summary

SplitStream lets DAOs and companies pay contributors continuously, second-by-second, instead of monthly, using stablecoin streams on Solana. Recipients can withdraw accrued funds anytime, and payers can pause or adjust streams instantly, improving cash flow and trust.

## Target users

DAOs, remote teams, freelance contractors, subscription businesses

## Problem

Freelancers and DAO contributors often wait weeks for payment, while payers lack flexibility to adjust or pause commitments as work progresses.

## Solution

A Solana program creates payment streams that accrue stablecoins per second, letting recipients withdraw anytime and payers modify streams on the fly, all visible in a simple dashboard.

## MVP features

- Create/fund a payment stream with start/end and rate
- Real-time balance accrual visible to both parties
- Instant withdrawal of accrued funds by recipient
- Pause/cancel/top-up stream controls for payer
- Multi-recipient batch streaming for payroll runs

## Chains

Solana

## Tech

Anchor, Rust, Next.js, Solana Pay, USDC SPL token, Wallet Adapter

## Category

Payments

## Why now

Stablecoin payroll and streaming payments are gaining traction as remote/DAO work grows, and Solana's speed makes true per-second streaming practical and cheap.

## Roadmap

- Add invoicing and tax-reporting export tools
- Support multiple stablecoins and FX auto-conversion
- Integrate with DAO tooling (Realms, Squads) for governance-approved payroll
