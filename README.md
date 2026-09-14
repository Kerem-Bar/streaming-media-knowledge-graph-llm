# <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Netflix_2015_logo.svg" width="30" height="30" valign="middle"> LLM-Driven Knowledge Graphs: Comparative Analysis & Query Benchmarking

An academic research repository evaluating Generative AI models (Gemini, Perplexity, and ChatGPT) across ontology engineering, Knowledge Graph construction, Neo4j implementation, structured graph queries versus AI free-text responses, and Wikidata SPARQL benchmarking within the domain of streaming media and traditional outlets.

![](https://img.shields.io/badge/Neo4j-Graph_Database-008CC1?style=flat&logo=neo4j&logoColor=white)
![](https://img.shields.io/badge/Semantic_Web-RDF_%2F_OWL-2e8540?style=flat)
![](https://img.shields.io/badge/Wikidata-SPARQL-11557c?style=flat&logo=wikidata&logoColor=white)
![](https://img.shields.io/badge/Project-Completed-44cc11?style=flat)

---

## 📌 Project Overview

This project explores the capabilities and limitations of Large Language Models in automated ontology engineering and Knowledge Graph (KG) construction. Using the domain of global streaming platforms versus traditional media as a testbed, the study investigates how different LLMs handle structural taxonomic constraints, how structured database queries (**Neo4j Cypher**) compare to natural language AI responses, and how closed-world graph models contrast with open-world public data ecosystems (**Wikidata SPARQL**). 

The complete project documentation and implementation details are divided into the main academic research report and accompanying appendices.

---

## 📁 Repository Structure

```text
streaming-media-knowledge-graph-llm/
│── README.md                        # Detailed Repository Architecture & Research Findings
│── /ontologies                      # Semantic Web Representations (.ttl files)
│   ├── Gemini_KG.ttl                # Gemini Baseline Ontology & Triples (Appendix A)[cite: 1]
│   ├── Perplexity_KG.ttl            # Perplexity Fine-Tuned Ontology & Triples (Appendix B)[cite: 1]
│   └── ChatGPT_KG.ttl               # ChatGPT Expanded Ontology & Triples (Appendix C)[cite: 1]
│── /documentation                   # Core Project Files
│   ├── Knowledge Graph Final Project.pdf # Main academic research report (Parts 1-4)
│   └── Appendices.pdf               # Comprehensive appendices (Models, Cypher, AI Free-Text, SPARQL)[cite: 1]
│── Gemini_KG.png                    # Gemini Knowledge Graph Topology (Figure 3.1)
│── Perplexity_KG.png                # Perplexity Knowledge Graph Topology (Figure 3.2)
└── ChatGPT_KG.png                   # ChatGPT Knowledge Graph Topology (Figure 3.3)[cite: 2]

```

---

## 🧬 Ontological Architecture & Tool Comparison

As documented in **Part 1 and Part 2** of `Knowledge Graph Final Project.pdf`, the study evaluates three distinct GenAI architectures built from a standardized initial prompt enforcing strict ontological criteria: a 3-level IS-A class hierarchy, at least 20 classes/sub-classes, 20 Data Properties, 20 Object Properties, 20 specific instances, and 20 Knowledge Graph triples.

* **Gemini (Model 1):** Maintained precise single-turn adherence to all numeric and taxonomic constraints without scope creep, producing a balanced, ready-to-implement baseline graph containing 23 classes across 5 core branches.


* **Perplexity / Sonar 2 (Model 2):** Highlighted the necessity of iterative prompt engineering. Its initial generation suffered from a *Predicate Redundancy Error* (repeatedly reusing `platformDistributesContent`), which was successfully resolved using targeted negative constraints (*"do not repeat any object property"*).


* **ChatGPT (Model 3):** Generated an expansive, research-grade knowledge graph exceeding 70 classes with advanced OWL constraints, though it exhibited *over-generation* beyond the immediate project scope.



---

## 🔍 Query Retrieval: Structured Cypher vs. AI Free-Text

As detailed in **Part 3** of `Knowledge Graph Final Project.pdf` and demonstrated in **Appendices D & E** of `Appendices.pdf`, multi-hop competency questions regarding content-driven conflicts, geopolitical regulations, and socio-behavioral impacts were evaluated across two parallel channels:

1. **Structured Neo4j Queries (Cypher):** Provided deterministic precision, auditable truth, and mathematical certainty over explicit graph topologies (though vulnerable to schema rigidity and join path mismatches).


2. **Free-Text AI Prompts:** Offered semantic flexibility and contextual synthesis, though prone to drifting from strict graph boundaries when relationships were unmodeled.



---

## 🌍 Wikidata SPARQL Benchmarking

As explored in **Part 4** of `Knowledge Graph Final Project.pdf` and **Appendix F** of `Appendices.pdf`, closed-world findings were benchmarked against the open-world Wikidata ecosystem via the Wikidata Query Service across three core axes:

* **Cultural Distribution:** Contrasting corporate distribution and soft power in Neo4j against objective bibliographic metadata (country of origin, language) in Wikidata.


* **Institutional Governance:** Contrasting active regulatory friction in closed graphs with formal legislative acts (AVMSD 2010, GDPR) in static legal ontologies.


* **Behavioral Impact:** Contrasting causal algorithmic consequences mapped to demographic cohorts in Neo4j against disconnected medical and sociological taxonomies in Wikidata.



---

## 📊 Visualizations Highlights

| Gemini Knowledge Graph (Fig 3.1) | Perplexity Knowledge Graph (Fig 3.2) | ChatGPT Knowledge Graph (Fig 3.3) |
| :---: | :---: | :---: |
| <img src="Gemini_KG.png" width="350"> | <img src="Perplexity_KG.png" width="350"> | <img src="ChatGPT_KG.png" width="350"> |
| *20 nodes, 20 relationships (Censorship & Behavioral Focus).* | *22 nodes, 20 relationships (Algorithmic & Policy Focus).* | *21 core nodes, 19 key relationships (Soft Power & Global Scope).* |

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
