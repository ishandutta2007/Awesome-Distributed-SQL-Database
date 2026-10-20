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

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **Amazon Aurora**

  **AWS's MySQL- and PostgreSQL-compatible managed database** with distributed storage and read replicas. **Pricing**: **Aurora Serverless** bills per ACU-hour (1 ACU ≈ 2 GiB memory); **Aurora Standard** includes instance hours + storage + per-request I/O; **Aurora I/O-Optimized** eliminates per-request I/O charges for I/O-heavy workloads . **Free tier**: **$100 AWS credit** for new customers, plus **Aurora PostgreSQL Serverless** with up to **4 ACUs and 1 GiB storage** for 12 months . **Best for**: AWS-native teams wanting managed MySQL/PostgreSQL with horizontal read scaling.



- **Google Cloud SQL**

  **Fully managed MySQL, PostgreSQL, and SQL Server** with automatic backups, replication, and patching. **Pricing**: **Enterprise Plus** edition includes **99.99% SLA**, near-zero downtime maintenance, and data cache for read-heavy workloads . **Free tier**: **30-day free trial** with Enterprise Plus configuration (PostgreSQL/MySQL) and **$300 Google Cloud credits** for new customers . **Best for**: teams on GCP wanting managed relational databases without sharding complexity.



- **Azure SQL Database**

  **Microsoft's managed SQL Server** with built-in high availability and intelligence. **Pricing**: **Business Critical** tier starts at **~¥13,897/month (~$1,900)** for 4 vCores with 20.4 GB memory; **Azure Hybrid Benefit** cuts costs by **~51%** for existing SQL Server licenses . **Free tier**: **Free offer** with 100,000 vCore-seconds/month and 32 GB storage for the lifetime of the subscription (limited to one database per subscription). **Best for**: Microsoft-centric enterprises needing managed SQL Server.



- **CockroachDB Cloud**

  **Managed CockroachDB** with three plans: **Basic** (usage-based Request Units, no provisioned compute), **Standard** (provisioned vCPUs + usage-based storage/backups/CDC), and **Advanced** (provisioned compute + IOPS) . **Pricing example**: 32 vCPU multi-region GCP cluster = **$3.872/hour** based on highest regional rate . **Free tier**: **Basic plan** includes **$400 in free credits** for 30 days; **Serverless** free tier offers **10 GiB storage and 50M Request Units/month** . **Best for**: global applications needing geo-partitioning and survivability.



- **PlanetScale**

  **Vitess-based MySQL-compatible managed database** with branching and non-blocking schema changes. **Pricing**: **Base plan** includes **10 GB storage**; additional storage **$0.50/GB/month** (Vitess) or **$1.50/GB** (HA production); cluster sizes from **PS-10** upward . **Free tier**: **Hobby plan** with **5 GB storage and 1 billion row reads/month** for one production branch. **Best for**: teams wanting MySQL scaling with Git-like database branching.



- **Neon**

  **Serverless PostgreSQL** with scale-to-zero and branching. **Pricing**: **Launch plan** at **$0.106/CU-hour** (autoscaling to 16 CU); **Scale plan** at **$0.222/CU-hour** (up to 56 CU); storage **$0.35/GB-month** . **Free tier**: **100 CU-hours per project per month** (enough for a 0.25 CU compute running ~400 hours) and **1 GB storage per project** across up to 100 projects . **Best for**: developers wanting pay-per-use Postgres with instant branching.



- **Supabase**

  **PostgreSQL-based backend-as-a-service** with auth, storage, and realtime. **Pricing**: **Micro** compute **~$10/month** (1 GB RAM, 10 GB DB); **Small** **~$15/month** (2 GB RAM, 50 GB DB); **Medium** **~$60/month** (4 GB RAM, 100 GB DB) . **Free tier**: **Nano** compute with **0.5 GB RAM** and **500 MB database** storage, plus 1 GB file storage and 2 GB bandwidth . **Best for**: full-stack apps wanting Postgres with bundled backend services.



- **SingleStore**

  **Distributed SQL database** for real-time analytics and transactions (HTAP). **Pricing**: **Shared** tier starts at **$0.99/hour** (evaluation/dev); **Standard** starts at **$1.49/hour** with **$600 free credits**; **Enterprise** custom . **Free tier**: **1 free Shared Workspace** with limited resources; **$600 credits** for Standard tier evaluation . **Best for**: real-time dashboards and HTAP workloads.



