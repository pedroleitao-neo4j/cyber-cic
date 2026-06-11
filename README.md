# A Network Graph Analysis of the CIC-UNSW-NB15 Dataset using Neo4j and Graph Data Science (GDS)

This notebook demonstrates possible applications in network security analysis using Neo4j and its Graph Data Science (GDS) library. It uses the [CIC-UNSW-NB15](https://www.unb.ca/cic/datasets/cic-unsw-nb15.html) dataset, which contains a rich set of network flow records labeled with various attack types and normal traffic. The dataset is ideal for exploring how graph-based techniques can enhance our understanding of network behavior and improve threat detection.

This presents typical patterns and techniques for analyzing network flow data, suitable for identifying anomalies, understanding communication patterns, and extracting insights from network traffic data captured by network monitoring tools such as [Zeek](https://zeek.org/), [Suricata](https://suricata.io/), [Argus](https://qosient.com/argus/), or [Wireshark](https://www.wireshark.org/).

## Key objectives

Amongst others, in this notebook, we will execute a complete Graph Data Science workflow tailored for security analysts to:

- Understand how networks and network traffic can be represented as graphs, and the types of insights that can be derived from such representations.
- Graph Modeling: Map the raw tabular data of the CIC-UNSW-NB15 dataset into a highly optimized graph schema.
- In-Memory Projections: Create high-performance graph projections suitable for cloud-ephemeral managed environments (like Neo4j AuraDS).
- Representation Learning (FastRP): Generate low-dimensional, topology-aware node embeddings that capture the unique structural footprint of every host.
- Behavioral Similarity (KNN & Cosine Similarity): Identify hidden, look-alike malicious actors by streaming similarity metrics against known indicators of compromise (IoCs).
- Sub-graph Visualization: Extract and render structural paths (CONNECTED_TO, IN_SUBNET) to visually compare the blast radiuses of suspicious network nodes.