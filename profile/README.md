<!--
  README institucional da organização Detran-RJ no GitHub.
  Renderizado automaticamente em github.com/Detran-RJ
-->

<div align="center">

# DTIC — Departamento de Tecnologia da Informação e Comunicação

![Detran-RJ](https://img.shields.io/badge/DETRAN--RJ-005D9F?style=for-the-badge&logoColor=white)
![DTIC](https://img.shields.io/badge/DTIC-298098?style=for-the-badge&logoColor=white)
![Gov.br](https://img.shields.io/badge/Gov.RJ-02BF4F?style=for-the-badge&logoColor=white)

**Tecnologia pública, transparente e a serviço do cidadão fluminense.**

[Site oficial](https://www.detran.rj.gov.br) · [Serviços](https://www.detran.rj.gov.br/_servico/) · [Ouvidoria](https://www.detran.rj.gov.br/_inst/ouvidoria/)

</div>

---

## Quem somos

A **DTIC/Detran-RJ** é a unidade responsável pela estratégia, desenvolvimento e operação dos sistemas de TI que sustentam os serviços do Detran-RJ, atendendo **4.000+ servidores** e milhões de cidadãos fluminenses.

---

## Mapa de Sistemas

```
┌─────────────────────────────────────────────────────────────────────────┐
│                        DTIC / DETRAN-RJ                                  │
├───────────────────┬─────────────────────┬───────────────────────────────┤
│  🏢 PATRIMÔNIO    │  📋 SEI / CONTRATOS │  🤖 AI / KNOWLEDGE           │
│                   │                     │                               │
│  patrimonio-web   │  contratos-app      │  detran-ai (Prometheus+Atlas) │
│  patrimonio-api   │  servagc            │  wiki-app + wiki-vault        │
│  detran-pat       │  sei-pipeline       │  chatbot-detran-rj            │
│                   │  sei-dirtic/divit   │  atlas-detran-rag             │
├───────────────────┼─────────────────────┼───────────────────────────────┤
│  🎓 CAPACITAÇÃO   │  ⚙️ INFRA / CI      │  📐 GOVERNANÇA               │
│                   │                     │                               │
│  detran-academy   │  ci-workflows       │  governanca-docs              │
│  assistente-sei   │  dev-environment    │  identidade-visual            │
│                   │  .github            │                               │
└───────────────────┴─────────────────────┴───────────────────────────────┘
```

---

## Projetos Ativos

### 🤖 Inteligência Artificial

| Projeto | Descrição | Stack |
|---------|-----------|-------|
| [**detran-ai**](https://github.com/Detran-RJ/detran-ai) | Agentes Prometheus (SEI) e Atlas (Patrimônio) — processamento inteligente de documentos | Python · LangGraph · FastAPI · Qdrant |
| [**detran-wiki-app**](https://github.com/Detran-RJ/detran-wiki-app) | Busca semântica + chat sobre legislação e serviços do Detran-RJ | React · Node · ChromaDB |
| [**chatbot-detran-rj**](https://github.com/Detran-RJ/chatbot-detran-rj) | Chatbot humanizado com RAG para atendimento | Python · LangGraph · LoRA |
| [**atlas-detran-rag**](https://github.com/Detran-RJ/atlas-detran-rag) | Pipeline RAG para base de conhecimento institucional | Python · LangGraph |

### 🏢 Sistemas de Gestão

| Projeto | Descrição | Stack |
|---------|-----------|-------|
| [**detran-patrimonio-web**](https://github.com/Detran-RJ/detran-patrimonio-web) | Sistema de Patrimônio DPAT — RBAC, OCR, levantamento multi-modal | React 19 · tRPC · Drizzle · MySQL |
| [**detran-patrimonio-api**](https://github.com/Detran-RJ/detran-patrimonio-api) | API REST do Sistema de Patrimônio | NestJS · Prisma · Docker |
| [**detran-contratos-app**](https://github.com/Detran-RJ/detran-contratos-app) | Gestão de contratos DTIC com integração SEI | React · tRPC · Drizzle · Tailwind |
| [**servagc**](https://github.com/Detran-RJ/servagc) | Pipeline central de documentação SEI | HTML · dados estruturados |

### 🎓 Capacitação

| Projeto | Descrição | Stack |
|---------|-----------|-------|
| [**detran-academy**](https://github.com/Detran-RJ/detran-academy) | LMS interno — vídeo-aulas e tutor IA para servidores | pnpm · Turbo · Supabase |
| [**assistente-sei**](https://github.com/Detran-RJ/assistente-sei) | Análise assistida de processos SEI | Python · Streamlit |

### ⚙️ Infraestrutura

| Projeto | Descrição | Stack |
|---------|-----------|-------|
| [**detran-ci-workflows**](https://github.com/Detran-RJ/detran-ci-workflows) | Workflows GitHub Actions reutilizáveis (node, python, php, codeql, deploy) | YAML |
| [**detran-governanca-docs**](https://github.com/Detran-RJ/detran-governanca-docs) | Governança, auditorias, runbooks e infra da org | Markdown · Shell |
| [**wiki-detran-rj**](https://github.com/Detran-RJ/wiki-detran-rj) | Base de conhecimento — 165 notas, 18 MOCs | Obsidian (Markdown) |

---

## Convenções

| Item | Padrão |
|------|--------|
| Naming | `detran-<domínio>-<tipo>` |
| Commits | [Conventional Commits](https://www.conventionalcommits.org/) em português |
| Branches | `main`, `feat/*`, `fix/*`, `docs/*` |
| CI | Workflows reutilizáveis em [`detran-ci-workflows`](https://github.com/Detran-RJ/detran-ci-workflows) |
| Deploy | GitHub Actions → SSH → VPS (Docker Compose) |

---

## Stack Tecnológica

```
Frontend:   React · TypeScript · Tailwind CSS · Vite
Backend:    FastAPI · NestJS · tRPC · Node.js
AI/ML:      LangGraph · LangChain · Qdrant · ChromaDB
Database:   PostgreSQL · MySQL · SQLite · Supabase
Infra:      Docker · GitHub Actions · Caddy · VPS
```

---

<div align="center">

**🏛️ Governo do Estado do Rio de Janeiro**

*Desenvolvido pela DTIC/Detran-RJ*

</div>