## Open-Source GitHub Projects



- **TiDB**

  **Open-source, cloud-native, distributed SQL database designed for modern applications** (Apache-2.0) — **the MySQL-compatible HTAP choice** . **40,442 GitHub stars** . **MySQL protocol compatible**—existing applications connect without driver changes . **Raft + Percolator** architecture separates compute (TiDB) from storage (TiKV) . **Features**: **horizontal scaling**, **ACID transactions**, **real-time analytics**, and **native vector search** for agentic workloads . **TiDB Operator** manages clusters on Kubernetes . **The reference implementation for MySQL-compatible distributed SQL**—**choose when you want HTAP with MySQL ecosystem compatibility**.



- **CockroachDB**

  **Cloud-native, distributed SQL database designed for high availability, effortless scale, and control over data placement** (CockroachDB Software License for versions after Nov 2024) — **the geo-partitioning choice** . **PostgreSQL wire protocol compatible**—use any PostgreSQL driver or ORM . **Survives disk, machine, rack, and datacenter failures** with minimal latency disruption and no manual intervention . **Strongly-consistent ACID transactions** with horizontal scaling . **The trade-off**: **license changed from Apache-2.0 to CockroachDB Software License** in November 2024—review commercial terms before adoption . **Best for**: global applications needing survivability and data placement control.



- **YugabyteDB**

  **Cloud-native distributed SQL database for mission-critical applications** (Apache-2.0 for core database) — **the PostgreSQL-compatible choice** . **10,386 GitHub stars** . **PostgreSQL fork rebased to version 15.0** with **YSQL API** supporting foreign keys on partitioned tables, stored generated columns, and parallel queries . **Features**: **HNSW indexing for pgvector** (AI-native vector search), **automatic transactional xCluster DDL replication**, and **cost-based optimizer** with bitmap scan support . **License split**: core database is **Apache-2.0**; **YugabyteDB Anywhere** (management platform) uses **Polyform Free Trial License** . **Best for**: teams wanting PostgreSQL compatibility with horizontal scaling and vector search.



- **Citus**

  **Distributed PostgreSQL as an extension** (AGPL-3.0) — **the extension-based choice** . **12,523 GitHub stars** . **Adds sharding to existing PostgreSQL**—install the extension and distribute tables without changing your database . **Features**: **`create_distributed_table`** for transparent sharding, **reference tables** replicated across nodes, **columnar storage** for analytics, and **co-location** for distributed joins . **The trade-off**: **AGPL-3.0 license**—copyleft requirements for modifications . **Best for**: PostgreSQL users wanting to scale out without migrating to a new database.



- **Vitess**

  **Database clustering system for horizontal scaling of MySQL** (Apache-2.0) — **the MySQL sharding standard** . **19,498 GitHub stars** . **Powers YouTube's database infrastructure since 2011**—grown to tens of thousands of MySQL nodes . **Encapsulates shard-routing logic**—application code remains agnostic to data distribution . **Features**: **live resharding with atomic cutover**, **connection pooling**, **automated failover and backups**, and **topology tracking** . **The reference implementation for MySQL horizontal scaling**—**choose when you need YouTube-scale MySQL**.



### Additional Strong Open-Source Options



- **Apache ShardingSphere** — **Distributed SQL ecosystem** (Apache-2.0) . **Sharding, read/write splitting, and data encryption** for any JDBC-compatible database.

- **Greenplum** — **MPP data warehouse** (Apache-2.0) . **PostgreSQL-based** with parallel query execution.

- **Apache Doris** — **Real-time analytical database** (Apache-2.0) . **MySQL protocol compatible** with lakehouse federation.

- **StarRocks** — **High-performance OLAP database** (Apache-2.0) . **Sub-second queries on data lake and warehouse**.

- Community **n8n** workflows for distributed database monitoring and failover alerting.



**Frameworks for building custom systems**: Combine **TiDB** for MySQL-compatible HTAP with **CockroachDB** for geo-partitioned survivability, **YugabyteDB** for PostgreSQL-compatible scaling, **Citus** for extension-based sharding, and **Vitess** for YouTube-scale MySQL—creating a comprehensive distributed SQL stack.



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
