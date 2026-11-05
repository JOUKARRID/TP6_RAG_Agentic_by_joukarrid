# TP6 — RAG Agentique avec LangGraph & Ollama

Un système **Agentic RAG** (Retrieval-Augmented Generation) qui combine :
- un **vector store Chroma** avec embeddings locaux gratuits (HuggingFace),
- un **retriever** pour la recherche sémantique,
- un **agent LangGraph** capable de décider quand appeler l'outil de recherche,
- un **LLM local gratuit** via Ollama (`llama3.1:8b`).

Le projet illustre comment un agent peut orchestrer lui-même la récupération d'information à partir de documents PDF, puis générer une réponse fondée sur le contexte, sans dépendre d'une API payante.

---

## Sommaire

- [Architecture](#architecture)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Structure du projet](#structure-du-projet)
- [Utilisation](#utilisation)
- [Configuration](#configuration)
- [Détails techniques](#détails-techniques)
- [Limites connues](#limites-connues)
- [Améliorations possibles](#améliorations-possibles)
- [Licence](#licence)

---

## Architecture
