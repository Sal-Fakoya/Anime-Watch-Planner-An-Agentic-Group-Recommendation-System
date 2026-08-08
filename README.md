# Anime-Watch-Planner-An-Agentic-Group-Recommendation-System
An agentic recommendation system for group anime watch-planning, built end-to-end on Databricks

[Demo video](https://youtu.be/M_iWYy627MQ) — the app requires Databricks workspace login, so a walkthrough video is linked here instead of a live link

An agentic recommendation system for group anime watch-planning, built end-to-end on Databricks: a Spark pipeline ingests and cleans data from the AniList API into a Postgres-backed Lakebase store, a Vector Search index enables semantic retrieval over synopses and tags, and a LinUCB contextual bandit re-ranks recommendations from a group's accumulated ratings. A LangGraph agent with five tools (semantic search, structured filtering, comparison, watchlist management, and rating logging) handles multi-turn conversations with persistent memory, deployed as a Databricks App with a chat interface. Debugged and resolved a full production deployment chain, including service-principal authentication for Vector Search, Lakebase secret management, and schema migrations for a live, evolving dataset.


