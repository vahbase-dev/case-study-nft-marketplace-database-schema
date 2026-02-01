# 05 — Performance, Scaling, and Backups

## Goal
Keep the database stable under high write load and enable safe recovery.

## Performance
- partitioning-ready tables for receipts and trades
- batching for ingestion writes
- connection pooling and tuned statement timeouts

## Scaling
- read replicas for analytics and dashboards
- async pipelines for non-critical enrichment
- sharding by collection or tenant when required

## Backups
- PITR strategy
- periodic restore tests
- exportable receipts for projection rebuilds
