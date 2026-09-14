# LLM-Driven Knowledge Graphs: Comparative Analysis & Query Benchmarking

## Overview
This repository contains the final academic project focused on ontology engineering, Knowledge Graph (KG) construction, and comparative evaluation of Generative AI models (**Gemini, Perplexity/Sonar 2, and ChatGPT**). The project evaluates how different LLMs handle structural constraints (hierarchies, data/object properties, and instances), how structured database retrieval (**Neo4j Cypher**) compares to natural language AI outputs, and how closed-world graphs contrast with open-world public data ecosystems (**Wikidata SPARQL**).

## Repository Structure
- **`/ontologies`**: Contains the semantic web representations (`.ttl` / RDF/OWL files) generated and refined across the LLM models.
- **`/cypher-queries`**: Includes graph creation scripts, analytical Neo4j Cypher queries, and comparative **Free-Text AI responses** (evaluating precision, determinism, and semantic generalization).
- **`/wikidata-queries`**: Contains SPARQL code and execution links benchmarking closed-world model findings against the Wikidata ecosystem.
- **`/images`**: High-resolution visualizations of the knowledge graphs exported directly from Neo4j.

## Methodology & Stages
1. **Stage 1 - Ontology & KG Generation**: Constructing multi-level IS-A taxonomies, data/object properties, and instance triples using GenAI with iterative prompt engineering (e.g., resolving *Predicate Redundancy* errors).
2. **Stage 2 - Neo4j Implementation & Querying vs. AI Free-Text**: Translating semantic models into Neo4j graph databases, executing multi-hop Cypher queries, and contrasting deterministic results with direct AI text prompts.
3. **Stage 3 - Wikidata Alignment (SPARQL)**: Benchmarking structured graph outputs against open-world public data via the Wikidata Query Service to analyze structural and institutional differences.

## Tech Stack
- **Graph Database**: Neo4j (Cypher Query Language)
- **Semantic Web**: RDF, OWL, Turtle (`.ttl`)
- **GenAI Frameworks**: Gemini, Perplexity, ChatGPT (Prompt engineering & iterative feedback workflows)
- **Data Ecosystems**: Wikidata SPARQL Query Service