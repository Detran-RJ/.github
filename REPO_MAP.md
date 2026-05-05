# Detran-RJ — REPO_MAP

Atualizado: 2026-05-05

## Repositórios

| Repo | Status | Visib. | Papel |
|---|---|---|---|
| [.github](https://github.com/Detran-RJ/.github) | ativo | público | Perfil público, templates, segurança, skills e configuração organizacional |
| [knowledge-base](https://github.com/Detran-RJ/knowledge-base) | ativo | privado | Vault Obsidian privado, governança e futura wiki interna |
| [detran-ai](https://github.com/Detran-RJ/detran-ai) | ativo | privado | Prometheus + Atlas; agentes IA para SEI, patrimônio e conhecimento |
| [detran-apps](https://github.com/Detran-RJ/detran-apps) | ativo | privado | Apps internos: contratos, wiki e ferramentas DTIC |
| [detran-infra](https://github.com/Detran-RJ/detran-infra) | ativo | privado | CI reutilizável, políticas, dev-env, identidade e publicação segura |
| [detran-patrimonio](https://github.com/Detran-RJ/detran-patrimonio) | ativo | privado | Sistema de patrimônio DTIC/DETRAN |
| [detran-sei](https://github.com/Detran-RJ/detran-sei) | ativo | privado | Monorepo SEI com pipeline e bundles |
| [detran-sei-pipeline](https://github.com/Detran-RJ/detran-sei-pipeline) | ativo | privado | Pipeline SEI sanitizado e documentação operacional |

## Padrão de topics

- `detran-rj`
- `dtic`
- `status-active`
- `private-by-default`
- `governance`
- `ai-agents`
- `sei`
- `patrimonio`
- `contratos`
- `academy`
- `infra`
- `deploy-vercel`
- `deploy-huggingface`
- `deploy-vps`

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
