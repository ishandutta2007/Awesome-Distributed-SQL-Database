# Awesome-Distributed-SQL-Database

## Top Distributed SQL Database Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Horizontal Scalability, ACID Transactions & Cloud-Native Operations*  

**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Distributed SQL Databases**. These tools enable organizations to run relational workloads across multiple nodes—providing horizontal scaling, fault tolerance, and strong consistency without abandoning SQL or ACID transactions.

**Examples** include Amazon Aurora, Google Cloud SQL, Azure SQL Database, CockroachDB, PlanetScale, Neon, Supabase, SingleStore, YugabyteDB, and TiDB (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, horizontal sharding, and open distributed SQL infrastructure—ideal for database administrators, platform engineers, and organizations seeking transparent, vendor-independent relational databases.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global distributed SQL and cloud database market is estimated at approximately $25–30 billion in 2026, growing at a CAGR exceeding 20% propelled by cloud migration, microservices, and AI-driven data demands. The sector exhibits moderate concentration with a barbell dynamic: hyperscalers (AWS Aurora, Google Cloud SQL, Azure SQL) dominate commodity managed workloads, while specialized independent innovators (CockroachDB, TiDB, YugabyteDB, Neon) maintain defensible moats in multi-cloud resilience, geo-partitioning, and serverless developer ergonomics.

## SaaS/Hosted Platforms

| Company / Product | Size (Revenue / Valuation) | Pricing | Free Tier / Trial Limits | Description & Best For |
| :--- | :--- | :--- | :--- | :--- |
| **Microsoft Azure SQL Database** | Parent Market Cap: ~$3.1T; Cloud Revenue: ~$135B+/yr | Starting at ~$0.02/vCore-hour (Serverless) or ~$14.60/month (Basic DTU 5 DTUs, 2 GB) | Free for lifetime: 100,000 vCore-seconds/month (~32 vCore-hours), 32 GB storage, 1 free DB per subscription | Managed SQL Server with automated backups, high availability, and AI tuning. Best for Microsoft-centric enterprise workloads. |
| **Amazon Aurora** | Parent Market Cap: ~$2.1T; AWS Revenue: ~$105B+/yr | Serverless v2 starting at $0.12 per ACU-hour; Standard provisioned db.t4g.medium from ~$0.073/hour | Free trial: 12-month free tier for new accounts offering up to 4 ACUs with 1 GiB storage, plus $100 AWS credit | High-performance MySQL/PostgreSQL-compatible relational engine with decoupled compute and distributed storage. Best for AWS-native applications. |
| **Google Cloud SQL** | Parent Market Cap: ~$2.0T; Google Cloud Revenue: ~$45B+/yr | Starting from ~$0.015/hour (~$11/month for db-f1-micro, 1 vCPU, 0.6 GB RAM) + $0.17/GB storage/month | Free trial: 30-day free trial with Enterprise Plus configuration (PostgreSQL/MySQL) and $300 new customer credits | Fully managed MySQL, PostgreSQL, and SQL Server with zero-downtime maintenance. Best for teams on GCP wanting simple managed relational infrastructure. |
| **CockroachDB Cloud** | Valuation: ~$5.0B; Revenue: ~$150M+ ARR | Serverless Basic starts at $0.20 per 1M RUs; Standard dedicated provisioned nodes from $0.22/vCPU-hour (~$160/node/month) | Free for lifetime: Basic Serverless tier provides 50M Request Units (RUs) and 10 GiB storage free every month; $400 credits for 30-day trial | True distributed SQL with survivability and geo-partitioning across multi-cloud deployments. Best for global applications requiring strict ACID compliance. |
| **SingleStore** | Valuation: ~$1.3B; Revenue: ~$100M+ ARR | Shared starter compute workspace starting at $0.99/hour; Standard provisioned tier at $1.49/hour | Free tier: 1 free permanent Shared Workspace with limited capacity, plus $600 free credits for Standard tier evaluation | Distributed SQL database optimized for high-throughput HTAP, combining transactional and real-time analytical workloads. |
| **Supabase** | Valuation: ~$500M+; Revenue: ~$25M+ ARR | Micro compute starting at $10/month (1 GB RAM, 10 GB DB storage); Pro tier at $25/month base | Free for lifetime: Nano compute with 500 MB database storage, 1 GB file storage, 2 GB egress bandwidth, and 50,000 MAUs | PostgreSQL backend-as-a-service with auto-generated APIs, real-time subscriptions, storage, and authentication. Best for full-stack and web developers. |
| **Neon** | Valuation: ~$400M; Revenue: ~$10M+ ARR | Launch tier starts at $0.106/CU-hour (autoscaling up to 16 CU); storage at $0.35/GB-month | Free for lifetime: 100 CU-hours compute/month (runs a 0.25 CU compute for ~400 hours), 1 GB storage per project, across up to 100 projects | Serverless PostgreSQL with instantaneous copy-on-write branching, autoscaling, and scale-to-zero capabilities. Best for preview environments and modern serverless apps. |
| **PlanetScale** | Valuation: ~$300M+; Revenue: ~$15M+ ARR | Base plan starting at $39/month (includes 10 GB storage, 100M row reads, 10M row writes); extra storage $0.50/GB-month | Free trial: 14-day free trial for Hobby/Pro with full branching and up to 5 GB storage | Vitess-powered horizontally scalable MySQL with non-blocking schema migrations and database branching. Best for hyperscale MySQL workloads. |

## Open-Source GitHub Projects

The following active open-source projects power distributed SQL, horizontally scalable relational workloads, and distributed query processing. Sorted by GitHub star count in descending order:

1. **[ClickHouse](https://github.com/ClickHouse/ClickHouse)** [![GitHub stars](https://img.shields.io/github/stars/ClickHouse/ClickHouse?style=social&color=white)](https://github.com/ClickHouse/ClickHouse/stargazers)  
   Column-oriented distributed SQL DBMS for real-time analytical reporting (Apache-2.0). Blazing-fast SQL queries over petabytes of distributed data with linear scale-out.

2. **[DuckDB](https://github.com/duckdb/duckdb)** [![GitHub stars](https://img.shields.io/github/stars/duckdb/duckdb?style=social&color=white)](https://github.com/duckdb/duckdb/stargazers)  
   In-process SQL OLAP database management system (MIT). High-performance analytical query processing with seamless zero-copy integration across Apache Arrow, Parquet, and distributed analytical engines.

3. **[TiDB](https://github.com/pingcap/tidb)** [![GitHub stars](https://img.shields.io/github/stars/pingcap/tidb?style=social&color=white)](https://github.com/pingcap/tidb/stargazers)  
   Cloud-native, distributed SQL database for modern applications (Apache-2.0). MySQL protocol compatible with horizontal write scalability, strong consistency via Raft, and real-time HTAP engine.

4. **[SurrealDB](https://github.com/surrealdb/surrealdb)** [![GitHub stars](https://img.shields.io/github/stars/surrealdb/surrealdb?style=social&color=white)](https://github.com/surrealdb/surrealdb/stargazers)  
   Multi-model distributed database combining SQL, graph, and document store queries with distributed ACID transactions, real-time live queries, and granular permission access.

5. **[CockroachDB](https://github.com/cockroachdb/cockroach)** [![GitHub stars](https://img.shields.io/github/stars/cockroachdb/cockroach?style=social&color=white)](https://github.com/cockroachdb/cockroach/stargazers)  
   Cloud-native distributed SQL database architected for high availability, zero-downtime rolling upgrades, geo-partitioning, and strongly consistent distributed ACID transactions with PostgreSQL wire compatibility.

6. **[TDengine](https://github.com/taosdata/TDengine)** [![GitHub stars](https://img.shields.io/github/stars/taosdata/TDengine?style=social&color=white)](https://github.com/taosdata/TDengine/stargazers)  
   Open-source distributed time-series database with full SQL support (AGPL-3.0). High-throughput ingestion, data caching, stream processing, and multi-node clustering for IoT and industrial big data.

7. **[Neon](https://github.com/neondatabase/neon)** [![GitHub stars](https://img.shields.io/github/stars/neondatabase/neon?style=social&color=white)](https://github.com/neondatabase/neon/stargazers)  
   Serverless open-source alternative to AWS Aurora Postgres (Apache-2.0). Decouples compute and storage, offering instant database branching, scale-to-zero, and petabyte-scale cloud-native storage.

8. **[Vitess](https://github.com/vitessio/vitess)** [![GitHub stars](https://img.shields.io/github/stars/vitessio/vitess?style=social&color=white)](https://github.com/vitessio/vitess/stargazers)  
   Database clustering system for horizontal scaling of MySQL (Apache-2.0). Battle-tested at YouTube, Slack, and GitHub; encapsulates shard routing, dynamic resharding, connection pooling, and failover.

9. **[Apache ShardingSphere](https://github.com/apache/shardingsphere)** [![GitHub stars](https://img.shields.io/github/stars/apache/shardingsphere?style=social&color=white)](https://github.com/apache/shardingsphere/stargazers)  
   Distributed SQL ecosystem providing a transparent database gateway (Apache-2.0). Adds distributed transactions, horizontal sharding, read/write splitting, and data encryption to any standard relational database.

10. **[rqlite](https://github.com/rqlite/rqlite)** [![GitHub stars](https://img.shields.io/github/stars/rqlite/rqlite?style=social&color=white)](https://github.com/rqlite/rqlite/stargazers)  
    Lightweight, distributed relational database built on SQLite and the Raft consensus protocol (MIT). Provides effortless clustering, replication, and fault tolerance with an easy HTTP/SQL interface.

11. **[QuestDB](https://github.com/questdb/questdb)** [![GitHub stars](https://img.shields.io/github/stars/questdb/questdb?style=social&color=white)](https://github.com/questdb/questdb/stargazers)  
    High-performance, open-source distributed SQL time-series database (Apache-2.0). Column-oriented architecture with SIMD vectorization, InfluxDB Line Protocol ingestion, and PostgreSQL wire compatibility.

12. **[Apache Doris](https://github.com/apache/doris)** [![GitHub stars](https://img.shields.io/github/stars/apache/doris?style=social&color=white)](https://github.com/apache/doris/stargazers)  
    High-performance, real-time distributed analytical database (Apache-2.0). Supports high-concurrency point queries, sub-second reporting, and interactive analysis with standard MySQL protocol compatibility.

13. **[Citus](https://github.com/citusdata/citus)** [![GitHub stars](https://img.shields.io/github/stars/citusdata/citus?style=social&color=white)](https://github.com/citusdata/citus/stargazers)  
    PostgreSQL extension that transforms Postgres into a distributed database (AGPL-3.0). Horizontally shards tables across multiple nodes with distributed queries, reference tables, and columnar storage.

14. **[StarRocks](https://github.com/StarRocks/starrocks)** [![GitHub stars](https://img.shields.io/github/stars/StarRocks/starrocks?style=social&color=white)](https://github.com/StarRocks/starrocks/stargazers)  
    Next-generation sub-second distributed OLAP database (Apache-2.0). Features a vectorized execution engine, cost-based optimizer, real-time materialized views, and unified query acceleration over data lakes.

15. **[YugabyteDB](https://github.com/yugabyte/yugabyte-db)** [![GitHub stars](https://img.shields.io/github/stars/yugabyte/yugabyte-db?style=social&color=white)](https://github.com/yugabyte/yugabyte-db/stargazers)  
    High-performance distributed SQL database for mission-critical apps (Apache-2.0 core). Combines complete PostgreSQL runtime and wire compatibility with Google Spanner-inspired distributed Raft consensus and auto-sharding.

16. **[OceanBase](https://github.com/oceanbase/oceanbase)** [![GitHub stars](https://img.shields.io/github/stars/oceanbase/oceanbase?style=social&color=white)](https://github.com/oceanbase/oceanbase/stargazers)  
    Enterprise-grade distributed relational database designed for ultra-high transaction concurrency and multi-cloud resilience (MulanPubL-2.0). Native multi-tenancy, Paxos-based high availability, and HTAP capabilities.

17. **[Apache Ignite](https://github.com/apache/ignite)** [![GitHub stars](https://img.shields.io/github/stars/apache/ignite?style=social&color=white)](https://github.com/apache/ignite/stargazers)  
    Distributed database, caching, and in-memory data grid platform (Apache-2.0). Delivers distributed ACID transactions, ANSI-99 SQL support, machine learning APIs, and real-time processing capabilities.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Distributed SQL databases handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.
- **The "managed cloud SQL vs. distributed SQL" distinction matters.** **Amazon Aurora, Google Cloud SQL, and Azure SQL Database** are **managed single-node or primary-replica databases**—they scale vertically and via read replicas, but don't shard automatically . **TiDB, CockroachDB, and YugabyteDB** are **true distributed SQL**—they shard data across nodes and provide horizontal write scaling . **Choose based on whether you need read scaling (managed cloud SQL) or write scaling (distributed SQL).**
- **TiDB's MySQL compatibility is the lowest-friction migration path.** **Existing MySQL applications connect without driver changes** . **CockroachDB and YugabyteDB require PostgreSQL drivers** . **If your application is MySQL-native, TiDB is the obvious first evaluation.**
- **CockroachDB's license change matters for commercial adoption.** **Versions after November 2024 use the CockroachDB Software License**, not Apache-2.0 . **YugabyteDB's core is Apache-2.0**, but its management platform uses Polyform Free Trial License . **Review licensing before committing to a production deployment.**
- **Citus is for PostgreSQL teams who don't want to migrate.** **Install the extension and distribute tables**—your PostgreSQL skills, tools, and drivers all carry over . **The trade-off**: **AGPL-3.0** and the operational complexity of managing a distributed PostgreSQL cluster yourself.
- Self-hosted open-source solutions require proper cluster management, backup strategies, and ongoing maintenance. **Distributed databases are operationally complex**—budget for DBA expertise regardless of platform choice.

---

**Made for database administrators, platform engineers, and organizations building transparent distributed SQL solutions.**  
Let's make Distributed SQL Databases more open, data-driven, and scalable.
