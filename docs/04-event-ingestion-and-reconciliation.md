# 04 — Event Ingestion and Reconciliation

## Goal
Project on-chain events into off-chain state deterministically.

## Ingestion
- store raw event receipts with block/tx/log identifiers
- dedupe using unique keys (chain_id, tx_hash, log_index)

## Reconciliation
- replay-safe consumers
- idempotent writes
- handle reorgs via safe-block strategy
- rebuild projections from receipts when needed

## Outcome
Off-chain state remains consistent with chain truth under retries and replays.
