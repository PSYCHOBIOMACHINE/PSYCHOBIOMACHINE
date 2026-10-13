# Self-taught software developer · Full-stack · Cloud · AI engineering
Building RAG and AI-assisted applications in TypeScript

![JavaScript](https://img.shields.io/badge/-JavaScript-1a1a1a?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![TypeScript](https://img.shields.io/badge/-TypeScript-1a1a1a?style=for-the-badge&logo=typescript&logoColor=3178C6)
![React](https://img.shields.io/badge/-React-1a1a1a?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/-Next.js-1a1a1a?style=for-the-badge&logo=nextdotjs&logoColor=FFFFFF)
![React Native](https://img.shields.io/badge/-React%20Native-1a1a1a?style=for-the-badge&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/-Expo-1a1a1a?style=for-the-badge&logo=expo&logoColor=FFFFFF)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-1a1a1a?style=for-the-badge&logo=postgresql&logoColor=4169E1)
![Supabase](https://img.shields.io/badge/-Supabase-1a1a1a?style=for-the-badge&logo=supabase&logoColor=3ECF8E)
![Docker](https://img.shields.io/badge/-Docker-1a1a1a?style=for-the-badge&logo=docker&logoColor=2496ED)
![n8n](https://img.shields.io/badge/-n8n-1a1a1a?style=for-the-badge&logo=n8n&logoColor=EA4B71)
![Python](https://img.shields.io/badge/-Python-1a1a1a?style=for-the-badge&logo=python&logoColor=FFD43B)


## About me
I’m two years into full-stack development, currently building applications around retrieval and inference while adding containerization and cloud networking to my toolkit. I’m also fascinated by LLMs' parallels with human cognition, and I want to learn work on these models directly.

## What I'm Working On

### 1. **Obsidian-RAG Starter → 3D Modeling Starter**
**Stack: Typescript, Next.js, Zustand, Supabase/PostgreSQL + pgvector, inference and embedding APIs**    
- This project tarted as a RAG app for my vault of neurobiology papers. I created a Substack series to document my learning process. There, I discuss RAG concepts such as vector embeddings, tokenization, chunking, etc., while tying in parallels between LLM inference and human semantic memory retrieval. **(https://psychobiomachine.substack.com/)**
- It needed a working memory system that went beyond passing the entire session history with every prompt → So I created a `WorkingMemory` class to retain memory for different categories (user info, goals, topics). The class contains methods for updating this memory in ways that parallel human working memory. These methods make it so that the arrays containing topics and goals are organized by recency. I also used a Zustand store to initiate the `WorkingMemory` object on first render, persist it in local storage, and call the object methods on every turn.
- Next: I realized I was creating a primitive narrow version of MCP, and that I can repurpose the working memory approach to conduct UI manipulation, such as rendering 3D models to support answers to a user query. A background LLM process can return JSON params that feed (awaiting) object methods. Then, those methods could pull elements from a component library and render them in the UI. So while I continue to work on this RAG app, I will also be orienting some effort toward a child app that models neurocognitive architectures.

**(https://github.com/PSYCHOBIOMACHINE/Obsidian-RAG-Starter)**

### 2. Learning: Containerization and Networking
**Stack: Docker, n8n, Discord**

- This pursuit comes from my interest in understanding how full-stack applications live in the general internet space, and how architectures change when it comes time to scale.
- The repot contains a local n8n workspace set up in a Docker Compose. It contains one Docker network, with one container running n8n and another running PostgreSQL. The database isn’t published to the host so only n8n is reachable from the outside. This workspace contains sample automations for scraping RSS feeds for new information, and for obtaining financial data for an AI stocks watchlist. These automations relay their formatted output to a Discord server.
- Where it’s going: I’m learning to containerize applications and host them on my own VPS, starting with private access over SSH or Tailscale.

**(https://github.com/PSYCHOBIOMACHINE/n8n_demos)**

# 🌌 🐉 💎💎💎



<!--
**PSYCHOBIOMACHINE/PSYCHOBIOMACHINE** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ... 
-->
