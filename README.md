# AI-Powered Security Knowledge Base

A local-first Obsidian vault for organizing security certification study, hands-on lab work, and technical reference material — with an integrated offline AI assistant powered by Ollama.

This repo contains a sanitized subset of my personal vault: the structure, templates, and example notes, minus anything tied to active certification exams or private project details.

## Why I Built This

I wanted a single, searchable home for everything I learn while working toward Network+, Security+, and hands-on platforms like TryHackMe — one that doesn't depend on an internet connection or a subscription to stay useful. The result is a knowledge base that grows with each cert and lab, cross-links related concepts automatically, and lets me query my own notes using a local LLM instead of digging through folders.

## Screenshots

![Vault graph view](./images/vault-graph.png)
![Ollama chat against the vault](./images/vault-chat.png)
![Vault dashboard](./images/vault-dashboard.png)

## Stack

- **[Obsidian](https://obsidian.md/)** — note-taking and linking engine
- **[Ollama](https://ollama.com/)** — local LLM runtime, fully offline
  - `llama3.1:latest` — general-purpose reasoning and Q&A over notes
  - `mistral:latest` — alternate model for comparison/fallback
  - `qwen2.5:0.5b` — lightweight model for fast, low-resource queries
  - `nomic-embed-text:latest` — embeddings for semantic search across the vault
- **Dataview** *(if applicable)* — auto-generated tables/queries across notes
- **Markdown** — all notes, templates, and reference material

## What This Demonstrates

- **Security domain knowledge** — structured documentation across Network+, Security+, and TryHackMe rooms, including methodology, tools, and takeaways per lab
- **Local AI integration** — wiring a local LLM (via Ollama) into a real, daily-use workflow, including embeddings-based semantic search
- **Systems thinking** — organizing sprawling technical material into a navigable, cross-linked structure rather than flat notes
- **Self-directed tooling** — building and maintaining infrastructure (templates, automation, model selection) to support ongoing learning

## Structure

```
vault/
├── security-plus/       # Security+ study notes
├── network-plus/        # Network+ study notes (completed)
├── tryhackme/            # Room-by-room notes: methodology, tools, takeaways
├── tools-reference/      # Fast reference by tool: syntax, common flags, use cases
├── projects/             # Personal project brainstorming and completed builds
└── templates/            # Note templates used across the vault
```

## Status

Core setup (Obsidian + Ollama integration) is working. Actively importing and organizing existing Network+ and Security+ notes into the structure above.

## About Me

I'm E'Van Powers, an IT Support Technician working toward a career in cybersecurity/network security. I hold CompTIA Network+ and PC Pro certifications, and I'm currently pursuing AWS Cloud Practitioner, CompTIA Security+, and a Cloud Computing Certificate at Lee College.

- LinkedIn: [linkedin.com/in/e-van-powers-57a616b2](https://www.linkedin.com/in/e-van-powers-57a616b2)
- Portfolio: [evpowe07825.github.io/e-van-powers-portfolio](https://evpowe07825.github.io/e-van-powers-portfolio/)
