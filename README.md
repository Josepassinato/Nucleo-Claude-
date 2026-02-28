# ExecutiveOS — CEO → CTO Agent

Sistema de delegação estratégica onde o CEO delega ao CTO Agent com autonomia técnica total.

## Features

- **CEO Command Center** — CEO define visão em linguagem natural
- **CTO Agent Analysis** — Análise técnica via Claude AI (arquitetura, integrações, riscos, MVP)
- **Code Generation Engine** — Geração automática de código, schema, migrations e Docker
- **Execution Pipeline** — Deploy com 5 stages em tempo real (scaffold → schema → codegen → tests → deploy)
- **Git & Rollback System** — Histórico de commits com rollback não-destrutivo

## Tech Stack

- React 18 + Vite
- Tailwind CSS
- Anthropic Claude API (`claude-sonnet-4-20250514`)

## Setup

```bash
npm install
npm run dev
```

## Deploy (Vercel)

```bash
npm run build
# ou conecte o repositório direto na Vercel
```

## Variáveis de Ambiente

Nenhuma necessária — a chave da API Anthropic é injetada via proxy do claude.ai.

## Estrutura

```
src/
  App.jsx      # Componente principal (CEO/CTO system)
  main.jsx     # Entry point React
  index.css    # Tailwind + estilos globais
index.html     # HTML entry
vite.config.js
tailwind.config.js
```
