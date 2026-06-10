# 🧠 System Story

Data flows through the system in this order:

1. Data is collected from external APIs (Twitter, TikTok, YouTube, News, Broadcast)
2. Airflow DAGs ingest and store raw data in PostgreSQL
3. AI models process the data (Sentiment + NER)
4. Data is structured into warehouse tables
5. Events are streamed through Kafka
6. Kafka consumers push data into Elasticsearch
7. Data is consumed by dashboards and analytics systems

This enables real-time + batch media intelligence across multiple platforms.
