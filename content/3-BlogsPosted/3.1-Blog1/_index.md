---
title: "Blog 1"
date: 2026-07-13
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# BLOG 1: REDUCING LATENCY FROM SECONDS TO MILLISECONDS: THE ART OF CACHING ON AWS

Hi everyone, in the process of system optimization, there is one metric that always haunts our team: **Latency**. Seeing a spinning web page taking 2-3 seconds to load data, while users constantly press F5, is truly a nightmare.

Typically, the culprit behind 90% of system bottlenecks is the traditional Database (RDS/SQL). As the application grows, the volume of incoming queries increases, forcing the database to handle complex JOIN and SELECT statements from thousands of users simultaneously. CPU usage spikes to 90%, and the system starts to "choke".

Instead of choosing the costly solution of scaling up the database instance to expensive tiers, our team applied a familiar yet highly effective cloud technique: **Optimizing the caching layer with Amazon ElastiCache**. The results were incredibly impressive, with latency dropping from seconds to sub-millisecond levels, while completely offloading the database.

---

## 1. Amazon ElastiCache: A Super-Fast "First Aid Station" on RAM

To understand why this solution is so fast, we need to look at the nature of data storage.

Traditional databases like MySQL or PostgreSQL store data on disk drives (SSD/HDD). No matter how fast today's SSDs are, reading/writing from disk must pass through physical layers and complex algorithms.

In contrast, **Amazon ElastiCache** is a fully managed in-memory data store service by AWS. This system supports two highly popular engines: Redis and Memcached. Because the data resides entirely in RAM, ElastiCache's response speed is incredibly fast, measured in milliseconds or even microseconds.

Instead of forcing the main database to constantly compute data that rarely changes (such as product categories, system configurations, user profiles, hot articles, etc.), we store that data directly in ElastiCache's RAM. In this setup, ElastiCache acts as a super-fast first aid station, intercepting most requests before they can reach and bottleneck the main database.

---

## 2. Post Link

View the detailed post and join the discussion on Facebook: 👉 [Facebook Shared Post](https://www.facebook.com/share/p/1GNrhrDMKH/)