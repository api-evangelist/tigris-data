---
title: "The Most Expensive ClickHouse Query Is the Restore"
url: "https://www.tigrisdata.com/blog/clickhouse-zero-egress/"
date: "2026-07-16"
feed_url: "https://www.tigrisdata.com/blog/rss.xml"
---
Self-hosted ClickHouse runs on cheap compute, but its backups and cold tier usually live on AWS S3, and AWS charges $0.09/GB to read your own data back. Point BACKUP TO S3 and TTL tiering at Tigris instead. You keep the same stock ClickHouse features, you pay zero egress fees, and disaster recovery drills cost nothing to run.
