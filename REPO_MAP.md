# Detran-RJ — REPO_MAP

Atualizado: 2026-07-03 (regenerado a partir do estado real da organização via `gh repo list`)

## Repositórios ativos

| Repo | Visib. | Papel |
|---|---|---|
| [.github](https://github.com/Detran-RJ/.github) | público | Perfil público, templates, segurança, skills e configuração organizacional |
| [detran-rj-portal](https://github.com/Detran-RJ/detran-rj-portal) | privado | **Monorepo canônico** — portal único com SSO centralizado (Guardian) + agregador de apps; microserviços PAT, Guardian, Wiki, Academy, Task |
| [detran-rj-tarefas](https://github.com/Detran-RJ/detran-rj-tarefas) | privado | Task — Kanban de tarefas e projetos; em absorção pelo `detran-rj-portal` (migração strangler) |
| [detran-rj-academia-dtic](https://github.com/Detran-RJ/detran-rj-academia-dtic) | privado | Detran Academy — capacitação interna gamificada da DTIC; em absorção pelo `detran-rj-portal` |
| [detran-rj-identidade-permissoes](https://github.com/Detran-RJ/detran-rj-identidade-permissoes) | privado | Gestão de segurança da informação — permissões, acessos, VPNs e senhas críticas; em absorção pelo `detran-rj-portal` |
| [sistema-patrimonio](https://github.com/Detran-RJ/sistema-patrimonio) | privado | Sistema de Gestão Patrimonial (v17, export Manus) — React 19 + tRPC 11 + Drizzle; **em transição** — será arquivado após portar os sprints para `Msc-Company-Org/detran-patrimonio` |
| [detran-rj-patrimonio-mcp](https://github.com/Detran-RJ/detran-rj-patrimonio-mcp) | privado | Servidor MCP read-only do patrimônio DIRTIC (ferramentas aterradas para agentes) |
| [documentacao-patrimonio](https://github.com/Detran-RJ/documentacao-patrimonio) | privado | Documentação do sistema de patrimônio DIRTIC (requisitos, atas) |
| [detran-rj-wiki](https://github.com/Detran-RJ/detran-rj-wiki) | privado | Base de conhecimento (fontes públicas) pronta para Wiki.js (storage Git) |
| [dirtic-dados-organizacionais](https://github.com/Detran-RJ/dirtic-dados-organizacionais) | privado | Dados organizacionais consolidados da DIRTIC (pessoas, empresas, contratos, órgãos) + seed do Guardian |
| [detran-rj-mcp](https://github.com/Detran-RJ/detran-rj-mcp) | privado | Servidor MCP do Detran-RJ, parte da família `msc-mcp-core` |

## Repositórios arquivados

| Repo | Visib. | Papel |
|---|---|---|
| [portal-detran](https://github.com/Detran-RJ/portal-detran) | privado | Antecessor do `detran-rj-portal` — infraestrutura, documentação e planejamento de features |
| [detran-rj-academia](https://github.com/Detran-RJ/detran-rj-academia) | privado | Educação formal (Vite + Drizzle + pnpm); arquivado em 2026-06, substituído por Academy (Msc-Company-Org) — snapshot histórico |
| [detran-rj-patrimonio-legado](https://github.com/Detran-RJ/detran-rj-patrimonio-legado) | privado | Pat-detran — sistema de patrimônio legado (React 19 + tRPC 11 + Drizzle/MariaDB + RAG Atlas) |
| [dashboard-patrimonio-dirtic](https://github.com/Detran-RJ/dashboard-patrimonio-dirtic) | privado | Dashboard de visualização dos dados patrimoniais consolidados da DIRTIC (export Manus) |

## Relação com outras organizações

Parte do trabalho relacionado ao Detran vive na organização `Msc-Company-Org` (repos `detran-patrimonio`, `detran-sei`, `detran-prd`), mantida pela mesma equipe. O `sistema-patrimonio` desta organização será arquivado quando a migração de sprints para `Msc-Company-Org/detran-patrimonio` for concluída.

## Estrutura deste repositório

```text
.github/
├─ profile/README.md        ← Perfil público da organização
├─ REPO_MAP.md              ← Este mapa
├─ CODEOWNERS               ← Donos de código da org
├─ SECURITY.md              ← Política de segurança
├─ CONTRIBUTING.md          ← Guia de contribuição
├─ CODE_OF_CONDUCT.md       ← Código de conduta
├─ ISSUE_TEMPLATE/          ← Templates de issue (bug, feature)
├─ PULL_REQUEST_TEMPLATE.md ← Template de PR
└─ docs/                    ← Credenciais (política), config da org, skills
```

## Política de deploy

| Plataforma | Padrão |
|---|---|
| GitHub | privado por padrão; PR com issue |
| Vercel | protegido por padrão; público só com dados sintéticos/aprovados |
| Hugging Face | Space privado por padrão; datasets públicos só sintéticos |
| Cloudflare Pages | usar apenas para conteúdo revisado e sem dados reais |

## Referências

- [`docs/credenciais.md`](./docs/credenciais.md)
- [`docs/config/organizacao.md`](./docs/config/organizacao.md)
- [`docs/skills/`](./docs/skills/)
