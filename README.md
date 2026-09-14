# <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Netflix_2015_logo.svg" width="30" height="30" valign="middle"> LLM-Driven Knowledge Graphs: Comparative Analysis & Query Benchmarking

An academic research repository evaluating Generative AI models (Gemini, Perplexity, and ChatGPT) across ontology engineering, Knowledge Graph construction, Neo4j graph implementation, structured vs. natural language querying, and Wikidata SPARQL benchmarking within the domain of streaming media and traditional outlets.

![](https://img.shields.io/badge/Neo4j-Graph_Database-008CC1?style=flat&logo=neo4j&logoColor=white)
![](https://img.shields.io/badge/Semantic_Web-RDF_%2F_OWL-2e8540?style=flat)
![](https://img.shields.io/badge/Wikidata-SPARQL-11557c?style=flat&logo=wikidata&logoColor=white)
![](https://img.shields.io/badge/Project-Completed-44cc11?style=flat)

---

## 📌 Project Overview

This project explores the capabilities and limitations of Large Language Models in automated ontology engineering and Knowledge Graph (KG) construction. Using the domain of global streaming platforms versus traditional media as a testbed, the study investigates how different LLMs handle structural taxonomic constraints, how structured database retrieval (**Neo4j Cypher**) compares to natural language AI outputs, and how closed-world graph models contrast with open-world public data ecosystems (**Wikidata SPARQL**).

---

## 📁 Repository Structure

```text
streaming-media-knowledge-graph-llm/
│── README.md                        # Detailed Repository Architecture & Research Findings
│── /ontologies                      # Semantic Web Representations (.ttl files)
│   ├── Gemini_KG.ttl                # Gemini Baseline Ontology & Triples
│   ├── Perplexity_KG.ttl            # Perplexity Fine-Tuned Ontology & Triples
│   └── ChatGPT_KG.ttl               # ChatGPT Expanded Ontology & Triples
│── /cypher-queries                  # Neo4j Database Implementation & Queries
│   ├── cypher_queries_and_results.md# Executed Cypher Scripts and Database Outputs
│   └── ai_free_text_responses.md    # Comparative Natural Language AI Prompt Responses
│── /wikidata-queries                # Open-World Benchmarking
│   └── sparql_queries_wikidata.md   # Wikidata SPARQL Code, Links, and Execution Tables
└── /images                          # High-Resolution Neo4j Visualizations
    ├── Gemini_KG.png                # Gemini Knowledge Graph Topology
    ├── Perplexity_KG.png            # Perplexity Knowledge Graph Topology
    └── ChatGPT_KG.png               # ChatGPT Knowledge Graph Topology

```

---

## 🧬 Ontological Architecture & Tool Comparison

The project evaluates three distinct GenAI architectures built from a standardized initial prompt enforcing strict ontological criteria: a 3-level IS-A class hierarchy, at least 20 classes/sub-classes, 20 Data Properties, 20 Object Properties, 20 specific instances, and 20 Knowledge Graph triples.

* **Gemini (Model 1):** Maintained precise single-turn adherence to all numeric and taxonomic constraints without scope creep, producing a balanced, ready-to-implement baseline graph containing 23 classes across 5 core branches.


* **Perplexity / Sonar 2 (Model 2):** Highlighted the necessity of iterative prompt engineering. Its initial generation suffered from a *Predicate Redundancy Error* (repeatedly reusing `platformDistributesContent`), which was successfully resolved using targeted negative constraints (*"do not repeat any object property"*).


* **ChatGPT (Model 3):** Generated an expansive, research-grade knowledge graph exceeding 70 classes with advanced OWL constraints, though it exhibited *over-generation* beyond the immediate project scope.



---

## 🔍 Query Retrieval: Structured Cypher vs. AI Free-Text

To evaluate retrieval paradigms, multi-hop competency questions regarding content-driven conflicts, geopolitical regulations, and socio-behavioral impacts were executed across two channels:

1. **Structured Neo4j Queries (Cypher):** Provided deterministic precision, auditable truth, and mathematical certainty over explicit graph topologies (though vulnerable to schema rigidity).


2. **Free-Text AI Prompts:** Offered semantic flexibility and contextual synthesis, though prone to drifting from strict graph boundaries when relationships were unmodeled.



---

## 🌍 Wikidata SPARQL Benchmarking

Closed-world findings were benchmarked against the open-world Wikidata ecosystem via the Wikidata Query Service across three axes:

* **Cultural Distribution:** Contrasting corporate distribution and soft power in Neo4j against objective bibliographic metadata (country of origin, language) in Wikidata.


* **Institutional Governance:** Contrasting active regulatory friction in closed graphs with formal legislative acts (AVMSD 2010, GDPR) in static legal ontologies.


* **Behavioral Impact:** Contrasting causal algorithmic consequences mapped to demographic cohorts in Neo4j against disconnected medical and sociological taxonomies in Wikidata.



---

## 📊 Visualizations Highlights

| Gemini Knowledge Graph | Perplexity Knowledge Graph | ChatGPT Knowledge Graph |
| --- | --- | --- |
|  |  |  |
| *20 nodes, 20 relationships (Censorship & Behavioral Focus).*<br> | *22 nodes, 20 relationships (Algorithmic & Policy Focus).*<br> | *21 core nodes, 19 key relationships (Soft Power & Global Scope).* |

---

## 🛠️ Tech Stack & Dependencies

* **Graph Database:** Neo4j (Cypher Query Language)


* **Semantic Web:** RDF, OWL, Turtle (`.ttl`)


* **GenAI Frameworks:** Gemini, Perplexity, ChatGPT (Prompt engineering & iterative feedback workflows)


* **Data Ecosystems:** Wikidata SPARQL Query Service



---

## 👤 Author

**Kerem Bar**

*Master's Student in Information Sciences (Information Technology Specialization)*

```

```
