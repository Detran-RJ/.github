<!-- README institucional da organização Detran-RJ no GitHub -->

<div align="center">

# DTIC — Detran-RJ

![Detran-RJ](https://img.shields.io/badge/DETRAN--RJ-005D9F?style=for-the-badge&logoColor=white)
![DTIC](https://img.shields.io/badge/DTIC-298098?style=for-the-badge&logoColor=white)
![Gov.RJ](https://img.shields.io/badge/Gov.RJ-02BF4F?style=for-the-badge&logoColor=white)
![Privado por padrão](https://img.shields.io/badge/Privado%20por%20padr%C3%A3o-Seguran%C3%A7a-red?style=for-the-badge)

**Tecnologia pública, governança, segurança e automação a serviço do cidadão fluminense.**

[Site oficial](https://www.detran.rj.gov.br) · [Serviços](https://www.detran.rj.gov.br/_servico/) · [Ouvidoria](https://www.detran.rj.gov.br/_inst/ouvidoria/)

</div>

---

## Objetivo

A organização `Detran-RJ` centraliza projetos, documentação e automações relacionados à DTIC/Detran-RJ, com foco em:

- governança e rastreabilidade;
- segurança e LGPD;
- automação de processos internos;
- IA institucional privada;
- documentação técnica e operacional.

Os repositórios da organização são **privados por padrão** — este perfil e os templates organizacionais são a única parte pública.

## Projetos ativos

O repositório canônico da organização é o [`detran-rj-portal`](https://github.com/Detran-RJ/detran-rj-portal): portal único com SSO centralizado (Guardian) e agregador de apps, organizado como monorepo de microserviços. Os apps internos independentes estão sendo absorvidos por ele em uma migração gradual (padrão strangler).

| Domínio | Projeto | Descrição |
|---|---|---|
| Portal | [`detran-rj-portal`](https://github.com/Detran-RJ/detran-rj-portal) | Portal único — SSO centralizado (Guardian) + agregador de apps; monorepo de microserviços (PAT, Guardian, Wiki, Academy, Task) |
| Tarefas | [`detran-rj-tarefas`](https://github.com/Detran-RJ/detran-rj-tarefas) | Task — Kanban de controle de tarefas e projetos (em absorção pelo portal) |
| Capacitação | [`detran-rj-academia-dtic`](https://github.com/Detran-RJ/detran-rj-academia-dtic) | Detran Academy — plataforma de capacitação interna da DTIC (em absorção pelo portal) |
| Segurança | [`detran-rj-identidade-permissoes`](https://github.com/Detran-RJ/detran-rj-identidade-permissoes) | Gestão de segurança da informação — permissões, acessos, VPNs e senhas críticas (em absorção pelo portal) |
| Patrimônio | [`sistema-patrimonio`](https://github.com/Detran-RJ/sistema-patrimonio) | Sistema de Gestão Patrimonial — React 19 + tRPC 11 + Drizzle (em transição; será arquivado após a migração dos sprints) |
| Patrimônio | [`detran-rj-patrimonio-mcp`](https://github.com/Detran-RJ/detran-rj-patrimonio-mcp) | Servidor MCP read-only do patrimônio DIRTIC (ferramentas aterradas para agentes) |
| Patrimônio | [`documentacao-patrimonio`](https://github.com/Detran-RJ/documentacao-patrimonio) | Documentação do sistema de patrimônio (requisitos, atas) |
| Conhecimento | [`detran-rj-wiki`](https://github.com/Detran-RJ/detran-rj-wiki) | Base de conhecimento (fontes públicas) pronta para Wiki.js com storage Git |
| Dados | [`dirtic-dados-organizacionais`](https://github.com/Detran-RJ/dirtic-dados-organizacionais) | Dados organizacionais consolidados da DIRTIC + seed do Guardian |
| IA | [`detran-rj-mcp`](https://github.com/Detran-RJ/detran-rj-mcp) | Servidor MCP do Detran-RJ (família `msc-mcp-core`) |
| Organização | [`.github`](https://github.com/Detran-RJ/.github) | Perfil público, templates, segurança e configuração organizacional |

## Mapa operacional

```text
DTIC / DETRAN-RJ
├─ Portal único     → detran-rj-portal (canônico; absorve os apps abaixo)
│   ├─ Tarefas      → detran-rj-tarefas
│   ├─ Academy      → detran-rj-academia-dtic
│   └─ Guardian     → detran-rj-identidade-permissoes
├─ Patrimônio       → sistema-patrimonio + detran-rj-patrimonio-mcp + documentacao-patrimonio
├─ Conhecimento     → detran-rj-wiki
├─ Dados            → dirtic-dados-organizacionais
├─ IA / agentes     → detran-rj-mcp
└─ Governança       → .github
```

Mapa completo (incluindo arquivados): [`REPO_MAP.md`](../REPO_MAP.md)

## Repositórios arquivados

| Repo | Motivo |
|---|---|
| `portal-detran` | Antecessor do `detran-rj-portal` (infraestrutura, documentação e planejamento) |
| `detran-rj-academia` | Educação formal; substituído — mantido como snapshot histórico |
| `detran-rj-patrimonio-legado` | Pat-detran, sistema de patrimônio legado |
| `dashboard-patrimonio-dirtic` | Dashboard de visualização dos dados patrimoniais (export Manus) |

## Convenções

| Item | Padrão |
|---|---|
| Branch principal | `main` |
| Commits | Conventional Commits em português |
| Fluxo | issue → branch → PR → quality → merge |
| Segurança | Não abrir issue pública com vulnerabilidade |
| Dados sensíveis | Nunca publicar `.env`, PDFs internos, bases extraídas, dados pessoais ou credenciais |
| Hugging Face | Spaces privados por padrão; datasets públicos somente sintéticos/anônimos |
| Vercel/Cloudflare | Deploy protegido por padrão; público somente com dados sintéticos/aprovados |

## Credenciais e publicação

- Credenciais reais nunca devem ser colocadas em README, issue, PR, commit ou chat.
- Use GitHub Actions Secrets, Vercel Environment Variables, Hugging Face Space Secrets ou secret manager equivalente.
- Todo token exposto deve ser considerado comprometido e rotacionado.
- Conteúdo Detran é **privado por padrão**.

Consulte:

- [`SECURITY.md`](../SECURITY.md)
- [`docs/credenciais.md`](../docs/credenciais.md)
- [`docs/config/organizacao.md`](../docs/config/organizacao.md)
- [`docs/skills/`](../docs/skills/)

---

<div align="center">

**🏛️ Governo do Estado do Rio de Janeiro**

<sub>Desenvolvido e mantido para uso institucional da DTIC/Detran-RJ.</sub>

</div>
