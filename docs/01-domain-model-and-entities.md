# 01 — Domain Model and Entities

## Goal
Define the canonical domain entities for a high-throughput NFT marketplace.

## Core Entities (Conceptual)
- users and wallets
- collections and tokens
- listings and orders
- trades and fills
- balances and settlement receipts
- chain events and ingestion receipts

## Principles
- separate write models from read models
- store immutable event receipts
- represent state as a deterministic projection from events + writes
