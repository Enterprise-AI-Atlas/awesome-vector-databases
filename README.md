# Awesome Vector Databases

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)

A curated registry of vector databases, vector stores, vector-search libraries, and benchmarks for AI, RAG, and semantic-search applications.

The goal is to be the definitive place to discover and compare production-grade vector data systems — from managed cloud services and self-hosted engines to embedded libraries and hybrid search platforms.

**Inclusion criteria:** Resources must provide native vector storage, indexing, or similarity search as a core capability. General SQL databases without vector extensions are out of scope. See [CONTRIBUTING.md](./CONTRIBUTING.md) for the full quality bar.

---

## Contents

- [Managed Vector Databases](#managed-vector-databases)
- [Self-Hosted Vector Databases](#self-hosted-vector-databases)
- [Embedded Vector Stores](#embedded-vector-stores)
- [Graph + Vector](#graph--vector)
- [Time-Series + Vector](#time-series--vector)
- [Vector Search Libraries](#vector-search-libraries)
- [Hybrid Search](#hybrid-search)
- [Benchmarks](#benchmarks)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

---

## Managed Vector Databases

Fully managed cloud services that provide vector storage, indexing, and similarity search without infrastructure overhead.

- **[Pinecone](https://www.pinecone.io/)** `Official` — Managed vector database with metadata filtering, hybrid search, and no-index tuning.
- **[Zilliz Cloud](https://zilliz.com/cloud)** `Official` — Fully managed Milvus service with GPU indexing and enterprise security.
- **[Weaviate Cloud](https://weaviate.io/cloud)** `Official` — Managed vector search engine with built-in vectorization and GraphQL interface.
- **[Qdrant Cloud](https://qdrant.tech/cloud/)** `Official` — Managed Qdrant cluster service with quantization and hybrid search.
- **[DataStax Astra DB](https://www.datastax.com/products/datastax-astra)** `Official` — Managed Cassandra-compatible database with vector search for RAG.
- **[Chroma Cloud](https://www.trychroma.com/cloud)** `Official` — Managed service for the Chroma embedded vector store.
- **[Azure AI Search](https://azure.microsoft.com/en-us/products/ai-services/ai-search)** `Official` — Cloud search service with vector and hybrid retrieval.
- **[AlloyDB AI](https://cloud.google.com/alloydb?hl=en)** `Official` — Google Cloud managed PostgreSQL with vector search and AI integrations.
- **[SingleStore](https://www.singlestore.com/)** `Official` — Distributed SQL database with SingleStore-V integrated vector search.
- **[MyScale](https://myscale.com/)** `Official` — ClickHouse-based managed vector database for structured + vector data.

---

## Self-Hosted Vector Databases

Production-ready vector databases you can deploy on your own infrastructure.

- **[Milvus](https://milvus.io/)** `Official` — Open-source distributed vector database with GPU support and cloud-native architecture.
- **[Qdrant](https://qdrant.tech/)** `Official` — Open-source vector database in Rust with filtering, quantization, and hybrid search.
- **[Weaviate](https://weaviate.io/)** `Official` — Open-source vector search engine with modular AI integrations.
- **[pgvector](https://github.com/pgvector/pgvector)** `Official` — PostgreSQL extension for vector similarity search with HNSW and IVFFlat indexes.
  - Install: `CREATE EXTENSION vector;` or use the pre-built Docker image.
- **[Chroma](https://www.trychroma.com/)** `Official` — AI-native open-source embedding database for local and production deployments.
- **[Vespa](https://vespa.ai/)** `Official` — Big data serving engine with native vector search, ranking, and tensors.
- **[Vald](https://vald.vdaas.org/)** `Official` — Cloud-native, highly scalable distributed vector search engine.
- **[Marqo](https://www.marqo.ai/)** `Official` — End-to-end vector search engine with built-in embedding generation.
- **[OpenSearch](https://opensearch.org/)** `Official` — Open-source search and analytics suite with k-NN vector search.
- **[Elasticsearch](https://www.elastic.co/elasticsearch)** `Official` — Distributed search engine with dense and sparse vector search.
- **[Redis Stack](https://redis.io/)** `Official` — In-memory data platform with vector similarity search via RediSearch.
- **[Couchbase](https://www.couchbase.com/)** `Official` — Distributed NoSQL database with vector search for RAG applications.

---

## Embedded Vector Stores

Lightweight, in-process vector stores and libraries for local development and edge deployments.

- **[Chroma](https://www.trychroma.com/)** `Official` — Popular embedded vector store with simple Python/JS APIs.
- **[FAISS](https://github.com/facebookresearch/faiss)** `Official` — Facebook AI Similarity Search library for efficient nearest-neighbor search.
- **[LanceDB](https://lancedb.com/)** `Official` — Serverless vector database built on the Lance columnar format.
- **[SQLite-vec](https://github.com/asg017/sqlite-vec)** `Community` — SQLite extension for vector search, designed for edge and embedded use.
- **[Voyager](https://github.com/spotify/voyager)** `Official` — Spotify's approximate nearest-neighbor search library with a Python/Java/C++ API.
- **[HNSWLib](https://github.com/nmslib/hnswlib)** `Community` — Header-only HNSW implementation with Python bindings.
- **[Annoy](https://github.com/spotify/annoy)** `Official` — Spotify's approximate nearest-neighbor library using random projections.
- **[ScaNN](https://github.com/google-research/google-research/tree/master/scann)** `Official` — Google's scalable nearest-neighbor search library.
- **[USearch](https://github.com/unum-cloud/usearch)** `Official` — Fast, compact, and broadly compatible single-file similarity search engine.
- **[Vectorlite](https://github.com/1yef/vectorlite)** `Community` — SQLite-like embedded vector database with HNSW indexing.

---

## Graph + Vector

Graph databases that combine vector similarity search with relationship traversal for GraphRAG and knowledge-graph workloads.

- **[Neo4j](https://neo4j.com/)** `Official` — Graph database with native vector indexes and GenAI integrations.
- **[ArangoDB](https://arangodb.com/)** `Official` — Multi-model database with ArangoSearch and vector search for documents and graphs.
- **[TigerGraph](https://www.tigergraph.com/)** `Official` — Native parallel graph database with TigerVector hybrid graph+vector search.
- **[Memgraph](https://memgraph.com/)** `Official` — In-memory graph database with native vector search and graph traversal.
- **[Kùzu](https://kuzudb.com/)** `Official` — Embedded property graph database with built-in vector and full-text search.
- **[FalkorDB](https://www.falkordb.com/)** `Official` — Low-latency graph database with vector support for RAG.
- **[Amazon Neptune](https://aws.amazon.com/neptune/)** `Official` — Managed graph database with vector search and Neptune Analytics.

---

## Time-Series + Vector

Databases that combine time-series/analytics workloads with vector search, often via SQL extensions.

- **[TimescaleDB](https://www.timescale.com/)** `Official` — Time-series PostgreSQL extension with pgvector and pgvectorscale for time-aware hybrid search.
- **[ClickHouse](https://clickhouse.com/)** `Official` — Real-time OLAP database with vector distance functions and ANN indexing.
- **[DuckDB](https://duckdb.org/)** `Official` — In-process analytical database with array distance functions and vector-search extensions.
- **[StarRocks](https://www.starrocks.io/)** `Official` — Fast OLAP engine with native HNSW/IVFPQ vector indexes and hybrid queries.
- **[Apache Doris](https://doris.apache.org/)** `Official` — Real-time OLAP data warehouse with vector index support for high-dimensional data.

---

## Vector Search Libraries

Low-level libraries and algorithms for building approximate nearest-neighbor indexes.

- **[FAISS](https://github.com/facebookresearch/faiss)** `Official` — Comprehensive library for efficient similarity search and clustering of dense vectors.
- **[HNSWLib](https://github.com/nmslib/hnswlib)** `Community` — Fast HNSW graph-based nearest-neighbor library.
- **[Annoy](https://github.com/spotify/annoy)** `Official` — Approximate nearest-neighbor library optimized for memory-mapped indexes.
- **[ScaNN](https://github.com/google-research/google-research/tree/master/scann)** `Official` — Google's library for vector similarity search at scale.
- **[USearch](https://github.com/unum-cloud/usearch)** `Official` — Single-file similarity search library compatible with many index formats.
- **[NMSLIB](https://github.com/nmslib/nmslib)** `Community` — Similarity search library and toolkit with non-metric space support.
- **[DiskANN](https://github.com/microsoft/DiskANN)** `Official` — Disk-resident ANN index from Microsoft for billion-scale datasets.
- **[Vearch](https://github.com/vearch/vearch)** `Official` — Scalable vector search system built on Faiss for deep-learning retrieval.

---

## Hybrid Search

Search engines that combine keyword/BM25, filtering, and vector similarity in a single platform.

- **[Meilisearch](https://www.meilisearch.com/)** `Official` — Instant search engine with vector search, typo tolerance, and faceting.
- **[Typesense](https://typesense.org/)** `Official` — Open-source typo-tolerant search engine with vector and semantic search.
- **[Algolia](https://www.algolia.com/)** `Official` — Managed search platform with hybrid neural and keyword search.
- **[Manticore Search](https://manticoresearch.com/)** `Official` — Open-source search engine with SQL-like queries and vector search.
- **[Quickwit](https://quickwit.io/)** `Official` — Cloud-native search engine for logs and traces with vector search support.
- **[Apache Solr](https://solr.apache.org/)** `Official` — Open-source search platform with dense vector search via the DenseVector field type.

---

## Benchmarks

Tools and datasets for measuring vector database and embedding performance.

- **[VectorDBBench](https://github.com/zilliztech/VectorDBBench)** `Official` — Open-source benchmark tool for vector databases and cloud services.
- **[ANN-Benchmarks](https://github.com/erikbern/ann-benchmarks)** `Community` — Standardized benchmarking suite for approximate nearest-neighbor algorithms.
- **[Big-ANN Benchmarks](https://big-ann-benchmarks.com/)** `Official` — NeurIPS competition benchmark for billion-scale ANN search.
- **[BEIR](https://github.com/beir-cellar/beir)** `Community` — Heterogeneous benchmark for information retrieval with zero-shot evaluation.
- **[MTEB](https://huggingface.co/spaces/mteb/leaderboard)** `Community` — Massive Text Embedding Benchmark leaderboard for embedding models.
- **[VIBE](https://github.com/vector-index-bench/vibe)** `Community` — Vector Index Benchmark for Embeddings using modern embedding datasets.

---

## Related Awesome Lists

Discover complementary resources for building RAG, agent, and local-LLM systems.

- **[Awesome RAG](https://github.com/jasonwcfan/awesome-rag)** — Curated list of open-source tools for retrieval-augmented generation.
- **[Awesome MCP Servers](https://github.com/wong2/awesome-mcp-servers)** — Curated list of Model Context Protocol servers, including vector-store integrations.
- **[Awesome Local LLM](https://github.com/janhq/awesome-local-llm)** — Curated list of tools and models for running LLMs locally.

---

## Contributing

Read [CONTRIBUTING.md](./CONTRIBUTING.md) for the quality bar, entry format, and PR process.

---

## License

This list is released into the public domain under [CC0-1.0](./LICENSE).

## Want us to build this for you?

Enterprise AI Atlas is maintained by [Vibe Coding Agency](https://vibecodingagency.com). We prototype and ship agentic systems, MCP servers, and enterprise AI integrations for teams that need working software fast — without hiring a full AI engineering team.
